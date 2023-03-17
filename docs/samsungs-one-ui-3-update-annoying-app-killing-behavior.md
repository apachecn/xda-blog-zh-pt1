# 据报道，三星的 One UI 3 更新增加了恼人的应用程序拦截行为

> 原文：<https://www.xda-developers.com/samsungs-one-ui-3-update-annoying-app-killing-behavior/>

# 据报道，三星的 One UI 3 更新增加了恼人的应用程序拦截行为

在最新的 One UI 3.0 更新中，三星似乎引入了一个新的应用程序扼杀政策，该政策影响了应用程序在后台的工作方式。

在其最新的 [One UI 3.0 更新](https://www.xda-developers.com/samsung-one-ui-3-1-features-changes/)中，三星似乎引入了一个新的应用程序扼杀政策，该政策影响了一些应用程序在后台的工作方式。该限制似乎过于激进，在实施过程中破坏了许多应用程序。

正如 Urbandroid 团队(Sleep as Android 和 Twilight 等热门应用的开发商)发现的那样，新的限制是最近 Android 11 更新的一部分。它在默认情况下是打开的，在如何处理后台运行的应用程序方面更加积极。应用程序无法保持唤醒锁和广播消息，这反过来破坏了许多用例。例如，当屏幕关闭时，依赖后台活动继续收集传感器数据的健康应用程序现在无法正常工作。该团队所做的测试表明，新政策在设备闲置且屏幕关闭的 3 分钟内生效。

三星也没有提供面向用户的选项来完全关闭这种新行为。似乎退出这一激进政策的唯一方法是禁用 Android 的标准电池优化。为了确保您最喜爱的应用程序不会意外终止，并在运行 Android 11 的 Galaxy 设备上按预期工作，请进入设置>应用程序>“您的应用程序”>电池>电池优化>所有应用程序>“您的应用程序”>不要优化。

Android 已经有了相当强大的省电功能，比如[瞌睡](https://www.xda-developers.com/how-android-n-will-improve-battery-and-memory-management/)和应用待机。但是，许多原始设备制造商喜欢执行他们自己的，而且通常[更激进的](https://www.xda-developers.com/huawei-cant-download-vlc-play-store/)策略来处理后台活动。这通常被宣传为实现更长电池寿命的一种方式，但通常是以[应用程序意外死亡](https://www.xda-developers.com/phone-software-killing-apps-background/)和无法按预期完成工作为代价的。

目前还不清楚这一新的后台政策是影响每一台运行 Android 11 的三星 Galaxy 设备一次 UI 3.x 更新，还是仅限于部分型号。

在 Galaxy 智能手机上安装了基于 Android 11 的 One UI 3.0 更新后，您是否注意到您的应用程序出现了任何意外行为？请在下面的评论中告诉我们。