# Android Studio 北极狐为可滚动手机添加了一个模拟器

> 原文：<https://www.xda-developers.com/android-studio-emulator-rollable-phones/>

# Android Studio 北极狐为可滚动手机添加了一个模拟器

Android Studio 最新的 Canary build 包括一个用于可滚动设备的模拟器，让你可以看到应用程序在滚动和展开时的行为。

金丝雀频道的最新版本 Android Studio 增加了一个反映设备设计方向的新功能:可滚动手机的仿真器。该模拟器目前在 Android Studio 的北极狐 Canary 1 版本中可用，它创建了一个 7.4 英寸的虚拟手机，运行 Android 11，折叠时显示 1600 x 2428 的显示屏，允许开发人员测试他们的软件在滚动或展开时的行为，这是一个比标准显示屏更具挑战性的优化屏幕。

正如 *Engadget China* 的 [Richard Lai](https://twitter.com/i/status/1334068020675715072) 在 Twitter 上指出的，新的 AVD target 允许你看到页面布局在展开模式、过渡期间以及最终在滚动模式下的反应，以确保没有代码异常导致它看起来，因为缺少一个更好的词，“错误”。因为随着显示屏的展开，应用程序需要适应一系列递增的屏幕尺寸，所以开发人员将面临一些挑战，以调整他们的应用程序布局来适应这种新的外形。

可折叠床看起来将成为 2021 年的新玩意儿之一。OPPO 已经展示了自己的概念验证设备，其他 OEM 厂商，包括三星、LG 和 TCL，都在为商业发布开发自己的手机。也就是说，我们可能还需要一段时间才能在 Android Studio 上看到稳定版本的可滚动模拟器。当前的[版本 4.1](https://www.xda-developers.com/google-releases-android-studio-4-1/) 于 10 月发布，虽然它可能会从金丝雀到测试版再到稳定版并在春季发布，但它可能要到明年秋天成为 Android Studio 4.3 时才会准备好。不过，请注意，[谷歌刚刚改变了 Android Studio 及其 Gradle 插件的版本号](https://android-developers.googleblog.com/2020/12/announcing-android-studio-arctic-fox.html)，以使其与 IntelliJ 版本保持一致，因此昨天的金丝雀版本带有“Android Studio 北极狐(2020.3.1)”的名称。