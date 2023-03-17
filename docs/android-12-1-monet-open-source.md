# Android 12 的壁纸主题系统将在 Android 12.1 中开源

> 原文：<https://www.xda-developers.com/android-12-1-monet-open-source/>

我们距离 Android 12 的发布只有几周的时间了，但重要的是要记住，传言中的 10 月 4 日[发布日期](https://www.xda-developers.com/android-12-stable-release-date-rumor/)只针对谷歌自己的 Pixel 手机。这需要几周，或者更可能是几个月的时间，更新才能到达其他设备，当它到达时，它不会包括每一个新功能。Android 12 开源版本中最值得注意的功能是谷歌基于壁纸的主题引擎，代号为“monet”，因此不会出现在该操作系统的许多 OEM 版本中。然而，它被开源 Android 排除在外似乎只是暂时的，因为有证据表明，随着 Android 12.1 的发布，“monet”将完全开源。

对于那些没有看过或试用过 Android 12 测试版的人来说，你可能不知道谷歌正在进行的重大 UI 更改。Android 12 将引入自 2014 年 Android 5.0 Lollipop 发布以来最重要的 UI 更新，当时谷歌首次推出了 Material Design，这是该公司为其设计语言打造的品牌。谷歌的设计语言多年来一直在发展，为了反映最新版本对个性化的强调，谷歌将其更名为“ [Material You](https://www.xda-developers.com/material-you/) ”

Material You 的一个关键特性是前面提到的“monet”主题系统，它会根据用户的壁纸自动为系统[生成调色板。根据谷歌的说法，颜色提取引擎采用带有材料颜色目标的聚类算法来确定用户壁纸的主色和次主色。然后，调色板生成算法会创建一个丰富的调色板，包含 5 种颜色(2 种中性色和 3 种强调色)以及 12 种材质颜色，用于确定最接近用户壁纸的色调。这些颜色值保存在一个索引中，应用程序可以通过 API 调用该索引，从而允许它们对自己的 UI 进行主题化。](https://www.xda-developers.com/android-12-wallpaper-theme/)

当谷歌在今年早些时候的 I/O 开发者大会上首次推出其“monet”主题系统时，该公司表示，它将于今年秋天在 T2 首次推出谷歌 Pixel 手机。然而，目前还不清楚谷歌是否只是声称“莫奈”的首次推出独占，或者该功能是否将完全专属于运行 Android 12 的 Pixel 手机。换句话说，我们不知道三星、小米、OPPO 或一加等设备制造商是否可以在自己的操作系统中使用“monet”。

除非谷歌强制要求(这种情况很少见)，否则设备制造商通常可以自由选择是否要实施谷歌的 UI 更改。在“monet”的情况下，设备制造商将不得不重新实现系统的一部分，因为并非所有方面都是开源的。据[开源其类似于谷歌“莫奈”的动态调色板生成器](https://www.xda-developers.com/android-12-material-you-theming-system-recreated/)的开发者 [kdrag0n](https://twitter.com/kdrag0n) 称，核心颜色提取和[色貌模型(CAM)](https://cs.android.com/androidx/platform/frameworks/support/+/androidx-main:core/core/src/main/java/androidx/core/content/res/CamColor.java;l=26;bpv=0) 都已经开源，而用于提取颜色的后处理/过滤的 AOSP 算法据报道“非常接近”谷歌的专有解决方案。剩下要开源的主要是调色板生成算法，这是主题化过程的关键部分。

幸运的是，谷歌似乎准备发布这种算法的源代码。两个消息来源证实，谷歌最近进行了一项名为“将莫奈加入 AOSP”的代码更改这个补丁最初只在安卓 13“提拉米苏”的 [AOSP 内部分支可用，但最近被精选到安卓 12-sv2 内部分支。](https://www.xda-developers.com/google-android-13-t-tiramisu-dessert-name/)

Android 12-sv2 将是一个伴随着 API 级别提升的点更新，所以我们暂时[称之为 Android 12.1](https://www.xda-developers.com/android-12-v2-update/) 。除了[的新壁纸](https://www.xda-developers.com/android-12-1-wallpaper/)，更新还将为可折叠手机体验带来一些[的小改进，包括任务栏功能。当然，这显然是第一个包含“莫奈”源代码的版本](https://www.xda-developers.com/android-12-1-foldable-phone-enhancements-pixel-fold/)

下面的截图来自一台运行 Android 12.1 内部 AOSP 版本的设备，显示“monet”已经在开源版本中实现。

我们还不知道谷歌计划何时向公众发布 Android 12.1，所以我们不知道 OEM 厂商多久才能完全访问谷歌的新主题化系统。我们已经可以看到[三星的 Android 12 beta](https://www.xda-developers.com/one-ui-4-beta-features-overview/) 完全跳过了实现材料 You，并且在 OPPO 的 ColorOS 12 公告中没有提到更新的设计或基于壁纸的主题[。如果任何一家公司——或任何其他原始设备制造商——希望其用户在 Android 12 上享受基于壁纸的主题化，他们将不得不自行实现或反向移植该功能。这当然是可行的，因为许多必要的代码已经包含在 Android 12 尚未公开的源代码中，其余的则包含在 Android 12.1 中，但这不是我们可以想象的*每个* OEM 厂商都会做的事情。](https://www.xda-developers.com/coloros-12-unveiled/)

*感谢开发者 [kdrag0n](https://twitter.com/kdrag0n) 对本文的投入！*