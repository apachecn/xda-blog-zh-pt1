# Android 12 中的应用休眠可以释放未使用应用的空间

> 原文：<https://www.xda-developers.com/app-hibernation-android-12-beta/>

# Android 12 增加了应用休眠，以释放未使用应用的空间

有很多你实际上不使用的应用程序吗？Android 12 正在添加一个应用程序休眠功能，以防止他们浪费空间。

谷歌的 [I/O 2021](https://www.xda-developers.com/tag/google-io-2021/) 主要主题演讲于昨天结束，我们了解了几个关于 Android 和 Android 生态系统本身的令人兴奋的消息。我们第一次看到了 [Android 12](https://www.xda-developers.com/android-12/) 及其全新的 [Material You](https://www.xda-developers.com/material-you/) 设计语言，这是几年来 Android 最大的 UI 改进之一。谷歌新用户界面指南背后的主要理念是可定制性，让你的手机真正成为你自己的——在某种程度上，这也包含了 Android 背后的理念。但是 Android 12 不仅仅是一张漂亮的脸。从 Android 12 开始，一些用户可见和隐藏的功能将进入该平台。其中之一就是 app 休眠。

今天宣布了应用程序休眠[和其他隐私功能，这是](https://android-developers.googleblog.com/2021/05/android-security-and-privacy-recap.html)[之前在 AOSP 代码更改中发现](https://www.xda-developers.com/android-12-hibernate-apps/)的一个功能，我们甚至在之前的 Android 12 版本中[自己打开了这个功能](https://www.xda-developers.com/android-12-hibernate-unused-apps/)。但出于上下文的考虑，应用程序休眠允许你将应用程序置于“休眠”状态，如果它们没有被主动使用的话。进入休眠状态的应用程序将优化其存储使用，其权限将被撤销。几个月不使用的应用程序将进入这种“休眠”状态，尽管用户可以快速打开和关闭这一功能，如果他们不想让他们不使用的应用程序进入休眠状态。要让一个应用程序从休眠中醒来，你只需要像平常一样打开它。

虽然谷歌表示，该功能现在可以在 Android 12 Beta 1 中使用，但你必须等待数月才能让应用程序真正进入休眠状态，或者使用 shell 命令手动将应用程序置于你设备中的休眠模式。我们使用 shell 命令将 Speedtest 应用程序置于休眠状态，并获得上面显示的屏幕截图。然而，如果你想自己尝试一下，你需要测试的命令在 [Android 开发者网站](https://developer.android.com/about/versions/12/behavior-changes-12#app-hibernation)的应用休眠部分有所提及。