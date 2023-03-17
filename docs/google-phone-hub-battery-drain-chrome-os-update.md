# 谷歌将在未来的 Chrome 操作系统更新中解决 Phone Hub 的电池耗尽问题

> 原文：<https://www.xda-developers.com/google-phone-hub-battery-drain-chrome-os-update/>

# 谷歌将在未来的 Chrome 操作系统更新中解决 Phone Hub 的电池耗尽问题

谷歌将在未来的 Chrome 操作系统更新中解决 Phone Hub 的电池耗尽问题。请继续阅读，了解即将到来的变化。

谷歌今年 3 月早些时候开始推出 Chrome OS 89。十周年更新包括一系列新功能，包括一个新的电话集线器，帮助用户将他们的 Android 手机连接到 Chromebook。该功能为 Chrome OS 添加了一个内置的控制中心，让用户可以检查手机的电池寿命，打开/关闭热点，并轻松定位他们的设备。它甚至允许用户回复信息和查看他们最近的 Chrome 标签。然而，自其发布以来，许多用户[报告称，当他们的手机连接到使用该功能的 Chromebook 时，出现了严重的电池耗尽问题](https://www.reddit.com/r/chromeos/comments/lwms9y/battery_drain_on_phone_after_turning_on_phone_hub/)。幸运的是，谷歌已经意识到了这个问题，并已经着手解决。

正如 [*Android Police*](https://www.androidpolice.com/2021/07/05/phone-hub-for-chromeos-may-finally-fix-the-massive-android-battery-drain/) 所发现的，Chromium Gerrit 上一个新的[正在进行的工作提交](https://chromium-review.googlesource.com/c/chromium/src/+/2872256)表明，谷歌正在努力使你的 Chromebook 和 Android 手机之间的连接更加有效。它的描述指出:

*“此更改允许附近的连接客户端在连接到附近的设备时请求特定的保持活动和超时。Nearby Share 保持默认值，而 Phone Hub 则选择使用电池更友好的选项。Phone Hub 的变化是由一个功能标志决定的，所以它可以在 Android 端准备就绪时推出。”*

在当前的 Chrome OS 版本中，Phone Hub 以 5 秒的间隔轮询其与您的手机的连接状态。上面提到的改变将实质上增加轮询持续时间，这应该是电池耗尽的问题。但是，增加时间间隔也意味着 Phone Hub 更新手机状态的时间会更长。这种差异可能不会很明显，因为这种变化只会将持续时间[增加到 15 秒](https://chromium-review.googlesource.com/c/chromium/src/+/2872256/10/chrome/browser/chromeos/secure_channel/nearby_connection_broker_impl.cc#58)。

目前，我们还不确定这一变化何时会向用户推出。我们会尽快更新这篇文章。