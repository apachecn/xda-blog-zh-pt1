# Android 12 Beta 4 推出了最终确定的 API 和行为

> 原文：<https://www.xda-developers.com/android-12-beta-4/>

Android 12 的第四个测试版今天上线，它标志着平台稳定性的里程碑。这意味着 Android 12 Beta 4 已经[完成了 API](https://developer.android.com/preview/features)和[面向应用的行为](https://developer.android.com/preview/behavior-changes-all)，因此开发者可以在最新版本上测试他们的应用，而不必担心下一个测试版的变化会影响兼容性测试。

随着 Beta 4 的发布，谷歌要求所有应用程序和游戏开发商开始他们的最终兼容性测试，并在最终版本发布前尽快发布兼容性更新(可能在下个月)。)这对于 SDK、库、工具和游戏引擎的维护者来说尤其重要，因为下游的应用和游戏开发者可能无法更新他们自己的产品，直到他们的依赖关系也被更新。当你发布了你的应用程序的兼容版本后，你也可以开始[将你的应用程序的 targetSdkVersion](https://developer.android.com/distribute/best-practices/develop/target-sdk) 更新到 31，这与 Android 12 一致。

谷歌表示，在未来几周内将会有更多的测试版发布，并且它将会是发布候选版本。然而，随着 Android 12 Beta 4 标志着平台稳定性的里程碑，开发者不再有任何理由等待他们的应用程序适应最新版本。

Android 12 Beta 4 今天可用于所有兼容的 Pixel 设备，包括 Pixel 3 和更高版本。注册了 Android beta 计划的用户将通过无线方式接收更新，不过与往常一样，固件下载链接将在谷歌网站上提供。第四个测试版也将面向拥有华硕、一加、Oppo、Realme、夏普或中兴兼容设备的开发者。这些设备包括华硕 ZenFone 8、一加 9 系列、OPPO Find X3 Pro、Realme GT、夏普 AQUOS sense5G 和中兴 Axon 30 Ultra 5G。

如果您正在寻找最新 Android 12 测试版的下载链接和安装指南，我们可以满足您的需求。[访问本页面](https://www.xda-developers.com/how-to-download-android-12/)获取我们最新的 Android 12 测试版下载库，然后[访问本指南](https://www.xda-developers.com/how-to-install-android-12/)获取安装测试版的操作指南。安装后，检查以确保您的构建与下面列出的信息相匹配。

**安卓 12 Beta 4**

**上映日期**:2021 年 8 月 11 日

**版本** : SPB4.210715.011

**仿真器支持** : x86 (64 位)、ARM (v8-A)

安全补丁级别:2021 年 8 月

**Google Play 服务** : 21.24.18

根据[发布说明](https://www.xda-developers.com/google-play-services-delete-ad-id-opt-out-personalization/)，Beta 4 引入了用一串零替换广告 ID 的功能，正如之前宣布的那样。这项功能将在 Google Play 服务版本 21.30.13 和更高版本中推出，用于运行 Beta 4 的设备，并将在 2022 年初扩展到其他设备。发行说明还提到以下错误已得到修复:

### Android 12 Beta 4 中修复的 bug

### 开发者报告的问题

*   修正了阻止一些未接来电通知被取消的问题。([第 193718971 号](https://issuetracker.google.com/issues/193718971)，[第 194388100 号](https://issuetracker.google.com/issues/194388100))
*   修正了系统主题颜色不适用于快速设置的问题。([期号 190633032](https://issuetracker.google.com/issues/190633032) ，[期号 190338020](https://issuetracker.google.com/issues/190338020) )
*   修正了一个问题，当拖动或重新排列快速设置块时，它们没有与栅格对齐。([问题编号 188641280](https://issuetracker.google.com/issues/188641280)
*   修正了警报和静音图标不显示在通知栏的问题。([问题编号 186769656](https://issuetracker.google.com/issues/186769656)
*   修正了当从另一个页面滑动回主屏幕时，主屏幕是空白的问题。([问题编号 189435745](https://issuetracker.google.com/issues/189435745)
*   修正了一个问题，当蓝牙设备连接后，在通话中将音频路由到手机后听不到音频。([问题编号 192585637](https://issuetracker.google.com/issues/192585637)
*   修正了日历控件添加到主屏幕后无法加载的问题。([问题编号 188799206](https://issuetracker.google.com/issues/188799206)
*   修正了设置程序中某些选项的切换不可见的问题。([发行号 193727765](https://issuetracker.google.com/issues/193727765)
*   修正了一个小工具有时会在重启设备后消失的问题。([问题编号 191363476](https://issuetracker.google.com/issues/191363476)
*   修正了当 VPN 激活时 RCS 消息不工作的问题。([问题编号 189577131](https://issuetracker.google.com/issues/189577131)
*   修复了有时会导致设备崩溃和重启的问题。([问题#194272305](https://issuetracker.google.com/issues/194272305)
*   修复了导致前台服务启动限制显示多个通知的问题。([问题编号 194081560](https://issuetracker.google.com/issues/194081560)
*   修正了从 dock 或主屏幕区域打开应用程序时，有时会打开错误的应用程序的问题。([发行号 194766697](https://issuetracker.google.com/issues/194766697)
*   修正了在某些情况下双击设备屏幕不会唤醒它的问题。([问题编号 190453834](https://issuetracker.google.com/issues/190453834)
*   修正了手机信号强度不显示在状态栏的问题。([问题编号 190894572](https://issuetracker.google.com/issues/190894572)
*   修正了一个问题，如果一个屏幕记录器是活跃的，通知阴影没有动画关闭时正常。([发行号 191276597](https://issuetracker.google.com/issues/191276597)

### 其他已解决的问题

*   修复了一个问题，当在 Android Auto 上播放 Youtube 上的音乐时，一些用户体验到从手机而不是汽车扬声器播放音频，或者在丰田汽车上根本没有音频。
*   修正了在 Android Auto 上使用谷歌地图导航时，一些用户遇到文本模糊的问题。
*   修正了用户在使用 Android Auto 时无法在 Waze 中选择目的地的问题。
*   修复了启动 Android Auto 后手机无响应或卡在锁屏的问题。
*   修复了一个问题，在某些情况下，谷歌地图不能提供不同的路线选项，而使用 Android Auto。
*   修正了 Android Auto 手机锁定时音乐会暂停的问题。
*   修正了 Android Auto 上的一个问题，用户在尝试使用谷歌助手回复短信时有时会听到音乐音频。
*   修正了 Android Auto 的自动昼夜切换不工作的问题。

谷歌已经[意识到 Beta 4 中的几个问题](https://developer.android.com/about/versions/12/release-notes#ki-beta4)，但是如果你遇到了[还没有提交的 bug](https://issuetracker.google.com/savedsearches/5938602)，你应该通过 Android Beta Feedback 应用向谷歌提交反馈。

最后，谷歌还在为 Android TV 提供新的 Android 12 测试版。但是，该版本仅适用于 ADT-3 开发工具包。谷歌还没有详细说明 Beta 4 中对 Android 电视平台做了哪些改变，但很可能他们会像 Beta 3 发布后一样，很快发布一篇独立的博客文章。