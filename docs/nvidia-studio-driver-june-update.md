# NVIDIA 的 Canvas 应用程序将你的涂鸦变成照片般逼真的绘画

> 原文：<https://www.xda-developers.com/nvidia-studio-driver-june-update/>

今天，NVIDIA 宣布了一系列面向创意专业人士的改进和新工具。新闻包括一个新的基于人工智能的应用程序，名为 Canvas，一个新的 NVIDIA GPUs 工作室驱动程序，新的 Adobe 应用程序和新的工作室笔记本电脑。

NVIDIA Canvas 应用程序可能是当天最有趣的[公告之一。它基于 NVIDIA 已经测试了一段时间的 GauGAN 项目，它本质上是实时将涂鸦变成照片级的绘画。NVIDIA 表示，用户用材料而不是颜色来绘画，当他们涂鸦时，他们使用的元素会转化为现实版的材料。这使得艺术家可以快速将他们对某个设计的想法可视化，或者快速为一个更大的项目奠定基础。该应用程序还支持图层，因此每个元素都是图像的一个独立部分。最终结果可以导出为. PSD 文件，以便在 Adobe Photoshop 中进一步编辑。](https://blogs.nvidia.com/blog/2021/06/23/studio-canvas-app/)

根据一天中的时间和光线等因素，有九种风格可以改变最终画作的外观。绘图时还有 15 种材质可供选择，如天空、山、水等等。主要目标是帮助创建景观图像，可以快速作为其他东西的基础。NVIDIA Canvas 是 NVIDIA Studio 的一部分，它包括其他创作工具，如 NVIDIA Broadcast 和 Omniverse。你可以[在这里下载测试版的应用程序](https://www.nvidia.com/en-us/studio/canvas/),看看它能做什么。

## 6 月 NVIDIA 工作室驱动程序

转到新的 NVIDIA Studio 驱动程序，它有一些改进。可调整大小栏是一种允许 CPU 一次访问更多 GPU 内存的功能。传统上，CPU 必须以 256MB 为单位访问 GPU 内存，但有了这一功能，它们可以根据需要访问整个帧缓冲区。这是不久前在 NVIDIA 的 GeForce [游戏就绪驱动](https://www.xda-developers.com/nvidia-resizable-bar-available-all-rtx30-gpus/)中添加的，但现在它也可以在工作室驱动中使用。它减少了 CPU 从 GPU 访问大块信息时必须发出的连续请求的数量，这意味着大大减少了开销。

另一个新功能是动态增强 2.0。这项技术平衡了笔记本电脑上 CPU、GPU 和 GPU 内存之间的电源管理，有助于提高性能和效率。现在，这项技术已经针对创意应用进行了优化，因此当需要更多 GPU 能力时，可以在那里分配，而 CPU 获得的能力较少。该驱动程序还增加了对 GeForce GPUs 虚拟化的支持。这意味着 Linux 用户可以为 Windows 虚拟机启用 GPU passthrough，如果你既想使用 Linux，又想运行 GPU 密集型的 Windows 应用和游戏，这是一个好消息。

该驱动程序还提高了一些 3D 渲染器的性能，包括 Blender。NVIDIA 表示，使用新的驱动程序，运动模糊渲染速度可以提高 41%。NDI 5 还增加了对英伟达解码的支持，使其能够以每秒 120 帧的速度播放和录制高达 4K 的视频。总而言之，新的驱动程序为十种不同的应用程序带来了优化的性能。

在这些应用程序中，还有 Adobe Substance tools 的新套件，它也有所扩展。有一个新的 Substance 3D Stager 应用程序用于渲染和照明 3D 场景，它支持实时光线跟踪，你可以在上面的操作中看到它。还有一个新的 Substance 3D Modeler 应用程序处于测试阶段，允许用户创建和组合 3D 模型，基于 Vulkan APIs 构建。其他物质应用程序——Designer、Painter 和 3D Sampler(以前称为 Alchemist)——都针对 RTX GPU 进行了优化。

最后，英伟达还强调了一堆最近推出的带有英伟达 GPU 和工作室驱动程序的工作室笔记本电脑。其中包括[联想 ThinkPad P1 第 4 代](https://www.xda-developers.com/lenovos-thinkpad-p1-gen-4-still-thin-powerful/)、P15 和 P17 第 2 代，新[戴尔 XPS](https://www.xda-developers.com/dell-xps-15-xps-17-come-with-11th-gen-processors-rtx-30-graphics/) 和 Inspiron 笔记本电脑，以及[宏碁 ConceptD](https://www.xda-developers.com/acer-conceptd-notebooks-creators-3d-display/) 笔记本电脑和台式机。