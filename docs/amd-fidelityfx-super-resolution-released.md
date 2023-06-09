# AMD FidelityFX Super Resolution 是一款开源 DLSS，现已上市

> 原文：<https://www.xda-developers.com/amd-fidelityfx-super-resolution-released/>

到目前为止，你可能已经对 DLSS 有所耳闻。深度学习超级采样的简称，是英伟达为其 GeForce RTX GPU 推出的一项技术，它允许游戏通过升级以更高的分辨率运行。它只在某些 NVIDIA GPUs 上可用，但现在，AMD 终于推出了自己的版本。AMD FidelityFX 超分辨率(FSR)从今天开始[可用，它本质上是一个更开放的 DLSS 版本。](https://www.amd.com/en/press-releases/2021-06-22-amd-fidelityfx-super-resolution-amd-brings-high-quality-high-resolution)

如果你不熟悉它，DLSS 是 Nvidia GeForce GPUs 上独有的张量核心。这些是针对机器学习处理而优化的特定处理器，用于处理给定图像在不同分辨率下的外观。通过这种方式，GPU 上的光栅化核心可以以较低的分辨率渲染游戏，张量核心可以将其转换为较高质量的版本。这使得游戏看起来更好，同时降低了对整体性能的影响。

AMD 的版本在概念上类似。该公司表示，FSR 使用边缘重建算法来分析原始图像，并确定它应该如何看待目标分辨率。然后，它使用锐化过程来增强纹理中的细节，并生成更好看的图像。FSR 有四种模式:超高质量、高质量、平衡和高性能。每个选项之间的变化是原生渲染分辨率。例如，如果你在 4K 玩，Ultra Quality 会以 2954 x 1662 的分辨率渲染游戏，然后升级到 4K。如果您选择性能，游戏将在升级之前以 1920 x 1080 或全高清进行渲染。

AMD FSR 最值得注意的一点是，它的可用性明显比英伟达的 DLSS 更广泛。FSR 支持 DirectX 11、DirectX 12 和 Vulkan 游戏，它可以在 100 多种 AMD 产品上运行。这包括镭龙 RX GPUs，一直到镭龙 RX 460，甚至是集成显卡的锐龙处理器。此外，它也可以在 NVIDIA 的显卡上工作，尽管 AMD 不为这些情况提供技术支持。

AMD [FidelityFX 超分辨率](https://www.amd.com/en/technologies/radeon-software-fidelityfx-super-resolution)今天在七款游戏中可用，包括 *22 Racing* 系列、 *Anno 1800* 、*邪恶天才 2* 、 *Godfall* 、 *Kingshunt* 、*终结者:反抗*、*裂土者*。不过，更多的游戏已经在计划中，包括*生化危机:村庄*、*孤岛惊魂 6* 和*for speken*。AMD 表示，已经有超过 40 家游戏开发商承诺支持这项技术，因此应该会有更多的游戏问世。您需要[下载最新的镭龙驱动程序](https://www.amd.com/en/support)才能启用该功能。今年 7 月，该驱动程序也将在 GPUOpen 上提供给任何人使用。