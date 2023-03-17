# Google Play Services 准备让你将应用程序传输到 Chromebook 上

> 原文：<https://www.xda-developers.com/google-play-services-stream-apps-to-chromebook/>

# Google Play Services 准备让你将应用程序流式传输到 Chromebook

Android 版 Google Play 服务的最新更新暗示了一项新功能，可以让你将手机中的应用程序传输到 Chromebook。

今天早些时候，Google Play 服务版本 21.21.12 开始向用户推出。上一个测试版本是 21.18.14，所以我们预计会有很多变化。虽然我们粗略地看了一眼，没有发现很多有趣的变化，但我们确实找到了进一步的证据，表明谷歌很快就会让用户将手机上的应用程序传输到连接的 Chromebook 上。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

以下字符串明确表示您可以将应用程序流式传输到 Chromebook，但它们没有提供该功能如何工作的任何细节:

```
 <string name="apps_stream_enabled_description">Stream apps to your Chromebook</string>
<string name="apps_stream_enabled_title">Apps</string> 
```

我的 Pixel 4 运行最新的 Google Play 服务版本，还没有这项功能。然而，由于二月份 Chromium code 的提示，我们一直期待这个特性能够登陆[。当时，我们得知谷歌正准备用应用流扩展](https://www.xda-developers.com/chrome-os-soon-support-mirroring-phones-screen/) [Chrome OS 的新手机中枢功能](https://www.xda-developers.com/chrome-os-phone-hub-new-features/)。未来，Chromebooks 将增加一个系统 Web 应用程序(SWA)，通过 WebRTC 同步视频和双向数据。据信该功能将为 Pixel 手机所独有，尽管我们从最新 Play Services 版本的初步观察中没有发现任何有关设备可用性的信息。

此版本中启用的一个功能是禁用 Cast 设备发现的切换。切换此选项将防止附近的 Cast 设备被发现。Google Play 服务可以发现连接到网络的 Cast 设备，但直到现在，你都无法关闭它。

我们将继续挖掘这个版本的更多特性。