# Android 12 可以引入类似可达性的“单手模式”

> 原文：<https://www.xda-developers.com/android-12-one-handed-mode-leak/>

多年来，智能手机制造商制造了越来越高的设备。虽然这让手机上的媒体消费变得更加愉快，但也导致许多手机无法单手使用。为了弥补这一点，一些手机制造商开发了软件解决方案来提高单手使用的便利性:最著名的是苹果公司的可达性功能。现在，谷歌将在 Android 12 中推出自己的单手模式版本。

XDA 现在了解到，谷歌正在开发一个单手模式功能，并将其纳入安卓的开源版本 AOSP。这意味着任何使用 AOSP 的智能手机制造商都可以使用该功能。更重要的是，这意味着尚未开发自己的单手模式功能的原始设备制造商将能够利用谷歌版本的软件。然而，我们不知道谷歌是否计划在所有 Android 12 设备上强制包含其单手模式版本。

虽然我们不确定 Android 12 的单手模式将如何设计，但我们认为它会像许多 OEM 实现一样，将整个屏幕缩小到一个角落(例如，像特色图片中显示的华硕实现)。我们确实知道谷歌目前在 Android 12 中的实现包括将屏幕尺寸缩小到其最大尺寸的 40%。我们还知道，将有一种方法来触发单手模式，使用传统的 3 按钮模式以及更新的手势导航模式。目前，计划将单手模式添加到设置>系统>手势>单手，这是有意义的，因为它是使用手势触发的(可能是在导航栏上向左/向右滑动)。

在 Android 12 中增加单手模式之前，许多原始设备制造商已经开发了自己的版本。一度，中国智能手机制造商华为甚至试图向 AOSP 提交其版本的功能，但谷歌拒绝了它的加入。给出的原因是华为的实现与其他功能冲突，并引入了错误，尽管任何问题都可以得到解决。尽管如此，谷歌花时间实现其合作伙伴的 Android 设备中已经存在的关键功能并不罕见。

例如，谷歌也终于在 Android 12 中引入了滚动屏幕截图功能，这是原始设备制造商实现多年后的事情。在去年 Reddit 上的一个“问我任何事情”帖子中，[谷歌表示](https://www.xda-developers.com/android-11-ama-summary/)它不想以一种不成熟的方式实现滚动截图；该公司指出，一些 OEM 实现如何在某些页面上无法工作，或者在滚动某些视图时无法拼接图像。同样，谷歌可能会在单手模式下投入类似程度的努力。除了缩小和重新定位所有系统 UI 元素，谷歌还必须考虑单手模式如何影响第三方应用程序，因为它的实施将影响整个 Android 生态系统，而不仅仅是设备的子集。

由于我们没有 Android 12 单手模式的图片，很遗憾我们不能准确展示它会是什么样子。然而，我们预计第一个 Android 12 开发者预览版将在本月晚些时候登陆，所以我们可能不用等很久就能看到该功能的运行。然而，我们不知道谷歌是否会在开发者预览版中包含该功能，甚至在未来的测试版或稳定版中也不会包含该功能。如果谷歌决定该功能仍未准备好发布，那么我们可能要到明年的 Android 版本才能看到该功能。

*特色图片:华硕在一台运行 Android 11 的 ZenFone 7 Pro 上的单手模式*

*本文更新于美国东部时间 2021 年 2 月 17 日晚 7 点 56 分，提及华为单手模式实现为何被拒绝。*