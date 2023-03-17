# 你现在可以通过 Hangover 在 ARM 上的 Windows 10 上运行一些 x86-64 的 Windows 应用

> 原文：<https://www.xda-developers.com/x86-64-windows-app-windows-10-arm-hangover/>

如果你从周末醒来，带着严重的宿醉，你可以从良好的宿醉中得到安慰。运行 PowerPC 或 ARM64 设备的设备用户们，欢呼吧——你们的祈祷得到了回应，由于 Hangover 的最新 Alpha 版本，你们现在可以在自己的机器上运行一系列 Windows x86/x64 应用程序了。对于外行人来说，Hangover 是一个基于 WINE 的虚拟化平台，最初是为了探索在 64 位 ARM 驱动的设备和基于 x86 的同类设备之间创建兼容性的方法而建立的。现在，由于与 Raptor Computing Systems 的合作，它正在使用该技术为 PowerPC 创建类似的解决方案(通过 [*Phoronix*](https://www.phoronix.com/scan.php?page=news_item&px=Hangover-Alpha-2) )。

该解决方案通过在主机上运行 WINE 64 位、一个经过特别调整的 QEMU 实例和一大堆“thunk”库来实现。结果是你最喜欢的 Windows 应用程序的虚拟化版本——尽管这种承诺伴随着大量的警告。

虽然进展仍在进行中，但它已经可以做很多事情了，甚至基本的 3D 渲染和 Direct3D，如果你安装了 OpenGL 的话。然而，如果你需要一些你可以依赖的 Windows 应用程序，这真的不适合你。也许有一天会实现，但开发者自己承认，这是一个非常初级的初级产品，还不能作为 Windows 原生 PC 的替代品。Hangover 现在允许 Windows x86/x64 应用程序在 ARM 64，PPC64LE，x86_64 上运行-但都非常“理论上”-你的结果可能会有所不同。用户可能会注意到 [Android 支持](https://www.xda-developers.com/wine-windows-compatibility-layer-android-version-5-0/)在这个版本中被移除了。这可能会令人失望，但它已经有一段时间没有正常工作了，似乎开发者已经决定在现在和可预见的未来禁用它。

要了解更多信息，并下载 Hangover Alpha，[单击此链接](https://github.com/AndreRH/hangover/releases/tag/hangover-0.5.15)进入 GitHub 资源库。