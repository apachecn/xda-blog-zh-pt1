# Access Dots 将 iOS 14 风格的隐私点添加到您的 Android 设备中

> 原文：<https://www.xda-developers.com/access-dots-brings-ios-14-style-privacy-dots-to-any-device-running-android-7-0/>

在 Android 6.0 中，Google 为外部存储、摄像头、位置等敏感权限引入了新的运行时权限模型。这个模型在 Android 9 之前没有太大的改进。但在 Android 10 中，谷歌最终引入了特殊版本的运行时权限，允许用户仅在应用程序处于活跃使用状态时授予位置权限。Android 11 [将一次性权限模型](https://www.xda-developers.com/android-11-developer-preview-privacy-security-features-changes/)扩展为两个更敏感的权限:摄像头和麦克风。虽然所有这些改进都带来了更大的透明度，并使 Android 用户能够更好地控制应用程序如何利用敏感权限，但如果用户能够实时看到某个应用程序何时访问摄像头、麦克风、位置等，将会更加直观。

苹果新发布的 iOS 14 更新以[隐私指示器](https://support.apple.com/en-us/HT211876)的形式拥有这一功能。当应用程序访问您的麦克风或摄像头时，它会在状态栏中显示橙色和绿色指示器。虽然 [Android 12 可能会添加功能](http://xda-developers.com/android-12)，但 XDA 公认的开发者 [*jagan2*](https://forum.xda-developers.com/m/jagan2.1884109/) 已经主动将 iOS 风格的隐私指示器带到任何运行 Android 7.1.2 及以上版本的智能手机上。在之前，我们已经[报道过](https://www.xda-developers.com/access-dots-brings-ios-14s-camera-and-mic-access-indicators-to-android/)这款应用[两次，但它将回到我们的首页，因为它的最新更新增加了对 GPS 指示器的支持。](https://www.xda-developers.com/access-dots-logs-camera-microphone-accessed/)

与苹果的实现类似，Access Dots 在状态栏中显示一个小点，以指示应用程序何时使用摄像头、麦克风和位置。

Access Dots 依靠辅助服务来完成它的工作。虽然应用程序本身不会请求摄像头和麦克风的权限，但如果您希望使用位置访问点，则需要授予 GPS 权限。该应用程序还维护一个日志，显示请求权限的确切时间，请求访问时哪个应用程序在前台，以及访问持续了多长时间。

每个圆点的颜色可以根据自己的喜好定制，也可以选择希望圆点弹出的位置。例如，您可以让圆点显示在自拍相机的右侧或左侧，右上角或左上角，或者底部。而且，你还可以自定义圆点的大小。

**[访问圆点 XDA 线程](https://forum.xda-developers.com/t/app-7-0-access-dots-android-12-ios-14-privacy-indicators-cam-mic-gps-for-all.4135219/)**

以下是接入点主要功能的概要:

*   每当手机的摄像头/麦克风/GPS 位置被第三方应用程序占用时，显示*访问点*
*   维护访问日志，可从应用程序的主设置屏幕访问。*访问日志*显示摄像头/麦克风/GPS 位置何时被访问，*在访问开始时哪个* App 在前台，以及*ho*w 访问持续了多长时间。
*   给任一个*访问点*分配任意颜色。
*   在 Android 10+上， *Access Dots* 默认贴在你的摄像头切口旁边(如果你的设备有。)您可以将接入点的位置配置到指定 X/Y 坐标的位置。
*   如果你的设备支持“能量环-通用版！”App，那么你也可以在打孔摄像头周围环绕接入点。
*   *接入点*的大小可以调整。