# Android 11 不能很好地处理控制器，但 Android 12 解决了这个问题

> 原文：<https://www.xda-developers.com/android-11-trouble-getting-games-recognize-their-controllers/>

自从 Android 11 [推出](https://www.xda-developers.com/android-11-stable-google-pixel-oneplus-xiaomi-realme-oppo/)以来，用户在试图将游戏控制器与智能手机连接时一直面临问题。据报道，运行 Android 11 的手机要么无法将控制器识别为输入设备，要么不允许用户正确映射按键。

根据官方 Android 问题追踪器上关于 bug 的[帖子，一些 Pixel 用户和 beta 测试人员面临这个问题，他们无法在自己的设备上使用 Xbox One 控制器、索尼的 DualShock 4 甚至谷歌自己的](https://issuetracker.google.com/issues/163120692?pli=1) [Stadia 控制器](https://www.xda-developers.com/stadia-wireless-controller-android-phone/)等蓝牙游戏控制器。虽然绝大多数报告来自 Pixel 2、Pixel 3、Pixel 3a、Pixel 4 和 Pixel 4a 用户，但一些运行 Android 11 版本的三星和一加用户也报告了类似的行为。

到目前为止，还没有确认到底是什么导致了这个问题。但值得注意的是，谷歌早在 2020 年 8 月就已经承认了这个问题，当时最初的 Android 11 版本开始接触用户。目前，开发团队似乎仍在试图找出潜在的原因，并努力带来一个可靠的解决方案。

虽然谷歌还没有找到解决方案，但一些用户已经分享了临时的解决方案。根据一些报告，这个问题可以通过关闭某些辅助功能选项来解决。例如，一个用户建议，*“可以确认，有一个特定的可访问性服务，如果我禁用它，控制器立即开始工作，不需要重新启动或任何东西。实际上，我可以在 Stadia 和 Settings 之间来回切换，禁用 Accessibility 上的服务，返回 Stadia，控制器工作；切换回设置，启用，回到视距，它突然死了，就像以前一样。没有重启，没有配对或连接/断开控制器，什么都没有。”*

如果您面临这个问题，您可以尝试上面提到的解决方法。在此之前，我们所能做的就是等待谷歌解决这个问题，并在未来的更新中发布修复程序。

* * *

## 更新 1:在 Android 12 中修复

*米沙·拉赫曼的章节*

在谷歌问题追踪器的[评论](https://issuetracker.google.com/issues/163120692#comment324)中，一名谷歌员工表示这个问题已经在 Android 12 中得到解决。该修复首次在 Android 12 Beta 4 中提供。这个错误的根本原因还没有被披露，但它可能与 Android 处理可访问性服务的方式有关。许多用户报告说，在“设置”中停用一个或多个辅助功能服务可以解决这个问题，但您的实际效果可能会有所不同。

*感谢 XDA 会员 [Some_Random_Username](https://forum.xda-developers.com/m/some_random_username.8234677/) 的提示！*