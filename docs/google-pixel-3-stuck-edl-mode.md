# 一些 Pixel 3 设备停留在 EDL 模式，没人知道为什么

> 原文：<https://www.xda-developers.com/google-pixel-3-stuck-edl-mode/>

Pixel 3 系列于 2018 年 10 月推出，所以它并没有那么老，当然也没有老到让人不得不担心随机硬件故障的地步。然而，越来越多的 Pixel 3 和 Pixel 3 XL 用户报告称，他们的设备陷入了紧急下载(EDL)模式。EDL 模式是配备高通芯片组的移动设备上提供的一种低级恢复模式，用于在设备无法启动时刷新软件。手机突然进入 EDL 模式表明该设备有严重问题，无法正常启动，而这似乎正在这里发生。

关于这个问题的报道堆积在[谷歌的问题跟踪器](https://issuetracker.google.com/issues/192008282)、[支持论坛](https://support.google.com/pixelphone/thread/113517096/pixel-3-xl-bricked-overnight-computer-recognizes-as-qusb-bulk-cid-likely-caused-by-security-update?hl=en)和[Reddit](https://www.reddit.com/r/GooglePixel/comments/mmcn93/my_pixel_3_xl_bricked_overnight/)(via[*ArsTechnica*](https://arstechnica.com/gadgets/2021/09/reports-of-pixel-3s-bricking-with-edl-message-are-growing/))上。这让人想起了 Nexus 5X 和 Nexus 6P，这两款设备在过去都存在无法启动的问题。在这些情况下，[有可能](https://www.xda-developers.com/nexus-5x-bootloop-fix-boot-phone/)到[通过安装修改后的引导镜像来恢复手机](https://www.xda-developers.com/nexus-6p-bootloop-fix/)，但是在这种情况下，还没有发现这样的修复。

由于 EDL 模式旨在闪现特殊类型的图像，而不是谷歌发布的常规“快速启动”包，目前没有办法从这种模式中恢复 Pixel 3 或 3 XL。诊断问题也很困难:一些谷歌人在支持线程中请求 Android 生成的错误报告，但一直被搁置，因为用户无法在没有可用手机的情况下获得这些报告。

要在 EDL 模式下恢复设备的出厂固件，您需要 NAND 映像和 QPST，或者高通产品支持工具。即使获得了 Pixel 3 和 3 XL 的正确文件，也不能保证导致这些设备进入 EDL 模式的问题会通过工厂恢复得到解决。当检测到严重故障，导致手机无法启动时，装有高通芯片的手机可能会启动到 EDL 模式，这意味着正确的文件甚至可能不会闪存，或者即使闪存，手机也可能无法启动。

目前还不清楚这个问题的根本原因是什么，尽管 Pixel 3 和 3 XL 并不是第一批面临硬件问题的 Pixel 手机。例如，由于电源和充电问题，Pixel 4 XL 最近的保修期延长了一年。如果谷歌在调查问题后发布声明，我们一定会更新这篇文章。