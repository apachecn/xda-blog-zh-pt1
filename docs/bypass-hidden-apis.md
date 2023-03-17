# 如何绕过 Android 9+上隐藏的 API 黑名单

> 原文：<https://www.xda-developers.com/bypass-hidden-apis/>

早在 2018 年，谷歌就发布了 Android Pie。在 UI 变化和新特性中，也有一些开发人员方面的变化。这些变化包括新的 API，现有 API 的错误修复，以及对访问隐藏 API 的限制。

幸运的是，有办法绕过这些限制。在我开始讨论如何绕过这些限制之前，我应该解释一下什么是隐藏 API，为什么它们首先受到限制，以及为什么您可能想要访问它们。

## 什么是隐藏 API？

隐藏 API 是 Android 中的 API，应用程序开发人员通常看不到。如果你看一下 AOSP 的代码，你会看到一大堆类、变量和方法在它们上面的注释块中有一个`@hide`注释。

该注释指示 Google 在编译 SDK 时使用任何工具来排除其下的项目。该 SDK 随后被分发给通过 Android Studio 下载的 SDK 中的开发人员。除非你使用修改过的 SDK，否则 Android Studio 会认为这些隐藏的项目根本不存在。如果你尝试直接使用一个，它会用红色显示，拒绝编译。

## 为什么 API 是隐藏的？

API 被隐藏的原因有很多。有些东西只能由内部或系统应用程序使用，如果由第三方应用程序使用，将不起作用。其他的是实验性的或不稳定的，将来可能会被删除或改变。有些甚至只是 API，谷歌只是不想苹果正常的折旧周期，如果他们曾经被删除。

## 为什么要使用隐藏 API？

虽然标准的 Android SDK 中有很多内容，但有时还不够。有时候你想做的事情已经存在于 Android 中，只是没有公开而已。

