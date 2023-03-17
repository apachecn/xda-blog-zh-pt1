# Android 12 准备为 Pixel 5 带来双击返回手势

> 原文：<https://www.xda-developers.com/android-12-prepares-double-tap-back-gesture-pixel-5/>

第一个 [Android 12](https://www.xda-developers.com/android-12/) 开发者预览版正式发布，和往常一样，谷歌自己的 [Pixel 手机是第一批体验最新味道的](https://www.xda-developers.com/how-to-install-android-12/)。在我们的[实践文章](https://www.xda-developers.com/android-12-developer-preview-hands-on/)中，我们已经讨论了一些主要变化。但是似乎还有很多事情有待发现。在我们的雷达下飞行的事物之一是双击手势。在真正的谷歌时尚中，这项功能最初是在 Android 11 开发者预览版 1 中推出的，但从未成为最终版本。

随着 Android 12 的推出，谷歌再次(通过[*9 to 5 谷歌*](https://9to5google.com/2021/02/18/android-12-dp1-pixel-double-tap-gesture-assistant-columbus/) )将双击手势带了回来，这一次，它也有了面向用户的设置。如果你有一个运行最新预览版的 Pixel 5，你可以在设置>系统>手势下找到新功能。双击手势允许用户在手机背面点击来执行/触发一系列动作。这些手势不需要任何特殊的硬件。他们依靠手机的加速度计和陀螺仪来确定用户的点击。

目前，双击手势提供了五个选项供您选择:

*   打开助手
*   截图
*   播放和暂停媒体
*   查看最近的应用
*   打开通知

*截图来自 Reddit 用户[Kris haks 301029](https://www.reddit.com/user/krishaks301029)*

您也可以通过一个简单的开关来调整敲击灵敏度。但不幸的是，这个特性在目前的实现中似乎并不奏效，因为它可能仍然很粗糙。此外，根据用户报告，目前该功能似乎只在 Pixel 5 上可见，因为这一选项不会在 Pixel 4、Pixel 4Xl、Pixel 4a 和 Pixel 3XL 等其他谷歌设备上显示。然而，代码分析证实，有适用于 Pixel 3 XL、Pixel 4 和 Pixel 4a 5G 的 TensorFlow Lite 型号，该功能只需要加速度计和陀螺仪等基本传感器即可工作。

虽然，在目前的状态下，谷歌是否会在 Android 12 的最终版本中完全实现双击功能，或者他们是否会再次放弃它，还有待观察。目前还不清楚这项功能是 Pixel 5 推出时独有的，还是其他 Pixel 手机也可以正式使用。