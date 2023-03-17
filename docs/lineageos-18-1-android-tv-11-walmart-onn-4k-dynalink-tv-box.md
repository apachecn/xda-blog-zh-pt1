# LineageOS 18.1 版本将 Android 11 引入 Amlogic G12 Android 电视机顶盒

> 原文：<https://www.xda-developers.com/lineageos-18-1-android-tv-11-walmart-onn-4k-dynalink-tv-box/>

沃尔玛的 Onn 和 Dynalink 安卓电视盒子是美国市场上最好的安卓电视流媒体设备中的两个。它们的价格都不到 50 美元，并提供一系列功能，包括 4K HDR 支持和伟大的遥控器。然而，他们都缺少的是最新版本的安卓电视。我们不知道这些设备何时会更新到 Android 11。好消息是，由于一个非官方的 LineageOS 端口，可以在这些设备上安装和运行最新版本的 Android。

如果你拥有一款采用 Amlogic G12/SM1 系列 SOC 芯片的产品，其中不仅包括前面提到的沃尔玛 Onn 4K 盒子和沃尔玛 Dynalink 4K 盒子，还包括谷歌 ADT-3 和 Chromecast 以及谷歌电视，那么由于多个开发人员的努力，安装 Android TV 11 是可能的。在 [XDA 的 Android TV 论坛](https://forum.xda-developers.com/c/android-tv.4276/)上，一个新的论坛主题是为 Amlogic G12/SM1 系列设备的基于 Android 11 的非官方构建的 LineageOS 18.1。开发者诺伦·约翰逊( [npjohnson](https://forum.xda-developers.com/m/npjohnson.5848265/) )、扬·阿尔滕森( [Stricted](https://forum.xda-developers.com/m/stricted.8184192/) )、 [webgeek1234](https://forum.xda-developers.com/m/steel01.1416222/) 、 [deadman96385](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiqtrnznZPyAhVbHM0KHaD9B7gQFjAAegQIAhAD&url=https%3A%2F%2Fforum.xda-developers.com%2Fm%2Fdeadman96385.4222965%2F&usg=AOvVaw22Hnvdi1uuwWvCqv-u5RzM) 、trautamaki、 [luca020400](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjWiIf8nZPyAhXKWM0KHfSYCFgQFjAAegQIBRAD&url=https%3A%2F%2Fforum.xda-developers.com%2Fm%2Fluca020400.5778309%2F&usg=AOvVaw2h7sAtrHuW7-K39Pbk38Tg) 和 [aleasto](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiv8NX_nZPyAhVbG80KHZMvBWgQFjAAegQIBBAD&url=https%3A%2F%2Fforum.xda-developers.com%2Fm%2Faleasto.4742143%2F&usg=AOvVaw2pKjorEhG7Wv0ZEZJqv9bG) 可以归功于他们使这个端口成为可能。尽管他们都是 LineageOS 的定期贡献者，但这个端口不是由 LineageOS 正式构建或发布的，因此它被认为是“非官方”的。

许多股票 Android TV 应用程序和组件都是封闭源代码的，所以尽管这个 LineageOS 18.1 版本在技术上不能被认为是“Android TV 11”，但它确实提升了“谷歌电视的一些更好的组件”。这包括谷歌预建的无 GMS 电视发射器等。其他的 Google Apps 都内置在 ROM 版本中，所以你不需要在安装版本后刷新一个单独的 Google Apps 包。

更重要的是，开发人员报告说似乎没有什么大的问题。大多数核心功能，包括遥控器和麦克风，都工作正常。当你解锁引导程序时，Widevine L1 DRM 不会被破坏，这意味着你可以播放来自网飞或亚马逊 Prime Video 等流媒体服务的高清视频。然而，开发人员指出，硬件支持的 OMX 问题会妨碍网飞的 Android TV 应用程序正常运行，所以建议你在解决这个问题之前，从侧面加载该应用程序的平板电脑版本。另一个警告是，SELinux 策略被设置为许可，这通常是一个主要的安全问题，但希望您不会访问或保存任何敏感数据。如果你遇到罕见的检查安全网的电视应用程序，那么开发者注意到你可以[安装 Magisk](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjW48f6opPyAhULCc0KHRKlBFUQFjABegQIBBAD&url=https%3A%2F%2Fwww.xda-developers.com%2Fhow-to-install-magisk%2F&usg=AOvVaw2K-4FNhQcC_7z2Rc0ZwM0T) 来通过这些检查。

至于为什么有人会对在他们的 Android 电视盒子上安装 LineageOS 18.1 感兴趣，这有几个好处。首先，这个版本完全没有膨胀软件，不像许多便宜的电视机顶盒附带的固件。第二，没有广告。第三，它运行的是更新的 Android 版本，这意味着你可以使用 Android 11 中引入的一些新功能。最后，这些电视盒子非常便宜，所以修理它们可能是一个有趣的周末项目！

## 下载适用于 Amlogic G12/SM1 系列设备的 LineageOS 18.1

如果所有这些听起来都让你兴奋，你可以在下面链接的每个设备的相应 wiki 页面上找到解锁引导加载程序、闪存沿袭恢复和安装 ROM zip 的步骤:

解锁沃尔玛 Onn 和 Dynalink 盒子的引导加载程序非常简单，但要用谷歌电视的引导加载程序解锁 Chromecast，你需要一个容易受到我们上周详细介绍的[引导加载程序解锁漏洞](https://www.xda-developers.com/chromecast-with-google-tv-bootloader-unlock-exploit/)攻击的模型。

关于这个版本的更多细节，请点击下面的论坛链接。

**[【非官方】linegeos 18.1 for Amlogic G12 */SM1 家族器件](https://forum.xda-developers.com/t/unofficial-lineageos-18-1-for-amlogic-g12-sm1-family-devices.4313743/)**

* * *

**更新 1 (09/20/2021 @美国东部时间上午 11:53):**本文已更新，以反映 LineageOS 18.1 版本[已发布](https://forum.xda-developers.com/t/unofficial-lineageos-18-1-for-amlogic-g12-sm1-family-devices.4313743/page-13#post-85627031)用于带有谷歌电视的谷歌 Chromecast。