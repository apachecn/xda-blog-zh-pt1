# Windows 11 虚拟机将需要 TPM 2.0

> 原文：<https://www.xda-developers.com/windows-11-vms-will-likely-soon-require-tpm-2-0/>

随着 [Windows 11](https://www.xda-developers.com/windows-11/) 中所有系统需求的增加，其中一个更突出的需求是 TPM 2.0。然而，如果你在虚拟机上安装新的操作系统，这一要求将被取消，允许你在不受支持的硬件上测试它，以及在苹果的 M1 MAC 电脑上运行它。

这种情况将会改变。昨天，微软[向 Dev 频道发布了 Windows 11 build 22458](https://www.xda-developers.com/microsoft-releases-windows-11-build-22458-to-the-dev-channel-with-fixes/) ，当时，changelog 只包括一些修复和微小的变化。今天，[的博文](https://blogs.windows.com/windows-insider/2021/09/15/announcing-windows-11-insider-preview-build-22458/)进行了更新，以反映 TPM 2.0 现在是虚拟机的一项要求。

今天晚些时候，微软在测试频道发布了一个新的 Windows 11 累积更新，这也将点亮 TPM 的要求。这意味着当 Windows 11 于 10 月 5 日发布时，TPM 2.0 仍将是一项要求，即使你试图在虚拟机中运行它。

微软表示，如果你用 ISO 安装新的操作系统，而不是通过 Windows Update，你将能够绕过新的系统要求。唯一的问题是，这可能会使您处于不受支持的状态。该公司表示，如果你用这种方法安装新的操作系统，你可能得不到更新。

TPM 代表可信平台模块，自 2016 年年中以来，它一直是所有新 Windows 10 电脑的要求。正因为如此，在裸机硬件上安装 Windows 11 通常不是一件坏事。对英特尔第八代或更新的 CPU 的要求是更大的问题，因为理论上，任何新的都应该已经有 TPM 2.0。

在 Windows 上，你需要在 Hyper-V 中创建第二代虚拟机。如果你在 Mac 上使用 Parallels，你仍然会很好，即使微软说[它在技术上是一个不受支持的用例](https://www.xda-developers.com/microsoft-wont-support-windows-11-m1-macs/)。Parallels 配备了虚拟 TPM，最新版本旨在正式支持 Windows 11。无论您使用什么解决方案，您都需要某种 TPM 支持。