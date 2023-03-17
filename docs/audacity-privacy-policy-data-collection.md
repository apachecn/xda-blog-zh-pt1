# Audacity 的新隐私政策再次引发了人们对数据收集的担忧

> 原文：<https://www.xda-developers.com/audacity-privacy-policy-data-collection/>

开源音频编辑器 Audacity 最近因其更新的隐私政策而成为新闻。几家媒体[报道](https://fosspost.org/audacity-is-now-a-spyware/)这些改变是入侵性的，甚至[将音频编辑器贴上间谍软件的标签](https://www.slashgear.com/audacity-open-source-audio-editor-has-become-spyware-05681012/)。Audacity 的新所有者 Muse Group 现在分享了一份声明，澄清了新的隐私政策条款。

对于不知道的人来说，Audacity 是一个免费的开源多声道音频编辑器和录音机，适用于 Windows、Mac 和 Linux。今年 4 月，[被 Muse Group](https://mu.se/newsroom/tpost/6dhedma301-muse-group-acquires-audacity-expanding-c) (音乐符号软件“MuseScore”和在线“终极吉他”社区的所有者)收购，作为收购的一部分，Muse Group 获得了商标权，但承诺“Audacity 的数千万用户可以放心，该软件将永远免费和开源。”

收购一个月后，Muse Group [宣布](https://github.com/audacity/audacity/pull/835)计划为 Audacity 添加基本的遥测数据收集功能。该公司计划使用这些数据来确定应用程序不稳定的问题，估计其用户群的规模，就支持哪些操作系统版本做出明智的决策，并估计 Audacity 3.0 中引入的新文件格式的影响。为此，该公司还计划实施谷歌分析和 Yandex Metrica。但它承诺所有的数据收集将是“严格可选的，默认情况下是禁用的。”

一些 Audacity 用户对 Muse Group 将遥测技术引入 Audacity 的决定感到不满，并认为该公司可以使用这些数据来描述用户或将其出售给第三方。由于强烈反对，Audacity 团队[宣布](https://github.com/audacity/audacity/discussions/889)已经放弃了提议的遥测功能。然而，它计划实现错误报告和检查更新的能力。

几天前，[许多用户发现【Audacity 更新了其隐私政策，加入了一项条款，允许 Muse Group 收集“执法、诉讼和当局请求所需的数据”等。这让用户担心遥测数据被收集以及它的用途。然而，该公司现在发布了另一份声明，澄清新的隐私政策条款。](https://www.reddit.com/r/linux/comments/od3h8b/audacity_may_collect_data_necessary_for_law/)

在 GitHub 上最近的一篇文章中，该公司声明:*“我们认为担忧主要是由于隐私政策中不明确的措辞，我们现在正在纠正这一点。与此同时，我们希望澄清主要的关注点。”*帖子进一步声明，Audacity 不会出售任何用户数据，也不会与第三方分享。它将收集有限的数据，包括 IP 地址、基本系统信息(操作系统版本和 CPU 类型)和错误报告数据(可选)。音频编辑器不会收集任何额外的数据，也不会与执法部门分享这些数据，除非法庭强制要求。此外，该公司澄清说，隐私政策不适用于离线使用。

尽管澄清，许多 Audacity 用户在评论中表达了他们对新隐私政策的担忧。谢天谢地，新的隐私政策还没有生效。它是针对即将到来的 3.0.3 版本的，所以如果你不想同意新的条款，你可以继续使用旧版本。或者，您可以在没有任何错误报告或更新检查的情况下从源代码编译 Audacity，这些特性默认情况下通过 CMake 选项被排除。