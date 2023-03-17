# 如何使用滴库提升应用权限

> 原文：<https://www.xda-developers.com/implementing-shizuku/>

通常授予您的应用程序的权限可能不够，原因有很多。也许你和我一样，喜欢创建滥用 Android API 的黑客应用程序。我使用的一些 API 被锁定在特殊权限之后。有时只有 shell 用户(ADB)或系统可以访问它们。不过有一个解决方案——滴。

滴允许你几乎直接调用系统 API，而且完全用 Java 或 Kotlin。本指南将向您展示如何实现和使用滴。

## 什么是滴？

在我们开始使用滴之前，知道它到底是什么可能会有所帮助。如果你熟悉 Magisk，那么滴也差不多。但是它不是管理 root 访问，而是管理 shell 访问。

滴使用 shell 级别的权限运行自己的进程。用户如何激活这个过程取决于他们的设备、Android 版本和选择。滴可以通过 ADB、通过设备上的无线 ADB(Android 11 上的[和之后的](https://www.xda-developers.com/android-11-developer-preview-3-announced/))或通过 root 访问来激活。实现滴的应用程序可以请求使用该进程来执行提升的操作。

## 为什么是滴？

虽然对系统的外壳级访问不能让你像根用户那样做很多事情，但它仍然给你比普通应用程序更多的访问权限。最重要的是，滴的工作方式让你可以像平常一样使用 Android APIs。您不必依赖 shell 命令(尽管如果您愿意的话也可以)。

如果你的应用程序需要特殊权限，只能通过亚行(或 root)授予，滴和 Android 11 是一个很好的配对。您可以只使用滴授予特殊权限完全在设备上。

即使在没有安装 Android 11 的设备上，滴也很有用。该应用程序为用户提供了说明和脚本，所以你不必。

## 综合

将滴添加到你的应用程序中不是最简单的，但也不难。不幸的是，[开发者文档](https://github.com/RikkaApps/Shizuku-API)并不完全完整，但是这篇文章已经涵盖了。以下是如何将滴集成到您的应用程序中。

### 属国

第一步是添加滴依赖项。在模块级 build.gradle 中，将以下内容添加到 dependencies 块中。

```
 def shizuku_version = '11.0.3'

implementation "dev.rikka.shizuku:api:$shizuku_version"
implementation "dev.rikka.shizuku:provider:$shizuku_version" 
```

如果需要，请确保更新版本。11.0.3 是撰写本文时的最新版本。

### 供应者

为了让滴正常工作，您需要向您的应用程序清单中添加一个提供者块。打开 AndroidManifest.xml 并在应用程序块中添加以下内容。

```
 <provider
    android:name="rikka.shizuku.ShizukuProvider"
    android:authorities="${applicationId}.shizuku"
    android:multiprocess="false"
    android:enabled="true"
    android:exported="true"
    android:permission="android.permission.INTERACT_ACROSS_USERS_FULL" /> 
```

### 许可

对于授权，滴使用运行时权限。我们一会儿将讨论如何授予这种许可。现在，将其添加到 Manifest 块内的 AndroidManifest.xml 中。

现在所有这些都已添加完毕，基本的集成工作也完成了。让 Gradle 做一个项目同步，并继续使用。

* * *

## 使用

### 检查可用性

在讨论如何使用滴之前，让我们先讨论一下如何确保它确实可用。

在检查权限是否被授予之前，以及在通过滴进行 API 调用之前，您可以使用以下方法确保这些检查和调用将会成功:

`Shizuku.pingBinder()`

如果滴安装并运行，这将返回**真**。否则，它将返回 false。

### 授予许可

因为滴使用运行时权限，所以在你可以用 shell 访问做任何事情之前，它必须被授予你的应用程序。还有两个 API 版本在流通，有不同的授予方式。本节将向您展示如何处理这两个问题。

#### 检查

在你请求许可之前，最好的办法是检查你是否已经有了许可。如果你这样做了，你可以继续做你需要做的事情。否则，您需要在继续之前请求它。

要检查您是否有权限使用滴，您可以使用以下内容。这段代码假设您正在一个活动中运行它。

**锅炉**:

```
 val isGranted = if (Shizuku.isPreV11() || Shizuku.getVersion() < 11) {
    checkSelfPermission(ShizukuProvider.PERMISSION) == PackageManager.PERMISSION_GRANTED
} else {
    Shizuku.checkSelfPermission() = PackageManager.PERMISSION_GRANTED
} 
```

**Java** :

```
 boolean isGranted;
if (Shizuku.isPreV11() || Shizuku.getVersion() < 11) {
    isGranted = checkSelfPermission(ShizukuProvider.PERMISSION) == PackageManager.PERMISSION_GRANTED;
} else {
    isGranted = Shizuku.checkSelfPermission() == PackageManager.PERMISSION_GRANTED;
} 
```

#### 要求

如果您需要申请使用滴的许可，以下是方法。

下面使用的 **SHIZUKU_CODE** 变量应该是一个具有稳定值的整数(静态变量)。

**锅炉**:

```
 if (Shizuku.isPreV11() || Shizuku.getVersion() < 11) {
    requestPermissions(arrayOf(ShizukuProvider.PERMISSION), SHIZUKU_CODE)
} else {
    Shizuku.requestPermission(SHIZUKU_CODE)
} 
```

**Java** :

```
 if (Shizuku.isPreV11() || Shizuku.getVersion() < 11) {
    requestPermissions(new String[] { ShizukuProvider.PERMISSION }, SHIZUKU_CODE);
} else {
    Shizuku.requestPermissions(SHIZUKU_CODE);
} 
```

为了监听结果，您需要覆盖 Activity 的**onRequestPermissionsResult()**方法。你还需要实现**滴。OnRequestPermissionResultListener**。我将要展示的例子假设您的活动实现了那个接口，但是如果您愿意，您可以在一个变量中实现它。

**锅炉**:

```
 class ExampleActivity : AppCompatActivity, Shizuku.OnRequestPermissionResultListener {
    ...

    override void onRequestPermissionsResult(requestCode: Int, permissions: Array<String>, grantResults: IntArray) {
        permissions.forEachIndexed { index, permission ->
            if (permission == ShizukuProvider.PERMISSION) {
                onRequestPermissionResult(requestCode, grantResults[index])
            }
       }
    }

    override void onRequestPermissionResult(requestCode: Int, grantResult: Int) {
        val isGranted = grantResult == PackageManager.PERMISSION_GRANTED
        //Do stuff based on the result.

    }
} 
```

**Java** :

```
 public class ExampleActivity extends AppCompatActivity implements Shizuku.OnRequestPermissionResultListener {
    ...

    @Override
    public void onRequestPermissionsResult(int requestCode, @NonNull String[] permissions, @NonNull int[] grantResults) {
        for (int i = 0; i < permissions.length; i++) {
            String permission = permissions[i];
            int result = grantResults[i];

            if (permission.equals(ShizukuProvider.PERMISSION) {
                onRequestPermissionResult(requestCode, result);
            }
        }
    }

    @Override
    public void onRequestPermissionResult(int requestCode, int grantResult) {
        boolean isGranted = grantResult == PackageManager.PERMISSION_GRANTED;
        //Do stuff based on the result.
    }
} 
```

### 使用 API

既然已经设置了滴并授予了权限，您就可以开始使用滴实际调用 API 了。这里的过程与您可能习惯的略有不同。不要调用`getSystemService()`并转换成类似`WindowManager`的东西，你必须使用这些内部 API(例如`IWindowManager`)。

滴包括一个绕过 Android 的隐藏 API 黑名单，所以你在使用它的时候不需要担心。如果你想知道如何自己绕过它，看看我以前的教程。

这里有一个简单的例子(使用反射),展示了如何获得一个`IPackageManager`的实例，并使用它授予一个应用程序运行时权限。

**锅炉**:

```
 val iPmClass = Class.forName("android.content.pm.IPackageManager")
val iPmStub = Class.forName("android.content.pm.IPackageManager\$Stub")
val asInterfaceMethod = iPmStub.getMethod("asInterface", IBinder::class.java)
val grantRuntimePermissionMethod = iPmClass.getMethod("grantRuntimePermission", String::class.java , String::class.java , Int::class.java )

val iPmInstance = asInterfaceMethod.invoke(null, ShizukuBinderWrapper(SystemServiceHelper.getSystemService("package")))

grantRuntimePermissionMethod.invoke(iPmInstance, "com.zacharee1.systemuituner", android.Manifest.permission.WRITE_SECURE_SETTINGS, 0) 
```

**Java** :

```
 Class<?> iPmClass = Class.forName("android.content.pm.IPackageManager");
Class<?> iPmStub = Class.forName("android.content.pm.IPackageManager$Stub");
Method asInterfaceMethod = iPmStub.getMethod("asInterface", IBinder.class);
Method grantRuntimePermissionMethod = iPmClass.getMethod("grantRuntimePermission", String.class, String.class, int.class);

val iPmInstance = asInterfaceMethod.invoke(null, new ShizukuBinderWrapper(SystemServiceHelper.getSystemService("package")));

grantRuntimePermissionMethod.invoke(iPmInstance, "com.zacharee1.systemuituner", android.Manifest.permission.WRITE_SECURE_SETTINGS, 0); 
```

其他 API 的过程类似。获取对该类及其存根子类的引用。获取对存根类的`asInterface`方法的引用。从类本身获取对所需方法的引用。然后，调用您拥有的`asInterface`方法引用，用您需要的任何服务替换上面的`"package"`。然后可以传递该实例进行方法调用。

如果你安装了一个修改过的 SDK，你可以完全避免使用反射。[查看 anggrayudi 的 GitHub 库](https://github.com/anggrayudi/android-hidden-api)获取修改后的 SDK 和安装说明。安装了这个之后，上面的代码(Kotlin)就变得简单多了。

```
 val iPm = IPackageManager.Stub.asInterface(ShizukuBinderWrapper(SystemServiceHelper.getService("package"))))
iPm.grantRuntimePermission("com.zacharee1.systemuituner", android.Manifest.permission.WRITE_SECURE_SETTINGS, 0)

```

任何基于 AIDL 的 API 都可以在你的应用中的任何地方使用这种方法，只要滴正在运行并且你的应用有权限。

### 用户服务程序

虽然 Binder 方法涵盖了大多数用例，但有时您可能需要一个没有直接 Binder 接口的 API。在这种情况下，您可以使用滴的用户服务功能。

这种方法的工作方式类似于 Android 中的普通服务。您“启动”它，通过使用 ServiceConnection 绑定到它来进行通信，并在 service 类中运行您的逻辑。不同的是，你没有使用 Android 的服务，服务内的任何东西都是在 ADB 许可下运行的。

现在有一些限制。用户服务在一个完全独立的进程和用户中运行，所以除了通过你自己的 AIDL 回调和绑定器，你不能与你的应用程序的其他部分交互。由于它也没有在正确的应用程序进程中运行，一些事情，如绑定 Android 服务，可能无法正常工作。

这也需要滴版本 10 或更高版本。虽然目前大多数应用程序的源代码都是版本 11，但是您仍然应该包含版本检查，这将包含在示例中。

#### 定义 AIDL

首先，您需要创建一个新的 AIDL 文件。你可以在 Android Studio 中这样做，右击 Android 文件视图中的任何东西，悬停在“新建”选项上，然后选择“AIDL”选项。输入文件名(如“IUserService”)，Android Studio 将为您创建一个模板文件。

如果你不熟悉 AIDLs 是如何工作的，一定要看看谷歌的文档。

从 AIDL 中删除模板方法，然后为滴添加一个具有适当 ID 的`destroy()`方法。当滴终止用户服务时，这个函数将被调用，并且应该被用来清理你拥有的任何引用或正在进行的逻辑。

AIDL 的例子:

```
 package tk.zwander.shizukudemo;

interface IUserService {
    void destroy() = 16777114;

    void grantPermission(String packageName, String permission, int userId) = 1; 
} 
```

#### 实施 AIDL

接下来要做的是实际实现 AIDL。

**Java** :

```
 public class UserService extends IUserService.Stub {

    public UserService() {
    }

    @Override
    public void destroy() {

        System.exit(0);
    }

    @Override
    public void grantPermission(String packageName, String permission, int userId) {

        IPackageManager.Stub.asInterface(SystemServiceHelper.getService("package")).grantRuntimePermission(packageName, permission, userId);
    }
} 
```

**锅炉**:

```
 class UserService : IUserService.Stub {

    constructor() {
    }

    override fun destroy() {

        System.exit(0)
    }

    override fun grantPermission(packageName: String, permission: String, userId: Int) {

        IPackageManager.Stub.asInterface(SystemServiceHelper.getService("package")).grantRuntimePermission(packageName, permission, userId)
    }
} 
```

上面的例子假设你已经安装了 [Android Hidden API](https://github.com/anggrayudi/android-hidden-api) SDK。

#### 设置服务连接

既然已经定义并实现了用户服务，那么是时候设置它以供使用了。您应该做的第一件事是定义一个您想要与之通信的 ServiceConnection(例如，从您的应用程序中的主活动)。

**Java** :

```
 private IUserService binder = null;

private final ServiceConnection connection = new ServiceConnection() {
    @Override
    public void onServiceConnected(ComponentName componentName, IBinder binder) {
        if (binder != null && binder.pingBinder()) {
            binder = IUserService.Stub.asInterface(binder);
        }
    }

    @Override
    public void onServiceDisconnected(ComponentName componentName) {
        binder = null;
    }
} 
```

**锅炉**:

```
 private var binder: IUserService? = null

private val connection = object : ServiceConnection {
    override fun onServiceConnected(componentName: ComponentName, binder: IBinder?) {
        if (binder != null && binder.pingBinder()) {
            binder = IUserService.Stub.asInterface(binder)
        }
    }

    override fun onServiceDisconnected(componentName: ComponentName) {
        binder = null;
    }
} 
```

`binder`变量是您将用来从应用程序与用户服务通信的变量。要检查它是否可用，只需检查它不为空，并且`pingBinder()`返回 **true** ，就像上面的代码示例一样。

#### 创建用户服务参数

在控制用户服务之前，您需要定义一些参数，供滴在启动和停止它时使用。这些包括实际告诉滴服务的类名，指定进程后缀，是否可调试，以及版本。

**Java** :

```
 private final Shizuku.UserServiceArgs serviceArgs = new Shizuku.UserServiceArgs(
    new ComponentName(BuildConfig.APPLICATION_ID, UserService.class.getName()))
        .processNameSuffix("user_service")
        .debuggable(BuildConfig.DEBUG)
        .version(BuildConfig.VERSION_CODE); 
```

**锅炉**:

```
 private val serviceArgs = Shizuku.UserServiceArgs(
    ComponentName(BuildConfig.APPLICATION_ID, UserService.class::java.getName()))
        .processNameSuffix("user_service")
        .debuggable(BuildCOnfig.DEBUG)
        .version(BuildConfig.VERSION_CODE) 
```

#### 启动、停止和绑定用户服务

开始和绑定操作以及停止和解除绑定操作在滴是统一的。没有单独的开始和绑定方法或者停止和解除绑定方法。

下面是如何**启动和绑定**用户服务。

**Java** :

```
 if (Shizuku.getVersion >= 10) {

    Shizuku.bindUserService(serviceArgs, connection);
} else {

} 
```

**锅炉**:

```
 if (Shizuku.getVersion() >= 10) {

    Shizuku.bindUserService(serviceArgs, connection)
} else {

} 
```

下面是如何**停止和解除**用户服务的绑定。

**Java** :

```
 if  (Shizuku.getVersion >= 10) {
    Shizuku.unbindUserService(serviceArgs, connection, true);
} 
```

**锅炉**:

```
 if (Shizuku.getVersion >= 10) {
    Shizuku.unbindUserService(serviceArgs, connection, true)
} 
```

#### 调用用户服务

一旦用户服务启动，您就可以开始使用它了。只需检查`binder`变量是否为非空且可 ping 通，然后进行方法调用。

**Java** :

```
 if (binder != null && binder.pingBinder()) {
    binder.grantPermission("com.zacharee1.systemuituner", android.Manifest.permission.WRITE_SECURE_SETTINGS, 0);
} 
```

**锅炉**:

```
 if (binder?.pingBinder() == true) {
    binder?.grantPermission("com.zacharee1.systemuituner", android.Manifest.permission.WRITE_SECURE_SETTINGS, 0)
} 
```

* * *

## 结论

如果您遵循了所有这些，您现在应该有一个工作的滴集成。只要记得告诉你的用户安装滴，并在尝试使用它之前正确检查滴是可用的。