# Android Automotive 是为汽车设计的，但这位开发者将其移植到了平板电脑上

> 原文：<https://www.xda-developers.com/android-automotive-ported-samsung-tablet/>

Android Automotive 是 Android 的一个特殊分支，旨在作为车载信息娱乐(IVI)系统的主要操作系统运行。相比之下，Android Auto 是一款在手机上运行的应用程序，它将驾驶优化的用户界面投射到汽车的内置仪表盘上。Android Automotive 和 Android Auto 都允许你运行谷歌地图等应用程序的驾驶优化版本，但 Android Automotive 与汽车传感器的集成要紧密得多，并允许你控制 AC 等车辆特定功能。

Android Studio 为开发人员提供了一个 [Android 汽车仿真器映像](https://www.xda-developers.com/google-releases-updated-android-automotive-emulator-image-with-play-store/)来测试他们的应用，但是也可以手动编译系统映像。这是因为 Android Automotive 是[开源](https://source.android.com/devices/automotive/start/what_automotive)和[在 AOSP](https://android.googlesource.com/device/generic/car/) 可用，所以可以构建它的通用系统映像。

Reddit 用户 [tompratt](https://www.reddit.com/user/tompratt) 就是这么做的。用户在/r/linegeos subreddit 上发布了一个帖子[，展示了他将 Android Automotive 引导到 Galaxy Tab S5e 上的工作。根据他的说法，它“在[他的]车上工作很好，这要归功于内置的 4G、GPS、麦克风、扬声器等。”Android Automotive builds 没有公开可用的 Google Apps 包(](https://www.reddit.com/r/LineageOS/comments/o9rggi/android_automotive_on_lineageos/) [Google Automotive Services](https://source.android.com/devices/automotive/start/what_automotive#google-automotive-services-gas) ，或 GAS，被授权给汽车 OEM 厂商)，因此开发者改为下载 Aurora Store 以下载应用程序，如 TomTom Amigo 导航应用程序，如他分享的图片所示。市场上只有为数不多的几款车内置了 Android Automotive，因此很难(但有可能)获得其他谷歌汽车应用。

*图片由 tompratt 提供*

当然，在平板电脑上闪现 Android Automotive 肯定是小众的，但 DIY 汽车改装者可能会发现这个组合提供了比汽车默认主机更好的车内体验(如果它甚至有一个的话！)可悲的是，安装 Android Automotive 不会让你控制像汽车空调这样的功能，但你至少可以获得 AAOS 的其余体验。

目前，tompratt 展示的版本还不能下载，但开发者表示他有兴趣与 LineageOS 团队合作发布官方汽车版本。他说，到目前为止，他已经基于 LineageOS 17.1 和 18.1(意思是 Android 10 和 Android 11)构建了 Android Automotive builds，我们期待着看到这项工作成为现实。

这篇文章在美国东部时间下午 2:22 更新，开发者对此进行了澄清。