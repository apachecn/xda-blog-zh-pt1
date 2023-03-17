# 开发人员通过苹果硅 Mac 上的虚拟化启动 Windows 10 和 Linux

> 原文：<https://www.xda-developers.com/apple-silicon-mac-boot-windows-10-and-linux-virtualization/>

自从苹果宣布为 Mac 系列定制基于 ARM 的芯片组[苹果 M1 SoC](https://www.xda-developers.com/apple-macbook-air-macbook-pro-13-mac-mini-m1-arm-soc/) 以来，改装爱好者一直在等待该平台的全面开放。长期以来，用户一直在思考是否有可能在 ARM Macs 上启动 Windows 或标准 Linux 发行版。毕竟，[主线 Linux 内核](https://www.xda-developers.com/samsung-galaxy-siii-samsung-galaxy-note-ii-htc-hd2/)和 [Windows 10](https://www.xda-developers.com/windows-10-arm-oneplus-6t/) 对于 ARM 界来说并不陌生。剩下的只有对破译苹果定制 ARM 实现足够感兴趣的开发人员的血汗和眼泪。现在，由于多个开发者的努力，在苹果硅 Mac 上启动 Windows 10 和 Linux 已经成为可能，尽管是通过虚拟化。

来自亚马逊 AWS 的工程师 Alexander Graf 一直在摆弄流行的开源机器仿真器和虚拟化器 QEMU，以添加苹果芯片支持。他在[投入了大量的工作，使](https://patchwork.kernel.org/project/qemu-devel/list/?series=391797)成为必要的管理程序框架[为 QEMU 代码库打补丁](https://patchew.org/QEMU/20201130030723.78326-1-agraf@csgraf.de/)，以便在 M1 MAC 电脑上以访客身份运行 Linux 和 Windows。我们现在处于几乎所有基本功能，包括虚拟化音频和网络接口都可以工作的阶段。更有趣的是，由于 ARM64 仿真层的 [WoW，为 x86 架构构建的传统 Win32 应用程序在访客 Windows 10 虚拟机上运行良好。](https://www.xda-developers.com/microsoft-qualcomm-and-intel-the-windows-10-arm-dustup/)

几个开发者联合起来修复剩余的错误，使[安装过程](https://gist.github.com/niw/e4313b9c14e968764a52375da41b4278#file-readme-md)更加[用户友好](https://github.com/KhaosT/ACVM)。在你的 Apple Silicon Mac 上安装 Linux 或 Windows 10 的[虚拟化实例并不会移除其上安装的主操作系统，所以你不需要担心破坏任何东西。如果你想通过 QEMU 在你闪亮的新 ARM Mac 上开始使用 Windows 10，请查看下面的视频教程。](https://twitter.com/jonmasters/status/1333541297563586561)

然而，在我们看到 Windows 或 Linux 在 ARM Macs 上本机启动之前，仍然有很大的障碍。根据 Linux 创建者 Linus Torvalds 的说法，M1 SoC 中集成的 GPU 和其他组件的封闭性使得移植过程有点复杂...除非苹果开放”。虽然苹果[不打算在基于 M1 的 MAC 电脑](https://www.youtube.com/watch?v=Hg9F1Qjv3iU)上支持 Boot Camp，但对于那些喜欢苹果的构建质量但不想局限于 macOS 的人来说，在一个节能但极其强大的 ARM 平台上运行 Linux 或 Windows 的想法是非常有趣的。我们肯定会密切关注修改场景，看看这些开发进展如何，并希望它最终如何有利于计算领域从 x86 到 ARM 的过渡阶段。