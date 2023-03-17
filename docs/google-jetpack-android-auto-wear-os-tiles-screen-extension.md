# Google 为 Android Auto 发布了一个 Jetpack 库，准备了两个新的 API

> 原文：<https://www.xda-developers.com/google-jetpack-android-auto-wear-os-tiles-screen-extension/>

鉴于谷歌每年的操作系统发布周期和 Google Play 不断变化的 API 要求，为 Android 开发可能是一件艰巨的事情，但这就是为什么谷歌在[“Android Jetpack”](https://www.xda-developers.com/android-jetpack-components-kotlin-android-studio-3-2/)保护伞下维护一组支持库。除了兼容性库之外，Jetpack 中还包括其他用于应用程序开发的库，最新的是 Android for Cars 应用程序库。由于 Jetpack 库是开源的，我们还发现一个新的 API 正在开发中:这将使为可折叠和双屏设备开发创新应用变得更容易。

## Android for Cars 应用程序 Jetpack 库

早在 2020 年 10 月，谷歌[发布了](https://www.xda-developers.com/google-releases-android-for-cars-app-library-developers-create-apps-android-auto/)测试版 Android for Cars 应用程序库，允许第三方应用程序开发者在 Android Auto 平台上设计、开发和测试他们自己的导航、停车和充电应用程序。2020 年 12 月，谷歌[开始允许](https://android-developers.googleblog.com/2020/12/opening-google-play-store-for-more-car.html)发布基于该库的安卓汽车应用。广受欢迎的第三方地图和导航应用软件 Sygic 是最先利用这一点的公司之一，[在 12 月中旬发布了该应用软件的安卓自动兼容版本](https://www.xda-developers.com/sygic-available-android-auto-alternative-google-maps-waze/)。2021 年 1 月下旬，谷歌允许用这个库构建的应用程序在开放测试轨道上发布，[宣布](https://android-developers.googleblog.com/2021/01/expanding-reach-of-your-android-auto.html)他们正在努力将 Android for Cars 应用程序库迁移到 Android Jetpack。

[](https://1.bp.blogspot.com/-MLpA7kPaK4I/YDk5t4cv-PI/AAAAAAAAQK0/m_pIhXTAbgQWSwYODMpM0qdm8fYPU1nGgCLcBGAsYHQ/s0/Screen%2BShot%2B2021-02-26%2Bat%2B1.06.08%2BPM.png)

[](https://1.bp.blogspot.com/-MLpA7kPaK4I/YDk5t4cv-PI/AAAAAAAAQK0/m_pIhXTAbgQWSwYODMpM0qdm8fYPU1nGgCLcBGAsYHQ/s0/Screen%2BShot%2B2021-02-26%2Bat%2B1.06.08%2BPM.png)

*T2`androidx.car.app`中新 GridTemplate 的例子*

今天，谷歌[宣布](https://android-developers.googleblog.com/2021/03/android-auto-apps-powered-by-jetpack.html)Android for Cars 应用程序库在 Jetpack 中作为[androidx . car . App](https://developer.android.com/jetpack/androidx/releases/car-app)1 . 0 . 0-beta 01 提供。这是之前关闭的源代码库的第一个版本，可以在安装了 Android Auto 6.1 或更高版本的设备[上运行。它包括旧库的所有功能，但也增加了一些特性，比如新的](https://www.xda-developers.com/android-auto-wallpaper-assistant-shortcut/) [GridTemplate](https://developer.android.com/reference/androidx/car/app/model/GridTemplate) 。谷歌还更新了[开发者指南](https://developer.android.com/training/cars/navigation)和[设计指南](https://developers.android.com/training/cars/Android%20for%20Cars%20Jetpack%20Library%20design%20guidelines.pdf)以涵盖新库，并计划在 2021 年 9 月 1 日之前弃用旧库。谷歌表示，将你的 Android Auto 应用从现有库迁移到新的 Jetpack 库[很容易](https://developers.android.com/training/cars/jetpack-migration)——改变名称空间并调整一些 API 调用。有了这一改变，我们现在离 Play Store 中出现的第三方 Android 汽车应用更近了一步。

## 屏幕扩展 API

可折叠和双屏设备是这个街区最酷的孩子，但他们还没有太多的粉丝。官方 Android 模拟器支持有趣的形式，如可折叠，双屏手机和可滚动。然而，开发人员仍然需要想办法扩展他们的应用程序的内容，并使用平台 API 来实现这一点。为了让开发者更容易完成这个过程，谷歌正在开发一个新的屏幕扩展 API。根据 [one commit](https://android-review.googlesource.com/c/platform/frameworks/support/+/1540814) 的说法，谷歌已经制作了演示，展示开发者如何使用屏幕扩展 API 来创建一个扩展到辅助显示器的游戏控制器和一个在另一个屏幕上显示预览的相机应用。该 API 目前在[被标记为实验性的](https://android-review.googlesource.com/c/platform/frameworks/support/+/1541347)，直到 [OEM 接口](https://android-review.googlesource.com/c/platform/frameworks/support/+/1579244)最终确定。我们很想知道一旦这个 API 被合并，开发者会开发出什么样的应用。

* * *

根据 AOSP 的其他消息，谷歌正在开发表情符号 Jetpack 库的[新版本](https://android-review.googlesource.com/c/platform/frameworks/support/+/1594993)，他们正在[继续工作](https://android-review.googlesource.com/c/platform/frameworks/support/+/1584923)以将[官方 Tiles API 引入操作系统应用开发](https://www.xda-developers.com/google-finally-preparing-tiles-api-release-wear-os-smartwatches/)。