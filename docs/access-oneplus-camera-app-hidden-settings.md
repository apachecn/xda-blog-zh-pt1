# 启用隐藏功能并调整一加相机应用程序中的所有设置

> 原文：<https://www.xda-developers.com/access-oneplus-camera-app-hidden-settings/>

对一加设备的抱怨之一是它们缺乏严肃的专业摄影功能。即使这些设备背后有强大的第三方开发者社区，它们从实际公司获得的相机功能定制方面的爱往往太少。

尽管如此，一加相机应用程序有自己隐藏的内部菜单，供一加工程师用于调试和测试。普通用户通常无法打开该菜单，因为相应的活动在相机应用程序中没有直接访问的方式。但是，如果您的设备具有 root 访问权限，则可以进入此内部菜单。正如 XDA 成员 [CoinsClassic](https://forum.xda-developers.com/m/coinsclassic.8727958/) 所发现的那样，你可以摆弄一些核心相机参数，解锁一些在普通配置中被禁用的功能。

按照本教程，你需要解锁你的设备的引导程序，并刷新一个 Magisk 补丁的引导镜像。

* * *

### 使用亚行

[在 PC/Mac 上安装 Android Debug Bridge(ADB)](https://www.xda-developers.com/install-adb-windows-macos-linux/)，将手机连接到电脑，授予调试权限。接下来，在命令提示符/Shell/终端窗口中键入以下命令:

```
 <span >adb shell</span> 
```

```
 <span >su</span> 
```

当手机提示时，授予超级用户访问“shell”的权限。

```
 <span >am start </span><span >-</span><span >n </span><span >"com.oneplus.camera/com.oneplus.camera.FeatureEditorActivity"</span> 
```

现在，您将看到手机上的内部菜单打开。

### 使用终端模拟器

打开您选择的终端模拟器应用程序。建议使用 Termux ，但是任何可以访问终端的设备都可以。键入以下命令:

```
 <span >su</span> 
```

当设备上出现提示时，授予超级用户访问权限。

```
 <span >am start </span><span >-</span><span >n </span><span >"com.oneplus.camera/com.oneplus.camera.FeatureEditorActivity"</span> 
```

内部菜单将在您的设备上打开。

### 使用活动启动器

下载并安装一个类似[这个](https://play.google.com/store/apps/details?id=de.szalkowski.activitylauncher)的活动启动程序。授予应用程序的超级用户访问权限，搜索一加相机应用程序(包名`com.oneplus.camera`)，并打开名为`FeatureEditorActivity`的活动。

内部菜单将在您的设备上打开。

### 使用 x 曝光

XDA 成员 [Alex193a](https://forum.xda-developers.com/m/alex193a.6183014/) 已经[想出了一个方便的曝光模块](https://twitter.com/alex193a/status/1381738317146947588)来启用一加相机应用程序中的隐藏内部菜单，但是有一个问题。由于不再支持 Xposed 框架的正式版本，您需要选择一个第三方分支，如带有 [EdXposed 管理器](https://github.com/ElderDrivers/EdXposedManager/releases)的 [Riru](https://github.com/RikkaApps/Riru/releases) ，以便安装该模块。

设置 Riru 和 EdXposed 后，从[这里](https://xposed.alex193a.com/download/oneplus-camera-debug-mode-enabler/)下载并安装模块。然后重新启动设备，并确保该模块允许挂钩相机应用程序(com.oneplus.camera)。如果一切正常，应该可以在相机的设置部分下访问该菜单。

* * *

## 说明

我们使用 ADB 或第三方活动启动器应用程序来启动`FeatureEditorActivity`，这是隐藏的内部菜单活动的名称。这个内部菜单中有一些设置和调整，一加相机应用程序的用户可能会从中受益。这个菜单意味着只有应用程序的开发者和测试者才能访问，所以你可以做很多事情。向下滚动查看一些示例。

* * *

使用过滤器框搜索参数，并根据其数据类型编辑值。例如，如果您想在录制 4K60fps 的 HEVC 视频时增加比特率，您只需通过[改变相应变量](https://forum.xda-developers.com/t/root-op-camera-app-edit-all-oneplus-camera-features-bitrate-image-quality-thresholds-etc.4246555/)的值，如下所示:

你也可以通过搜索普通车型的名字来找到一加 8T 赛博朋克 2077 版的相机滤镜。

但是，等等，还有更多——回传部分。[一加 9](https://www.xda-developers.com/oneplus-9/) 和[一加 9 Pro](https://www.xda-developers.com/oneplus-9-pro-review/) 推出了新版本的相机应用程序，该应用程序具有基于[哈苏图像处理软件](https://www.xda-developers.com/oneplus-9-series-march-23-hasselblad-partnership-confirmed/)的新用户界面和一些令人兴奋的新功能。不仅可以在旧的一加设备上从一加 9 下载更新的相机应用[，还可以通过隐藏菜单](https://forum.xda-developers.com/t/oneplus-9-pro-stock-camera-apk.4251731/post-84715545)[解锁一系列额外功能](https://forum.xda-developers.com/t/root-op-camera-app-edit-all-oneplus-camera-features-bitrate-image-quality-thresholds-etc.4246555/post-84717933)。

* * *

如果你发现一加相机应用程序中隐藏的任何其他有用的功能，请在下面的评论中告诉我们！