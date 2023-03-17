# 你现在可以通过 WSL 在 Windows 10 上运行带有图形用户界面的 Linux 应用程序

> 原文：<https://www.xda-developers.com/run-gui-linux-apps-windows-10-wsl/>

Windows 可能是最受欢迎的桌面操作系统，但这并不意味着它可以做任何事情。例如，如果你想做类似于[运行 JetBrains 投影仪服务器](https://www.xda-developers.com/android-studio-remote-development-jetbrains-projector/)的事情，你需要一个基于 Unix 的系统，比如 Linux。微软不久前推出了 Windows Subsystem for Linux (WSL ),它支持直接从 Windows 安装中运行 Linux 应用程序。

但是 WSL 有一些限制。版本 1 甚至没有使用完整的 Linux 内核，所以很多应用程序仍然无法运行。版本 2 做了很多改进，但是仍然缺少一些东西:GUI 应用程序支持。

当然，你总是可以建立一个 hacky 解决方案，在 Windows 上安装一个 X 服务器，处理一些端口转发，并在 WSL 中建立一个自动环境变量，但是这很麻烦，而且并不总是工作得很好。

输入 WSLg。

## WSLg:在 Windows 10 上用 GUI 运行 Linux 应用

WSLg 是微软对 Linux GUI 问题的回答，老实说有点奇怪。这是一个有趣的图表，它是如何工作的，由微软提供。

这里有很多事情要做，但是基本的想法实际上非常类似于建立你自己的 X 服务器的旧的手动方法。相反，X 服务器运行在一个用户看不见的并行 WSL 实例上。然后，Windows 使用远程桌面协议将视频和音频从该不可见实例传输到 Windows 端。这听起来可能很复杂，的确如此，但它确实有效。

微软还表示，即使通过所有这些层，Linux 应用程序也应该能够利用你的 GPU，比如 OpenGL passthrough。目前，这种行为需要 AMD、Intel 或 NVIDIA 的特殊驱动程序，但计划在未来默认捆绑它。

这种未来可能会在今年下半年到来，伴随着 Windows 21H2 [和一个大的 UI 革新](https://www.xda-developers.com/microsoft-big-ui-overhaul-windows-10-2021/)。Windows 开发者平台的项目经理 Craig Loewen 在 Twitter 上证实，在下一个主要的 Windows 版本中，所有用户都将获得对 Linux 应用程序的 GUI 支持。

## 特征

现在，WSLg 实际上看起来功能相当完善。据称，您可以拥有对 Linux GUI 应用程序的完整视频和音频支持，以及 3D 加速。而且非常无缝。当一个新的 GUI 应用程序安装在 WSL 实例中时，它甚至会被添加到开始菜单中，所以您可以直接启动它。应用程序应该显示在与相应的 WSL 实例同名的文件夹下。

## 疯狂的

当然这是早期发布，有一些 bug。就我个人而言，当我在我的一台笔记本电脑上设置它时，我甚至无法运行任何应用程序。我也没有得到任何应用程序的开始菜单条目。然而，这背后的团队做出了令人难以置信的响应，至少第一个问题已经在下一个版本中得到解决。

显然还有其他涉及复制粘贴和音频中断的问题。你可以在 [WSLg GitHub 库](https://github.com/microsoft/wslg/issues/)上查看完整的问题列表。

## 入门指南

那么如何获得 WSLg 呢？那么目前最简单的方法就是更新到 Windows 10 Insider 的最新开发者环版本(build 21364 或更高版本)。一旦你这样做了，你可以简单地在提升的命令提示符或 PowerShell 窗口中运行 **wsl - update** ，然后运行 **wsl - shutdown** 。

然后只需打开一个 WSL 实例，运行一个带有 GUI 的 Linux 应用程序。假设一切顺利，你会看到你的应用看起来几乎像一个原生的 Windows 应用。否则，检查 GitHub 问题，或者如果需要，提交您自己的问题。

## 资源

要了解更多关于带有 GUI 的 Linux 应用程序如何运行的信息，请务必查看以下资源:

或者观看 Craig Loewen 的演练和示例视频: