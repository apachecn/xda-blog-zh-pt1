# Android 12 DP2 新特性:更浅的黑暗主题，单手模式

> 原文：<https://www.xda-developers.com/android-12-dp2-new-features/>

谷歌在该软件于今年秋天广泛发布之前发布了 Android 12 开发者预览版 2。虽然我们已经给出了最新开发者预览版中正式包含的内容的[概述](https://www.xda-developers.com/android-12-dp2-hidden-features/)，但我们现在要更仔细地看看这个版本，并涵盖谷歌没有宣布的其他几个功能。

## 新黑暗主题

谷歌在 Android 10 中首次推出了全系统黑暗主题，为像素所有者提供了真正的黑色外观。第一个 Android 12 开发者预览版为黑暗主题引入了深灰色调，在开发者预览版 2 中，谷歌[将其变成了更浅的灰色调](https://twitter.com/MishaalRahman/status/1372237092277870599)。

当把不同的主题放在一起看时，对比是鲜明的。然而，灰色深色主题仍然应该为用户提供一个看起来很舒服的外观，并且仍然可以节省一些电池寿命。

## 单手模式

随着设备变得越来越大，单手使用变得越来越困难。谷歌正在 Android 12 中用单手模式解决这个问题，这将使单手使用更加容易。

在 Pixel 的手势设置菜单中，有一个[单手模式选项](https://www.xda-developers.com/android-12-is-adding-a-native-one-handed-mode/)，它将向下移动屏幕，这样你可以更容易地到达顶部；类似于苹果在 iOS 中的可达性功能。一旦启用，你可以通过向下滑动导航条附近的显示屏底部来触发单手模式。

该功能提供了一个开关，可以在切换应用程序时退出单手模式，还有四个不同的超时选项:从不，4 秒，8 秒和 12 秒。

## 新的通知向下滑动手势

在第一个 Android 12 开发者预览版中，我们[发现了一个叫做“滑动通知”的新手势](https://www.xda-developers.com/android-12-new-swipe-down-gesture-notification-shade-from-any-screen/)此手势允许您在屏幕底部附近向下滑动，以下拉通知栏。许多启动器应用程序——包括谷歌自己的 Pixel Launcher——让你在主屏幕的任何地方向下滑动，拉下通知阴影。然而，当在设置>系统>手势>滑动通知中启用该手势时，您可以在任何屏幕上拉下通知阴影。

因为推送通知手势的触发方式与单手模式的触发方式相同，所以它们彼此不兼容。当您启用其中一个时，另一个将被禁用。此外，如果你有一部后置指纹扫描仪的 Pixel 手机，这个手势似乎不会起作用，因为谷歌希望你使用现有的“刷指纹通知”手势来完成同样的事情。

我们在 Android 12 DP2 中发现的第一个变化是 Pixel Launcher 中的一个新的小部件选择器。就像以前一样，长按主屏幕，您可以轻松地选择您选择的小工具。不过，新的外观更加简洁，为了更容易滚动，它将不同的选项折叠起来。

## 从特定通知监听器“取消桥接”应用程序

在 Android 12 开发者预览版 2 中，你现在可以选择从通知监听器“解绑”应用。这是令人困惑的措辞，但我们认为这意味着您将能够挑选通知侦听器服务可以拦截的应用程序。对于那些不知道的人来说，通知监听器是一种可以在你发布通知时读取通知的服务，例如，Wear OS 应用程序就是这样读取你的通知并将其同步到你的智能手表上的。

## 智能转移呼叫

Android 12 开发者预览版 2 增加了智能转发功能，这是我们很久以前在 AOSP 发现的[。该功能允许您在设备上提供的两个 sim 卡之间转移呼叫。当一个 SIM 卡不可达而另一个不可达时，该功能可能会派上用场。](https://www.xda-developers.com/android-version-support-smart-forwarding-forward-calls-between-sims/)

## 将屏幕调暗设置

正如我们之前解释的，Android 12 正在[增加一个“减少亮色”](https://www.xda-developers.com/android-12-smart-autorotate-game-mode-reduced-brightness/)(现在在 DP2 中称为“降低亮度”)功能。现在在 DP2 中，这个功能，以及其他与对比度、大小和主题相关的偏好，已经合并到一个新的“将屏幕调暗”设置页面中。您可以在设置>辅助功能>文本和显示下找到此页面。

## 锁屏调整到 PIN 和模式锁

Android 12 开发者预览版 2 对 PIN 和模式锁视图进行了一些细微的更改。这些变化不像我们上个月第一次向你展示的[泄露锁屏改造中看到的那样引人注目，但它们是我们在文章](https://www.xda-developers.com/android-12-new-lockscreen-notifications-design-leak/)[中描述的变化的一部分，涵盖了整体材料“下一个”变化](https://www.xda-developers.com/android-12-ui-changes-material-next/)。

在 PIN 和 pattern 视图中,“紧急呼叫”按钮周围现在有一个圆形气泡，与系统强调主题相匹配。在模式视图中，当您输入模式时，沿着手指的线条现在比以前粗了很多。

根据您为设备设置的主题，媒体播放器现在会跟随系统强调色。提醒一下，Android 11 中的通知面板[增加了一个媒体播放器。](https://www.xda-developers.com/android-11-media-controls/)

* * *

在第二个开发者预览版中还有一些其他的变化，包括一些隐藏的变化。如果你对阅读这些感兴趣，我们有一篇文章，涵盖了迄今为止我们在 Android 12 DP2 中发现的所有隐藏功能。