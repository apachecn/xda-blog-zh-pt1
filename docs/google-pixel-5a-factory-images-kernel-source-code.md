# 谷歌 Pixel 5a 工厂图片和内核源代码现已可用

> 原文：<https://www.xda-developers.com/google-pixel-5a-factory-images-kernel-source-code/>

上周，谷歌终于揭开了 Pixel 5a 的神秘面纱，但山景城巨人有点松懈，在发布后没有给我们在线旅行社和工厂图片的直接下载链接。如果你已经[设法为自己争取到一个](https://www.xda-developers.com/best-google-pixel-5a-deals/)，我们有好消息告诉你，因为谷歌现在已经发布了该设备的初始工厂图像集，可以用来在你的新玩具上恢复 Android 11 的股票形式。除了股票固件，谷歌还上传了所有的工具，文件和第三方开发人员运行定制软件所需的文档。

**[谷歌 Pixel 5a XDA 论坛](https://forum.xda-developers.com/f/google-pixel-5a.12359/)**

### 工厂图像

如果你想回到 Pixel 5a(代号:“barbet”)上的股票软件，你可以从下面的链接中提取并刷新最新的工厂映像固件。还可以从索引中获取完整的 OTA zip，并使用 ADB 通过恢复环境加载它。初始版本的版本号为 RD2A.210605.x，对应于 2021 年 6 月的 Android 安全补丁级别。有两套工厂图像可用:一套用于日本承运人单位(次要版本号 006)，另一套用于解锁单位(次要版本号 007)。

**[工厂画面](https://developers.google.com/android/images#barbet)| |[全 OTA 画面](https://developers.google.com/android/ota#barbet)**

### Android 12 呢？

谷歌 Pixel 系列的一个隐含承诺是，设备所有者将会收到更新，而且会很快收到。话虽如此，Pixel 5a 仍然无法报名参加 [Android 12](https://www.xda-developers.com/android-12/) beta 计划。目前，你可以解锁引导程序，然后[刷新一个官方的 GSI 版本](https://www.xda-developers.com/how-to-download-android-12/)来体验一下 Android 12。

### 内核源代码，设备树

内核源代码和设备树源代码现已上线，因此开发人员很快就可以开始为设备构建 TWRP 和定制内核。如果你想为自己建立一个全新的系统映像，或者想为基于 AOSP 的定制 rom 启动移植工作，你不需要等待太久，因为谷歌已经发布了 Pixel 5a 的驱动程序二进制文件。

**[内核源代码](https://android.googlesource.com/device/google/barbet-kernel/) || [设备树](https://android.googlesource.com/device/google/barbet/) || [策略](https://android.googlesource.com/device/google/barbet-sepolicy/)**