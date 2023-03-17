# 经过几个月的沉寂，Signal 终于更新了公共服务器代码

> 原文：<https://www.xda-developers.com/signal-updates-public-server-code/>

**更新 1 (04/09/2021 @ 04:00 PM ET):** 我们现在知道为什么 Signal 的后端服务器软件的更新源代码过了这么久才发布。[点击这里了解更多信息。](#update1)这篇发表于的文章保存如下。

由于专注于隐私和端到端加密，Signal Private Messenger 多年来一直是一个受欢迎的消息平台。该项目已经发布了 Signal 每个组件的源代码，包括后端服务器和客户端应用程序，但服务器软件的公共代码在几个月前就已经过时了，直到今天。

Signal 在远程服务器上存储尽可能少的信息，但仍然有一个服务器组件用于将用户与电话号码联系起来，发送推送通知和其他功能。Signal 已经在 GitHub 上提供了服务器软件的源代码，使得任何人都有可能[建立自己独立的基础设施](https://gist.github.com/WisdomSky/fd348eb012b8f37f6b9b7dbb69eed6e1)。然而，大多数人只是选择使用 Signal 的平台，因为不支持主服务器和自托管服务器(联盟)之间的通信。

去年 4 月 22 日之后，Signal 停止更新其服务器软件的公共代码库。此举令人担忧，因为 Signal 的开源特性使其更容易进行安全审计，并确保该平台不会泄露私人数据。继[在 Reddit](https://www.reddit.com/r/signal/comments/m4fun0/the_latest_version_of_signals_server_is/) 和 [Signal 自己的社区论坛](https://community.signalusers.org/t/where-is-new-signal-server-code-why-not-share-signal/15068)上的其他讨论之后，上个月又出现了一个关于缺乏发布的 [GitHub 问题](https://github.com/signalapp/Signal-Android/issues/11101)。

虽然 Signal 尚未公开声明代码发布中的差距，但该项目今天终于向[公共 GitHub 库](https://github.com/signalapp/Signal-Server/)发布了数百份提交。该库现在显示了 2020 年和 2021 年完成的许多代码提交，将最新的服务器版本从 [3.21](https://github.com/signalapp/Signal-Server/commit/3432529f9c018d75774ce89f3207b18051c26fe7) 提升到 [5.48](https://github.com/signalapp/Signal-Server/commits/master) 。

仍然不清楚为什么 Signal 这么长时间没有更新其公共服务器代码，特别是当该组织一直以开放和透明而自豪的时候。我们已经发出了声明的信号，如果我们得到回应，我们将更新我们的报道。

* * *

## 更新 1:解释

Signal 首席执行官莫邪·马林斯派克[对 GitHub 问题发表了评论](https://github.com/signalapp/Signal-Android/issues/11101#issuecomment-815400676),并解释了延迟的原因。他说，推迟并不是因为该公司试图在推出之前隐藏其在[新的注重隐私的支付功能](https://www.xda-developers.com/signal-testing-privacy-focused-payments-feature/)的细节，而是主要旨在防止垃圾邮件发送者收集该公司计划颁布的新的反垃圾邮件措施。他进一步重申，每个版本都发布客户端源代码，构建是可复制的，Signal 被设计为无论如何都不信任服务器，这意味着访问服务器源代码“没有安全后果”然而，他在结束时说，他理解为什么人们可能希望出于教育目的或运行自己的实例来查看服务器源代码，因此他承诺该公司将“在更实时地推动变化方面做得更好。”

以下是他的评论全文:

> #### “首先，很抱歉我们的一项服务的源代码落后了这么多。我们经常在发布之前不推送源代码，在那个时期发生了一些重叠的发布，这使得在任何时候推送都很困难，并使我们落后。此外，我们已经看到垃圾邮件的大量增加，并且不愿意立即发布我们正在应对的确切反垃圾邮件措施，因为垃圾邮件发送者可以立即看到这些措施与上述措施相结合，导致了这种极端的延迟。
> 
> #### 正如本主题中的人们所注意到的，我们的客户端源代码总是在每个版本中发布，构建是可复制的，并且一切都被设计成不信任服务器。对于这里的一些锡纸帽匠来说，非常清楚的是(在这一点上，如果没有你，互联网就不一样了，感谢你的服务)，我们没有任何“禁言令”，也没有 NSL，关键是我们没有可以安装在服务器上的“恶意软件”。
> 
> #### 即使没有安全后果，我们也明白了为什么 server source 对那些想运行自己的 Signal 版本、想了解 Signal 如何工作、想大致了解事物是如何构建的人很有用。我们会更好地实时推动变革。
> 
> #### 我们尽量不使用生长激素的问题进行讨论，所以我现在要关闭它，但打我们的论坛。"