例如，我开发的很多应用，包括[系统界面调谐器](https://forum.xda-developers.com/t/app-6-0-systemui-tuner.3588675/)和[锁屏小工具](https://forum.xda-developers.com/t/android-5-1-lockscreen-widgets.4097817/)，都使用了一堆不同的隐藏 API。SystemUI Tuner 需要访问一些以正确跟踪、更改和重置选项。Lockscreen Widgets 使用一些来显示它下面的壁纸，等等。

大多数开发人员不需要访问隐藏的 API，但有时它们非常有用。

## 隐藏 API 是如何被限制的？

随着 Android 9 (Pie)的发布，Google 引入了隐藏 API 黑名单。并不是每个隐藏的 API 都包含在内，并且有不同级别的列表。白名单上隐藏的 API 可以被任何人访问。浅灰色列表中的隐藏 API 可以被任何应用程序访问，但在未来版本的 Android 中可能无法访问。暗灰色列表中的任何内容都只能由针对 Pie 之前的 API 级别(即 API 级别 28 之前)的应用程序访问。针对 Pie 和更高版本的应用将被拒绝访问。最后，黑名单上隐藏的 API 不能被任何非系统(或非白名单)应用程序访问，无论目标 API 是什么。

Android 10 改变了列表的组织方式，并略微简化了它们，但想法保持不变。某些隐藏的 API 可以被应用程序访问，而其他的则被阻止。Android 11 [加强了访问检测](https://www.xda-developers.com/android-11-harden-hidden-api-restriction-meta-reflection/)到[阻断一个用于 Pie 和 10 的旁路](https://www.xda-developers.com/android-development-bypass-hidden-api-restrictions/)。

在所有 Android 版本中，每当第三方应用程序试图访问黑名单中的隐藏 API 时，Android 都会抛出相应的“未找到”错误。

## 如何绕过隐藏的 API 黑名单

实际上有相当多的方法可以通过隐藏的 API 黑名单。根据您的需求，您可以选择适用于所有 Android 版本的版本、仅适用于 Android 9 和 10 的版本、使用原生 C++代码的版本以及完全基于 Java 的版本。甚至有一个使用 ADB 的开发专用解决方案。

### 亚行变通办法

如果您的设备运行 Android Pie，运行以下两个 ADB 命令来启用隐藏的 API 访问。

```
 adb shell settings put global hidden_api_policy_pre_p_apps 1
adb shell settings put global hidden_api_policy_p_apps 1 
```

如果您的设备运行的是 Android 10 或更高版本，请运行以下 ADB 命令来启用隐藏的 API 访问。

```
 adb shell settings put global hidden_api_policy 1 
```

要恢复默认行为，只需用`delete`替换`put`，并移除`1`。

显然，这些命令对于生产应用程序来说并不十分有用。我可以直接告诉你，正确地指导用户如何使用 ADB 是非常困难的。但是如果你需要更新旧的应用程序以符合新的限制，它们会很有用。

### 本地/JNI 解决方案

有两种方法可以在你的 Android 应用中使用 JNI 绕过隐藏的 API 黑名单。一个适用于 Android 9 和 10，另一个适用于 Android 9 和更高版本。

#### 安卓 9 和 10

如果你已经有了应用的原生部分，这将很容易实现。使用`JNI_OnLoad()`功能即可。

static art::Runtime * Runtime = nullptr；

```
 extern "C" jint JNI_OnLoad(JavaVM *vm, void *reserved) {
    ...
    runtime = reinterpret_cast<art::JavaVMExt*>(vm)->GetRuntime();
    runtime->SetHiddenApiEnforcementPolicy(art::hiddenapi::EnforcementPolicy::kNoChecks);
    ...
} 
```

要知道这个方法只在 Android 9 和 10 上有效。

#### Android 9 及更高版本

对于任何版本的 Android，您都可以选择两个库来绕过隐藏的 API 限制:FreeReflection 和 RestrictionBypass。

两者都易于实现和使用。

**要实现 FreeReflection** ，将依赖项添加到你的模块级 build.gradle 中。

`implementation 'me.weishu:free_reflection:3.0.1'`

然后在应用程序类中覆盖`attachBaseContext()`。

```
 @Override
protected void attachBaseContext(Context base) {
    super.attachBaseContext(base);
    Reflection.unseal(base);
} 
```

如果您没有应用程序类，您可以非常容易地添加它。创建一个扩展`Application`的新类，然后在 AndroidManifest.xml 中指向它。

示例:

```
 public class App extends Application {
    ...
    @Override
    protected void attachBaseContext(Context base) {
        super.attachBaseContext(base);

        Reflection.unseal(base);
    }
} 
```

```
 <manifest>
    ...
    <application
        ...
        name=".App">
        ...
    </application>
</manifest> 
```

**要实现 RestrictionBypass** ，将 JitPack 存储库添加到您的项目级 build.gradle。

```
 allprojects {
    repositories {
        ...
        maven { url "https://jitpack.io" }
    }
} 
```

然后将依赖项添加到模块级 build.gradle 中。

```
 implementation 'com.github.ChickenHook:RestrictionBypass:2.2' 
```

仅此而已。该库自动删除黑名单限制。

### Java 变通方法

虽然 JNI 解决方案是有效的，但有时您可能不希望使用本机代码。如果你还没有用 C++做过一些事情，它会给你的应用程序增加不必要的大小和平台限制。幸运的是，只使用 Java 就有办法绕过隐藏的 API 黑名单。

#### 安卓 9 和 10

在 Android 9 和 10 中，你可以使用所谓的双反射或元反射来绕过隐藏的 API 黑名单。因为系统只检查第三方应用程序正在调用什么，双反射欺骗它认为系统正在进行隐藏的 API 调用。

这个技巧可以用来调用一个方法来给你的应用程序隐藏 API 豁免，恰当地命名为`setHiddenApiExemptions()`。只需在应用生命周期的早期添加以下代码(比如应用的`onCreate()`方法)，它就能绕过黑名单。

```
 Method forName = Class.class.getDeclaredMethod("forName", String.class);
Method getDeclaredMethod = Class.class.getDeclaredMethod("getDeclaredMethod", String.class, Class[].class);

Class vmRuntimeClass = (Class) forName.invoke(null, "dalvik.system.VMRuntime");
Method getRuntime = (Method) getDeclaredMethod.invoke(vmRuntimeClass, "getRuntime", null);
Method setHiddenApiExemptions = (Method) getDeclaredMethod.invoke(vmRuntimeClass, "setHiddenApiExemptions", new Class[] { String[].class} );

Object vmRuntime = getRuntime.invoke(null);
setHiddenApiExemptions.invoke(vmRuntime, new String[][] { new String[] { "L" } }); 
```

如果你的应用程序与低于 9 的 Android 版本兼容，记得在版本检查中包含这个。

#### Android 9 及更高版本

要绕过 Android 9 和任何更高版本上隐藏的 API 黑名单，可以使用 LSPosed 的库。这个库使用 Java 的不安全 API，所以它不太可能会崩溃。

要实现它，只需将依赖项添加到您的模块级 build.gradle 中。

```
 implementation 'org.lsposed.hiddenapibypass:hiddenapibypass:2.0' 
```

然后用它绕过黑名单。

```
 HiddenApiBypass.addHiddenApiExemptions("L"); 
```

如果你的应用程序与低于 9 的 Android 版本兼容，记得在版本检查中包含这个。

## 结论和更多信息

无论你使用哪个平台版本，都有很多方法可以绕过 Android 上隐藏的 API 黑名单。如果您想了解更多关于这些方法和库如何工作的信息，请务必查看以下链接。