# Parallels Desktop 17 for Mac 评论:越做越好

> 原文：<https://www.xda-developers.com/parallels-17-mac-review/>

毫无疑问 macOS 很棒。它有一个干净的现代外观，在苹果优化的硬件上运行速度惊人。也就是说，有时候你需要使用 Windows，即使是在你的 Mac 上。Parallels Desktop 17 是与 macOS 并行运行 Windows 的流行软件的最新版本。有许多你可以使用的程序仍然只能在 Windows 上运行。您可能还需要运行一些 Windows 应用程序来工作。对于那些喜欢在笔记本电脑上玩游戏的人来说，在 Mac 上运行一些 PC 游戏的能力是一个额外的好处。

[Parallels Desktop 17 for Mac](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU4855/https://www.parallels.com/products/desktop/) 最吸引人的功能之一是能够在您的 Apple 硬件上运行 Windows 11。目前，Windows 11 目前通过 Windows Insider 计划提供测试版。此外，您可以使用 Parallels Desktop 17 在虚拟机中运行 macOS Monterey。这是 Parallels Desktop 第一次将苹果芯片和英特尔兼容性整合到一个应用程序中，如果您需要在 M1 Mac 上使用 Windows 程序，这是一件大事。

过去几周，我一直在我的 2018 Macbook Pro 15 "上使用 Parallels Desktop 17，采用酷睿 i9 处理器。在本次回顾中，我们将了解 Parallels 17 的新特性，并讨论整体性能。

**浏览此评论:**

## Parallels Desktop 17 for Mac 的新增功能

Parallels Desktop 17 显然有很多新功能。我不可能在这篇评论中对每一个新特性都做出公正的评价，所以我选择了几个重要的特性来强调。以下是我认为从可用性角度来看最重要的五个新特性。

### 针对 Windows 11 和 macOS Monterey 进行了优化

Parallels Desktop 针对 Windows 11 和 macOS Monterey 进行了最新优化，可持续保持最新状态，因此您可以不间断地工作——即使出现新的 macOS、Windows 或 Linux 版本。您目前可以在 Parallels Desktop 17 上运行 Windows 11，首先安装 Windows 10，然后加入 Windows Insider 计划。我已经使用 Parallels 17 在我的 2018 英特尔 Macbook Pro 上运行了 Windows 11 Pro，到目前为止没有问题。不仅安装 Windows 11 很容易，而且它还继承了 Windows 10 中所有流行的 Parallels 功能。

您也可以使用 Parallels 17 将 macOS Monterey 安装为虚拟机。这样做的唯一缺点是，您必须在您的主机 Mac 上运行 Monterey，才能在虚拟机中设置 Monterey。这显然现在有点令人失望，因为 Monterey 还在测试阶段，但对于以后的用例来说，这不是问题。事实上，你也可以运行几个旧版本的 macOS，包括 macOS Big Sur 11、macOS Catalina 10.15、macOS Mojave 10.14 和 macOS High Sierra 10.13。

### 图形速度改进

Parallels Desktop 17 中改进的显示驱动程序提供了更流畅的 Windows UI 响应和同步视频播放。除了性能改进之外，新驱动程序还提高了许多 Windows 游戏的帧速率，以获得更好的游戏体验，并提供与 Mac 显示器更好的同步。

图形部门的这些改进在使用 OpenGL 实现 2D 图形的游戏中最为明显。我测试了游戏“Smelter ”,没有发现丢帧现象。这非常类似于在 Windows PC 上玩这个游戏。在 Parallels Desktop 的旧版本中，像“Smelter”这样的游戏由于糟糕的图形性能几乎无法运行。

我还使用 [Vsync Tester](https://www.vsynctester.com) 在 Windows 中运行了一个快速的每秒帧数测试，以验证游戏时见证的改进。您可以从上面的截图中看到，在 Parallels 17 中几乎没有丢帧(注意我的测试中平均接近 60FPS)。

### 在 Mac 和 Windows 之间拖放文本/图形

在 Parallels Desktop 17 中，您现在可以快速轻松地在 Mac 和 Windows 应用程序之间拖放文本或图形。在 macOS Monterey 上，你也可以像从 macOS 应用程序一样轻松地将任何内容从 Windows 应用程序拖放到 Quick Note。这个过程在我的经验中是绝对无缝的。

如果你在 Parallels 中使用 Coherence 模式，看起来你根本不是在使用 Windows。你可以打开任意多的 Windows 应用程序，它们的行为就像 macOS 中的任何其他应用程序一样。这样，拖放文本或图像的过程就像是在原生 Mac 应用程序之间进行简单的拖放。

### Windows 电池状态

使用 macOS 时，您可以点按右上角的电池图标来获取您的电池状态。有了 Parallels 17，您现在也可以在 Windows 中获得准确的电池状态。如果你打算花更多时间在 Windows 而不是 macOS 上，这是一个非常方便的新功能。

除了查看准确的百分比，Windows 还可以识别 Mac 何时电量不足，并打开电池节电模式。这是在 Parallels 中无缝使用 Windows 的另一个例子。

### 更好的磁盘空间控制

过去，在 Mac 上使用 Parallels Desktop 时，磁盘空间管理可能是个问题。当您暂停虚拟机时，Parallels 会存储快照以记住 Windows 的完整状态。这些快照通常会占用大量存储空间，如果您不注意，这可能会成为一个问题。

现在，在 Parallels 17 中，您可以更好地了解 Mac 资源和内存。快照使用的磁盘空间现在在更新的*释放磁盘空间*助手中计算。如果你的 Mac 存储空间不足，你可以使用*释放磁盘空间*助手来优化可用资源，并获得相当大的空间。

## Parallels Desktop 17 for Mac 的日常性能

总的来说，我对 Parallels 17 的体验非常积极。打开 Windows 11 的速度非常快，在很长一段时间后恢复暂停的 Windows 11 虚拟机也是如此。图形性能比以前版本的 Parallels 要好很多，现在有很多有趣的游戏可以在 Windows 上玩。除了“Smelter”之外，我还测试了“King Rush Frontiers ”,运行时没有打嗝。

所有被吹捧的功能都很棒，比如文本/图像的拖放，Windows 11 中的电池状态，以及新的存储优化工具。我还运行 macOS Monterey 作为我的主机操作系统，而 Windows 11 Pro 是我在虚拟机中运行的客户操作系统。我想也许同时运行这两个会产生一些问题(因为它们目前都在测试中)，但是我很高兴地报告到目前为止还没有问题。

我注意到我的 MacBook Pro 粉丝在运行 Parallels Desktop 17 时会定期开机，即使在 Windows 11 中执行相当基本的任务时也是如此。这可能是我的 Core i9 处理器的问题，而不是软件问题，但不管怎样，这还是值得一提的。当然，Parallels 会消耗大量系统资源，所以当你在 Windows 中执行要求更高的任务时，一定要保持警惕。

## 定价和可用性

如果您有兴趣购买该软件，Parallels Desktop 17 有三个不同的版本-标准版、商务版和专业版。所有上述功能都可以在标准版中获得，适用于个人、小型企业和教育用户，需要 79.99 美元的年费。该订阅包括所有未来的升级，但也有可能以 99.99 美元的价格购买标准版作为一次性购买的“永久许可证”，未来的升级需要额外收费。

专业版在此次升级中为 M1 MAC 电脑添加了一个 Microsoft Visual Studio 插件，并改进了管理多个“克隆”虚拟机的选项。面向企业用户的商业版现在允许用户在整个组织内将预配置的虚拟机部署到英特尔和 M1 MAC 电脑上。商业版和专业版只提供年度订阅，每个价格为 99.99 美元。Parallels Desktop 17 现在可以下载。

## 结论

需要在苹果电脑上运行 Windows 应用程序的用户仍然最适合运行 Parallels Desktop，而不是其他替代品。这款流行软件的最新版本是迄今为止最好的，它支持 Windows 11、macOS Monterey，并提高了苹果 M1 Macs 的性能。如果您是一名需要在苹果电脑上运行像 AutoCAD 这样的 Windows 应用程序的工科学生，这是您可以为学校购买的最好的产品之一。

除了兼容性升级，Parallels Desktop 17 还全面提升了图形性能，尤其是在 OpenGL 游戏中。Coherence 模式和 Parallels Toolbox for Mac and Windows 带来的额外便利使其成为并行运行 Windows 和 Mac 应用程序的最佳软件包。如果你对在 Chrome OS 上运行 [Windows 感兴趣，Parallels Desktop 也能帮上忙。](https://www.xda-developers.com/windows-10-chrome-os/)

 <picture>![Parallels Desktop 18 for Mac offers support for Windows 11, macOS Ventura, and Apple Silicon hardware. All of these features come with added performance improvements, making this the best Parallels Desktop yet.](img/b964ca11c8cbd7e6c9bfbbd2a5b11c63.png)</picture> 

Parallels Desktop 18 for Mac

##### Parallels 桌面

新的 Parallels Desktop 17 for Mac 支持 Windows 11、macOS Monterey 和 Apple silicon 硬件。所有这些新功能都带来了额外的性能改进，使其成为迄今为止最好的 Parallels Desktop。