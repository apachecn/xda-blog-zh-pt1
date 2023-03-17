# 设备映像生成器允许您为您的 PC 制作 Windows 10X 映像

> 原文：<https://www.xda-developers.com/windows-10x-device-image-generator/>

# 此工具可让您轻松地为您的电脑制作 Windows 10X 映像

设备映像生成器是一个方便的工具，可以让您集成驱动程序，并为您的 PC 构建一个完整的 Windows 10X 映像。请继续阅读！

Windows 10X 开始菜单

微软的 Windows 10 操作系统享有桌面操作系统市场的最大份额，因为它可以安装在几乎任何现代 x86 PC 上。然而，Windows 10X 是微软操作系统的独特风格，最初是专为可折叠和双屏设备设计的，但后来被重新设计为专注于单屏电脑。有趣的是，整个 Windows 10X 架构与普通的 Windows 10 截然不同。没有通用的安装程序，因为微软不打算让最终用户在他们的电脑上安装这个变种。如果你[已经看到了重新制作的 UI](https://www.xda-developers.com/microsoft-windows-10x-hands-on-details/) ，并且想要马上在你的电脑(或者你最喜欢的虚拟化平台)上体验一下，那么你会很高兴地知道一个独立的开发者已经发布了一个名为“设备映像生成器”的工具来简化创建 Windows 10X 映像的过程。

设备映像生成器由 Twitter 用户*[@ the book disclosed](https://twitter.com/thebookisclosed)*创建，旨在成为一个简单方便的实用程序，为通用 x86 PC 生成当前可用的 Windows 10X 版本的全功能[全闪存更新(FFU)包](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/wim-vs-ffu-image-file-formats)。用户现在可以选择从 Windows 10 的现有实例中导出所有需要的驱动程序，并将它们注入到基础映像中，而不是使用 CLI 工具。

此外，该实用程序会自动创建一组构建最终映像所需的配置包。请记住，设备映像生成器不会下载 Windows 10X 版本的统一更新平台(UUP)文件集，因此用户必须提前[获取它们](https://github.com/gus33000/UUPMediaCreator)。

您可以从下面的链接下载设备图像生成器。下载完成后，解压 7Z 文件的内容并启动 DevImgGen.exe。

**[下载 Windows 10X 设备镜像生成器](https://twitter.com/thebookisclosed/status/1356172974353768448)**

值得注意的是，该工具被标记为“beta”，这意味着不能保证它能有效地为硬件组件模糊的 PC 构建映像。此外，Windows 10X 本身还没有达到 RTM 阶段，所以一旦你在 PC 上安装了该操作系统，预计会出现一些随机错误。