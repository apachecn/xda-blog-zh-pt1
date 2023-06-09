# 微软表示不会在 M1 MAC 电脑上支持 Windows 11

> 原文：<https://www.xda-developers.com/microsoft-wont-support-windows-11-m1-macs/>

一名微软发言人告诉 [The Register](https://www.theregister.com/2021/09/10/windows_11_m1/) 在装有苹果 M1 的个人电脑上运行 [Windows 11](https://www.xda-developers.com/windows-11/) “不支持这种情况”。就是这样；故事就是这样。Windows 10 不支持的东西，微软从未承诺支持，Windows 11 也不会支持。

需要说明的是，这句话并不意味着在 M1 Mac 上运行 Windows 11 就不行，至少通过 Parallels 这样的虚拟化解决方案不行。只能说明不支持。如果出现问题，您尝试联系 Microsoft 支持，他们会告诉您这是您的问题。

是这样的。微软目前不为 ARM 上的 Windows 提供 ISO 镜像。你*能*得到的是一个用于虚拟机的 Windows Insider 预览版的 VHDX 文件。这是您在 M1 Mac 电脑上使用 Parallels 安装并运行 Windows 11 的文件。

然而，这并不是微软开始发布它们的初衷。这是因为从 Windows 10 内部预览版 19559 开始， [Redmond 公司开始在 ARM 设备上提供 Hyper-V](https://sinclairinat0r.com/2020/02/04/running-hyper-v-in-windows-on-arm)。为了在 ARM PC 的 Windows 上运行虚拟机，你需要一个 ARM 映像，就像在 M1 Mac 上一样。这就是为什么该公司开始在 ARM 版本上发布 Windows 的虚拟硬盘。

显然，那发生在 2020 年初，而我们在这里；用于 ARM 上的 Windows 的 Hyper-V 尚未向非业内人士发售。这是由于各种原因导致 Windows 10 获得了支持包更新，而不是实际的功能更新。你会注意到，即使 Windows 10 版本 21H2 即将更新，版本号(19044)仍然低于第一个在 ARM 上获得 Hyper-V 的版本。

那个 Windows 10 开发分支最终变成了 Windows 11。当新的操作系统于 10 月 5 日发布时，ARM PCs 将支持 Hyper-V。据推测，这意味着微软将在那时开始提供生产 VHDX 图像(专业提示:目前提供给内部人士的将是生产图像)。

既然我们已经讨论了 ARM 上的 Windows、它的映像以及它们存在的原因，你可能想知道是什么阻止了你在 M1 Mac 上安装 Windows 11。事实是，现在没有什么能阻止你。Windows 11 确实有一个更严格的运行 CPU 列表，在 ARM 方面，包括高通制造的芯片组，Snapdragon 835 除外。苹果 M1 根本不是受支持的处理器，尽管 Parallels 说它正式支持 Windows 11。

微软还表示，如果你通过新媒体安装 Windows 11，它不会检查以确保你有一个支持的处理器。你猜对了，它只会给你留下一个不受支持的场景。

与在 Mac 上的任何虚拟机中运行 Windows 一样，您仍然需要 Windows 许可证。如果你已经有了一个产品密钥，那就可以了，或者你可以像平常一样买一个。

现在提供给 Windows 内部人员的版本是 [Windows 11 build 22000.132](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewARM64) ，这应该是该操作系统的生产版本。以防微软*在 Windows 11 发布后*不提供 VHDX 图像，你可能想在它被切换到开发频道版本之前下载这个。

 <picture>![Parallels Desktop lets you run virtual machines on your Mac.](img/7ebdcb284ee34e9a4f5d9eaf7c66ff14.png)</picture> 

Parallels Desktop

##### Parallels 桌面

Parallels Desktop 允许您在 Mac 上运行虚拟机。