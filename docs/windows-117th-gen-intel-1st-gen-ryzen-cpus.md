# Windows 11 可能不会将第七代英特尔和第一代锐龙 CPU 抛在后面

> 原文：<https://www.xda-developers.com/windows-117th-gen-intel-1st-gen-ryzen-cpus/>

当微软发布 Windows 11(T1)的文档时，很明显这将是十多年来,( T2)首次显著提高 Windows(T3)的最低要求。最低 RAM 和存储分别增加到 4GB 和 64GB。对于 CPU，不再支持 32 位，也不支持单核芯片。

但是此外，微软[对受支持的 CPU 代次](https://www.xda-developers.com/cpus-compatible-windows-11/)画了一条硬线。对于英特尔，你需要第八代或更新，对于 AMD，你需要锐龙 3000 或更新。对此有些愤慨。幸运的是，微软今天宣布，它可能会向英特尔的第七代芯片和 AMD Zen 1 开放。

在一篇解释新系统要求的[博客文章](https://blogs.windows.com/windows-insider/2021/06/28/update-on-windows-11-minimum-system-requirements/)中，它说 Windows 11 是一组功能，所以它需要安装在能够支持这些功能的芯片上。这包括第八代和更新的英特尔，AMD Zen 2 和高通 7 和 8 系列。它还说，英特尔第六代和更老的产品，以及 AMD pre-Zen 根本无法满足 Windows 11 的标准。然而，英特尔的第七代芯片和 AMD Zen 1 *可能*没问题。这将通过内部人士来检验他们。

具体来说，这篇博客文章说，“当我们向 Windows 内部人士发布并与我们的原始设备制造商合作时，我们将进行测试，以确定运行在英特尔第 7 代和 AMD Zen 1 上的设备可能符合我们的原则。随着时间的推移，我们致力于与您分享我们测试结果的更新，并分享其他技术博客。”

虽然 TPM 2.0 是 Windows 11 的一项要求，但这并不是新芯片的唯一要求。还需要考虑其他安全特性，例如基于虚拟化的安全性(VBS)、受虚拟机管理程序保护的代码完整性(HVCI)和安全引导。另外，CPU 需要采用新的 Windows 驱动程序模型。

这解释了为什么 Windows 11 发货时的最低要求与 Windows Insider 计划中的测试要求不同。你可以注册一台采用第七代英特尔 CPU 的电脑，例如最新的微软 Surface Studio 2，但当 Windows 11 推出时，你可能无法运行它。

微软提到的另一件事是，它正在推出 [PC 健康应用](https://www.xda-developers.com/microsoft-updates-pc-health-why-windows-11/)，该应用旨在帮助你了解你的 PC 是否与 Windows 11 兼容。它将努力使它变得更好，然后它将重新发布应用程序。与此同时，[第三方工具](https://www.xda-developers.com/tool-tells-you-exactly-why-pc-cant-run-windows-11/)已经在告诉你为什么你的电脑不能运行 Windows 11 方面做得更好，尽管这些工具需要根据今天对最低要求的澄清进行更新。

**更新:**微软已经删除了其博客文章中称英特尔第六代和更早的芯片以及 AMD pre-Zen 处理器肯定不符合其标准的部分。