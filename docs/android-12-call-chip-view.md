# Android 12 可以显示一个状态栏芯片，显示正在进行的通话的持续时间

> 原文：<https://www.xda-developers.com/android-12-call-chip-view/>

**更新 1 (08/12/2021 @ 11:38 PM ET):** 谷歌手机应用程序在 Android 12 上推出支持显示状态栏芯片的持续通话时间。[点击这里了解更多信息。](#update1)文章发表于 2021 年 6 月 14 日，下面保留。

[Android 12](https://www.xda-developers.com/android-12/) Beta 2 正式来了。我们已经对新软件进行了一次[深度挖掘，发现了谷歌自 Beta 1 以来的所有新功能和变化。第二个测试版是向前迈出的一大步，因为它将 Android 12 的许多重要功能带入了生活，这些功能在之前的版本中是隐藏的或正在进行中。例如，谷歌在 Google I/O 2021 上展示的新隐私仪表板现在在 Beta 2 中完全可用。此外，Material You 的动态主题化功能也是实时的，同时还有新的通知重新设计和改进的电源菜单。](https://www.xda-developers.com/android-12-beta-2-features/)

因为这是测试版软件，毕竟，有些功能仍在开发中，用户无法使用。其中一个正在开发的功能是新的通话状态栏指示器。我们在深入研究 Android 12 Beta 2 的代码时发现了这个功能。这项功能实际上是默认启用的，但由于谷歌手机应用程序还不支持它，它对最终用户是不可见的。但是感谢 Android 开发者 [@kdrag0n](https://twitter.com/kdrag0n) ，我们现在可以第一次看到 Android 12 新的持续通话芯片。

为了测试这个特性，kdrag0n 实现了新的[通知。在他的 Android 12 扩展](https://developer.android.com/about/versions/12/features#:~:text=Using%20this%20template%20lets%20your%20app%20indicate%20the%20importance%20of%20active%20calls%20by%20displaying%20a%20prominent%20chip%20that%20shows%20the%20time%20of%20the%20call%20in%20the%20status%20bar%3B%20the%20user%20can%20tap%20this%20chip%20to%20return%20to%20their%20call.)[应用](https://github.com/kdrag0n/android12-extensions)中调用 Style 。

正如你在上面的截图中看到的，当一个呼叫正在进行，并且用户离开主呼叫屏幕时，Android 12 会在状态栏中显示一个突出的芯片，显示呼叫的持续时间。Android 11 目前不在状态栏显示你正在进行的通话时长。要检查通话持续时间，您必须返回到主通话屏幕或下拉通知托盘。

如上所述，Beta 2 中已经支持新的呼叫芯片功能。一旦谷歌更新谷歌手机应用程序，它应该会为每个人上线。

* * *

## 更新 1:谷歌手机应用增加支持

Tipster @ [panduu221](https://twitter.com/panduu221) 最近联系到我们，表示他们在状态栏中看到了正在进行的通话筹码。用户运行的是 Google Phone 应用程序的 Beta 3 版本 68.0.388241074-publicbeta。如果你看到这个功能，请在下面的评论中告诉我们！