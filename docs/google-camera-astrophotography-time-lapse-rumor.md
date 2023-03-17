# 谷歌相机更新可以让你拍摄天体摄影延时照片

> 原文：<https://www.xda-developers.com/google-camera-astrophotography-time-lapse-rumor/>

在谷歌[于 2019 年推出 Pixel 4 系列](https://www.xda-developers.com/google-pixel-4-specs-features-pricing-availability/)后，该公司开始定期在所谓的“ [Pixel 功能下降](https://www.xda-developers.com/tag/pixel-featuredrops/)中发布新的软件功能第一次这样的发布发生在 2019 年 12 月，而最近的一次发生在 2021 年 3 月初。我们预计下一个像素功能将于 6 月 7 日——本月的第一个星期一——与 2021 年 6 月的安全补丁一起登陆。在发布之前，谷歌已经对其 Pixel Tips 应用程序进行了新的更新，该应用程序可以向 Pixel 所有者介绍新功能。虽然更新没有透露太多关于即将到来的像素功能下降的信息，但它确实暗示了谷歌相机应用程序可能会有一个新功能:天体摄影延时。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Pixel Tips 应用程序的 3.4.0.373287606 版本今天在谷歌 Play 商店上推出，在对其进行反编译后，我们发现了一个名为“cameraastortimelapsesettingcontroller”的新类如果谷歌相机应用程序的安装版本是 8.2.3 或更高版本(最新的公开版本是 8.2.204)，那么 Pixel Tips 应用程序将显示“CameraAstrotimelapse”提示。我们无法访问谷歌相机应用程序的 8.2.3 版本，也无法访问这个新的“CameraAstrotimelapse”提示的资产，但我们根据名称和版本检查猜测，这个功能将出现在下一个谷歌相机版本中。

至于它将如何工作，它可能会非常简单。谷歌相机应用程序将可能能够在设定的时间内(例如 1-2 小时)每隔几分钟自动拍摄一次天体照片。这会让你捕捉到星空的动人镜头。目前，天体照相术可以在曝光最长 4 分钟后拍摄一张星空图像。

天文摄影在 Pixel 3 和更高版本的上的谷歌相机应用[中可用，尽管它](https://support.google.com/googlecamera/answer/9708795/take-photos-in-low-light-or-at-night-on-your-pixel-phone?hl=en)[不支持 Pixel 4a 5G 或 Pixel 5 上的广角镜头](https://www.xda-developers.com/google-disables-ultra-wide-angle-astrophotography-pixel-5-pixel-4a-5g/)。另一方面，延时摄影在 Pixel 手机[上的使用时间比天文摄影稍长一点](https://www.xda-developers.com/google-pixel-smartphones-time-lapse-google-camera/)，尽管这是一个非常简单的功能，你可以在许多其他相机应用程序中找到。谷歌[在开发天体摄影](https://www.xda-developers.com/google-explains-pixel-4s-astrophotography-works-shares-tips/)上投入了大量精力，所以很高兴看到它通过与延时模式相结合而变得更加有用。

最新 Pixel Tips 版本中添加的另一个类称为“CameraLockedFolderSettingController”，但这很可能与谷歌在 2021 年 I/O 上宣布的“安全文件夹”功能有关。

* * *

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*