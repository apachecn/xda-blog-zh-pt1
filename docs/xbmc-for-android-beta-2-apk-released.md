# 如何在 Android 上以 apk 或应用捆绑包的形式下载和安装应用

> 原文：<https://www.xda-developers.com/xbmc-for-android-beta-2-apk-released/>

应用程序是任何操作系统的生命线。没有[应用](https://www.xda-developers.com/best-android-apps/)，我们只能在像安卓这样的平台上，在我们[最喜欢的智能手机](https://www.xda-developers.com/best-android-phones/)上做这么多。幸运的是，Google Play 提供了数百万个应用，但由于平台限制，并不是每个好的应用都能在商店上找到。有时，应用程序的可用性也会受到地理位置的限制。因此，获得这类应用程序的唯一方法是侧装。

由于 Android 的开放性，你可以从第三方商店以及其他来源下载和安装 Android 应用程序。在本指南中，我们将解释如何下载 Android 应用程序。

## 获取 APK 文件或应用捆绑包

在 Android 上下载应用程序之前，你需要获取它的安装文件。Android 应用程序安装程序有。APK 文件扩展名是安卓包的缩写。APK 文件包含安装和运行应用程序所需的一切。除了 apk 之外，你还会发现应用捆绑包，它们也被用来安装 Android 应用。

有两种应用捆绑包——官方的和非官方的。官方的 Android 应用捆绑格式是 AAB，由谷歌在 2018 年推出。该公司强制要求应用程序开发者从 2021 年 8 月开始在 AAB 的 Google Play 商店发布所有新的 Android 应用程序。你也可以把一个标准的 AAB 包转换成一个 APK 文件集，它使用。apks 文件扩展名。

非官方的应用捆绑包来自 APKMirror 和 APKPure 等网站，它们分别创建了自己的应用捆绑包 APKM 和 XAPK。app bundles 打包了一个基本的 APK 文件和多个资源包，适用于不同的架构、布局和语言。

这些 APK 和应用捆绑包由开发者和社区成员在 XDA 论坛上分享，并上传到第三方资源，如 [APK 镜报](https://www.apkmirror.com/)、 [APKPure](https://apkpure.com) ，或商店，如 [F-Droid](https://f-droid.org/en/) 和[亚马逊](https://www.xda-developers.com/amazon-appstore-support-android-app-bundles/)。一旦您获得了 APK 文件或您需要安装的应用程序的应用程序包，我们就可以前进到实际的侧加载位。

**注意:**不要从随机来源安装 APK 文件。仅安装来源可靠的 APK 文件。否则，你的设备可能会感染恶意软件。

## 将 APK 或应用捆绑包传输到您的手机

如果你没有将 APK 文件或应用捆绑包直接下载到你的 Android 手机上，你需要将它从你的电脑转移到手机上。您可以使用蓝牙、USB 电缆或云存储服务来传输它。使用 Google Drive 等云存储服务通常是将 APK 安装到手机上的最简单方法。只需将它从你的电脑上传到 Google Drive，然后使用手机上的 Drive 应用程序下载即可。如果您正在寻找更多的文件传输方法，请查看我们关于如何在 Android 和 Windows PC 之间传输文件的指南。

## 安装/侧装 APK 文件

一旦 APK 传输到您的手机上，您就可以开始安装了。

*   在手机上找到该文件。下载的 apk 可以在下载应用程序中找到。或者您可以使用文件管理器导航到下载文件夹。
*   点击文件名开始安装。如果这是你第一次从文件管理器、下载应用程序或网页浏览器安装 APK，Android 会抛出一个警告并询问你是否允许继续。授予权限，根据您安装 APK 的应用程序，您可能需要点击“返回”才能进入安装程序。在某些应用程序中，你会被自动送回安装程序。
*   点击 *Install* ，应用将成功安装，除非存在兼容性问题。

如果你的 Android 设备运行的是 Nougat 或更老的版本，你必须首先通过进入**设置>安全**来启用来自未知来源的*安装，之后你就可以安装 APK 了。所有安卓版本都支持侧装，你不需要 [root](https://www.xda-developers.com/root) 权限或者任何其他特权。*

## Android 上的侧装应用捆绑包

虽然侧装一个 APK 非常容易，正如你在上一节中看到的，但安装应用捆绑包可能有点棘手，无论是官方的 Android 应用捆绑包还是非官方的捆绑包。令人欣慰的是，有一些应用程序使得安装应用程序包变得更加容易。或者，您可以使用 ADB 安装非官方的应用程序捆绑包，使用 Google 的 bundletool 安装官方的应用程序捆绑包。

### 如何使用 Split APKs 安装程序(SAI)安装应用程序包

Split APKs 安装程序支持 APKM 和 XAPK 应用程序包。

1.  要安装 APKM 或 XAPK 应用捆绑包，请从 Google Play 商店下载并安装 [SAI 应用。](https://play.google.com/store/apps/details?id=com.aefyr.sai)
2.  打开 SAI 并点击底部的*安装 APKs* 图标。
3.  现在，您可以使用应用程序的内部文件选择器或系统文件选择器来定位应用程序捆绑包。
4.  SAI 现在将自动从捆绑包中为您的设备选择正确的资源。在大多数情况下，自动选择的资源会工作得很好。如果觉得不对劲，也可以手动选择资源。
5.  点击*安装*继续。
6.  如果这是你第一次通过 SAI 安装应用捆绑包，你必须允许应用“*安装来自未知来源的应用*”。
7.  再次点击*安装*进行确认，app 就会安装到你的手机上。

### 如何使用应用捆绑包安装程序安装应用捆绑包

除了 APKM 和 XAPK 格式，应用捆绑安装程序还可以安装官方的 Android 应用捆绑(AAB)。

1.  从 Google Play 下载并安装[应用捆绑安装程序。该应用程序目前处于早期访问，所以你可能会看到一些错误。](https://play.google.com/store/apps/details?id=com.lifesavi.bundle.v2)
2.  打开应用捆绑包安装程序，并从底部栏中选择正确的应用捆绑包格式。你可以从 AAB，APKS，XAPK 和 APKM 中选择。普通的 apk 也可以用 app 安装。
3.  一旦选择了格式，您可以使用*扫描*或*选择*选项来选择应用捆绑包。
4.  点击*安装文件*继续安装。
5.  如果这是你第一次通过应用捆绑包安装程序安装应用捆绑包，你必须允许应用*安装来自未知来源的应用。*
6.  再次点击 *Install* 进行确认，App Bundle Installer app 将安装该应用。与 SAI 不同，App Bundle Installer 应用程序不提供手动选择应用程序资源的选项，而是自动为您的设备选择正确的资源。
7.  一旦应用程序安装完毕，你会看到一个确认。

### 使用 ADB 下载应用程序包

如果你已经在电脑上安装了 ADB，你可以用它来下载应用程序包，如 APKS(从 AAB 转换而来)、APKM 和 XAPK。要获得设置帮助，请查看我们的指南[如何在 Windows、Mac 和 Linux 上安装 ADB](https://www.xda-developers.com/install-adb-windows-macos-linux/)。

现在，要安装一个应用程序包，我们需要将其内容提取到一个文件夹中。你可以使用一个归档应用程序来提取它。如前所述，该包可以包括一个基本 APK 和用于不同应用程序二进制接口(ABI)、语言和屏幕 dpi 的各种资源 apk。如果你不确定你的设备的 ABI 或屏幕 DPI，你可以下载 [Droid 硬件信息](https://play.google.com/store/apps/details?id=com.inkwired.droidinfo)或 [DevCheck 硬件和系统信息](https://play.google.com/store/apps/details?id=flar2.devcheck)应用程序，并检查 ABI 和 DPI 的详细信息。您必须根据 ABI 和 DPI 数据，从提取的 apk 中为您的设备选择正确的 apk。

一旦 ADB 启动并运行，使用下面的命令安装 app bundle。确保将提取的 APK 文件放在平台工具或 ADB 文件夹中，以便于访问。如果需要，您也可以重命名它们。或者，如果您设置了 ADB 路径/别名，您也可以在包含提取的 apk 的文件夹中直接运行 ADB。

```
 adb install-multiple one.apk two.apk three.apk 
```

此命令会将应用程序安装到您的手机上。

如果捆绑包包括额外的不透明二进制 blobs(通常称为 OBB 文件)，您需要手动将它们复制到设备的内部存储/Android/OBB/ <package_name_of_the_app>文件夹中。</package_name_of_the_app>

* * *

这就是你如何在 Android 上下载 APK 文件和应用程序包。如果你认为我们错过了什么，请在评论区告诉我们。