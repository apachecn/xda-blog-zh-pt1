# 谷歌正在为 Android 12 的设置测试一个新的 x 轴过渡动画

> 原文：<https://www.xda-developers.com/google-android-12-x-axis-transition-animation/>

# 谷歌正在为 Android 12 的设置测试一个新的 x 轴过渡动画

谷歌正在最新的 Android 12 Beta 2 版本中测试来自 Material Design 的运动系统的新 x 轴过渡动画。

谷歌今天早些时候发布了第二个 [Android 12](https://www.xda-developers.com/android-12/) 测试版，新版本带来了谷歌在上个月的 I/O 开发者大会上宣布的[大量隐私功能](https://www.xda-developers.com/android-12-beta-2/)。和往常一样，这个版本中也有许多未记录的变化，如果你有兴趣了解它们，我有一个正在运行的 tweet 线程，我会不断添加。

当我在写一个总结我们发现的所有变化的帖子时(有很多要看！)，我想强调一下我在 Android 12 Beta 2 中发现的一些隐藏的变化。在分析 APK 的设置时，我发现谷歌在一个功能标志后面设置了一个新的页面转换动画。此标志一旦启用，会将过渡动画更改为使用共享的 x 轴动画，详见[谷歌的材料设计指南](https://material.io/design/motion/the-motion-system.html#shared-axis)。此动画目前仅适用于设置应用程序，不适用于设备上安装的任何其他系统或第三方应用程序。

Android 12 Beta 2 中正常设置页面过渡动画:

Android 12 Beta 2 中新增共享 x 轴设置页面过渡动画:

[video width = " 303 " height = " 624 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/06/Android-12-Beta-2-X-Motion-animation . MP4 "]

看到这个动画现在被测试很奇怪，因为它不是新的，也不是你们宣布的材料的主要焦点，但我很喜欢 x 轴过渡，并希望它一直存在。正如我提到的，这个动画目前被关在一个旗帜后面，因此在 Android 12 Beta 2 中默认情况下是不启用的。我们不知道这种共享的 x 轴过渡动画是否会在未来的测试版中成为 Settings 应用程序的默认设置，但测试版已经不多了，所以我们不用等太久就能找到答案(在今年晚些时候稳定版发布之前，只剩下 2 个测试版)。