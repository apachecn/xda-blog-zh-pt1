# 流行的条形码扫描仪应用转向恶意软件，感染 Android 设备

> 原文：<https://www.xda-developers.com/popular-barcode-scanner-app-caught-infecting-android-smartphones/>

# 流行的条形码扫描仪应用程序感染了 Android 智能手机

谷歌 Play 商店上一款流行的条形码扫描应用程序被发现用恶意软件感染安卓手机。请继续阅读，了解更多信息。

一款在谷歌 Play 商店下载量超过 1000 万的流行条形码扫描应用程序被发现用恶意软件感染安卓设备。这款名为*条形码扫描仪*的应用已经从 Play Store 中移除，但它很可能仍然存在于许多受感染的设备上。

顾名思义，*条形码扫描仪*应用是一个简单的应用，允许用户扫描条形码和二维码。但正如 [*的安全研究人员所发现的，这款应用在 12 月份接受了一次更新，添加了之前版本的应用中没有的恶意代码。研究人员指出，该应用程序使用了严重的模糊处理来避免检测。这种恶意更新在谷歌的*](https://blog.malwarebytes.com/android/2021/02/barcode-scanner-app-on-google-play-infects-10-million-users-with-one-update/) *[Play Protect 服务](https://www.xda-developers.com/google-play-protect-eset-lookout-zimperium-app-defense-alliance-store/)的雷达下确实有效，该服务正是为了检测和关闭这种恶意应用程序而设置的。Malwarebytes* 的研究人员能够确认该应用程序是由与以前版本相同的数字证书签署的，因此确认它来自同一个开发者 LavaBird LTD。

在使用*条形码扫描仪的情况下，*添加了之前版本的应用程序中没有的恶意代码。此外，添加的代码使用了严重的混淆来避免检测。

该应用在安装后几分钟内就活跃起来，开始用广告软件轰炸用户，并在没有用户交互的情况下自动将网页重定向到可疑网站。您可以在下面的视频中看到恶意活动:

Malwarebytes 称谷歌已收到私下通知，并已将该应用从 Play 商店下架。到目前为止，谷歌还没有使用它的 Play Protect 工具来通知那些仍然在手机上安装了这种恶意软件的用户。这意味着用户必须自己采取行动，从手机上删除该应用程序。

如果你的设备上安装了条形码扫描仪应用程序，并且最近注意到一些奇怪的行为，请前往应用程序设置并查找应用程序的包名称。如果 app 有包名**com . QR code scanner . barcode scanner**，立即卸载。