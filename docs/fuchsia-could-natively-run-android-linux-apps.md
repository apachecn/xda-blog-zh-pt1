# 谷歌提出了一种让 Fuchsia“原生”运行 Android 和 Linux 应用的方法

> 原文：<https://www.xda-developers.com/fuchsia-could-natively-run-android-linux-apps/>

自从开始以来，Fuchsia 总是给人一种有点神秘的感觉。谷歌自 2016 年以来一直在公开研究它，但直到 2019 年 5 月，这家搜索巨头才评论它的存在，称[这只不过是一个实验](https://www.xda-developers.com/google-acknowledges-fuchsia-os-experiment/)。与构建在 Linux 内核之上的 Android 和 Chrome OS 不同，Fuchsia 使用了一种新的名为锆石的微内核。谷歌将 Fuchsia 描述为“安全、可更新、包容、实用”的开源操作系统。

围绕谷歌计划用 Fuchsia 完成什么，有多种理论在流传，其中最受欢迎的一种是 Fuchsia 最终将取代 Android 和 Chrome 操作系统。不过，与成熟的 Android 平台相比，这个操作系统仍然处于起步阶段，这不太可能很快发生。然而，如果谷歌的一项新提议(通过 [*、瑟罗特*](https://www.thurrott.com/mobile/247226/google-investigating-m1-like-os-translation-for-fuchsia) )实现的话，Fuchsia 似乎可以运行原生的 Android 和 Linux 应用。

在 Fuchsia Gerrit 上提交的文件提议开发一个名为 Starnix 的兼容层，它可以“将来自 Linux 客户端程序的请求翻译到 Fuchsia 子系统”，本质上允许原生 Android 和 Linux 应用程序在该平台上运行，而不必求助于虚拟机或仿真器。

> 当我们扩展我们希望在 Fuchsia 上运行的软件领域时，我们遇到了我们希望在 Fuchsia 上运行但我们没有能力重新编译的软件。例如，Android 应用程序包含为 Linux 编译的本机代码模块。要在 Fuchsia 上运行这个软件，我们需要能够在不修改二进制文件的情况下运行它们。

该提案进一步指出，这个兼容层的目的是“创建一个可以运行现有的、未经修改的 Linux 二进制文件的 Linux 接口的实现。”如果你对技术方面的东西感兴趣，你可以在这里通读提案文档[。](https://fuchsia-review.googlesource.com/c/fuchsia/+/485181/1/docs/contribute/governance/rfcs/NNNN_starnix.md#57)

在 Fuchsia 上运行原生 Android 和 Linux 应用的能力听起来令人兴奋。然而，值得注意的是，这仅仅是一个提议——而不是最终特性的实际文档——很可能不会被纳入操作系统。

尽管目前对 Fuchsia 的最终目标知之甚少，但它的开发一直在稳步进行。谷歌最近[扩展了 Fuschsia 的开源模式](https://opensource.googleblog.com/2020/12/expanding-fuchsias-open-source-model.html)以允许公众贡献。该公司为与项目相关的讨论建立了新的邮件列表，增加了一个治理模型，还为公众贡献开辟了一个问题跟踪器。