# 找出你的电脑无法运行 Windows 11 的确切原因

> 原文：<https://www.xda-developers.com/tool-tells-you-exactly-why-pc-cant-run-windows-11/>

微软即将推出的 [Windows 11](https://www.xda-developers.com/windows-11/) 操作系统是十多年来第一个显著提高系统要求的操作系统版本。这也不仅仅是一两件事，比如需要更多的 RAM 或存储(尽管你确实需要更多的 RAM 和存储)。[最低要求全面上调](https://www.xda-developers.com/windows-11-minimum-requirements/)。

微软[发布了一个叫 PC Health](https://www.xda-developers.com/windows-11-can-my-pc-run-it/) 的 app，一直不太好。它最近才更新，告诉你*为什么*你不能有 Windows 11。起初，它只告诉你不能运行 Windows 11，而没有告诉你缺少什么要求。

一款名为 WhyNotWin11 的新应用旨在解决这个问题，它可以在 GitHub 上获得。它分解了你的电脑的哪些部分与 Windows 11 最低要求兼容，哪些部分不兼容。根据上面的截图，其实是在 2.1.0.0 版本上。开发人员 Robert C. Maehl 在两天内实际上已经发布了九个版本。

其他增加的是 CPU 需求。首先，Windows 11 现在需要 64 位 CPU，它需要至少两个至少 1GHz 时钟速度的内核。不过这似乎无关紧要，因为实际上有一个 CPU 列表。该列表排除了任何早于英特尔第八代芯片的产品。

另一个新要求是 TPM 2.0，这是一个安全特性。如果它说你没有这个，你可能需要[检查你的 BIOS 是否启用了它](https://www.xda-developers.com/how-to-check-pc-tpm-windows-11-upgrade/)。

WhyNotWin11 列出了 Windows 11 的每一项要求。如果它会被阻挡，它们会被清楚地标记为红色，如果你可以继续，它们会被标记为绿色。从上图可以看出，AMD 锐龙 7 1800X 处理器是用黄色标记的。该芯片不在支持的处理器列表中，但仍然有一些争论，即该列表是否会真正阻止你获得 Windows 11。

要查看 WhyNotWin11，你可以[在 GitHub 上找到它，这里](https://github.com/rcmaehl/WhyNotWin11)。