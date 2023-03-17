# Ubuntu 20.10 Groovy Gorilla 更新将 Ubuntu 桌面带到了树莓派

> 原文：<https://www.xda-developers.com/ubuntu-20-10-groovy-gorilla-raspberry-pi-support/>

Canonical 已经宣布发布 Ubuntu 20.10，又名“Groovy Gorilla”。这个版本中的大新闻是一个新的优化堆栈，它将 Ubuntu 桌面和服务器带到了 Raspberry Pi 范围。自 2019 年推出 [Raspberry Pi 4](https://www.xda-developers.com/raspberry-pi-4-upgraded-cpu-4gb-of-ram-dual-4k-displays/) 以来，小型电脑系列越来越多地被用作桌面替代品，而最大的 Linux GUI(当然，Android 除外)定制版的到来是这条道路上的重要一步。

Canonical 首席执行官马克·舒托沃尔斯表示:“在这次发布中，我们庆祝树莓派基金会致力于将开放计算交到全世界人民的手中。“*我们很荣幸通过在 Raspberry Pi 上优化 Ubuntu 来支持这一计划，无论是用于个人用途、教育目的，还是作为他们下一次商业冒险的基础。*

Ubuntu 20.10 也可以在 RP 2 和 RP 3 版本上运行，但只能使用 4GB 或更高的内存——如果你的内存低于这个数字，你可能会得到平稳的安装，但会有一些问题。您还将看到对具有屏幕键盘模式的 2 合 1 设备的支持得到了改善，并且更多各种外形的设备现在都支持 Linux 下的指纹读取器。

Raspberry Pi Trading 首席执行官 Eben Upton 表示:“从经典的 Raspberry Pi 板到工业级计算模块，这是在 Raspberry Pi 上实现 Ubuntu LTS 并提供长期支持和安全更新的第一步，符合我们扩大最佳计算和开源功能的承诺。

对于更高级的用户，边缘按需计算通过“微云”堆栈获得了巨大的推动，该堆栈结合了 MAAS、LXD、MicroK8s 和 Ceph，为从人工智能到智能城市管理的各种用例提供了轻量级、低姿态的云实例。

Ubuntu 20.10 现已推出，对大多数用户免费，有桌面、服务器、云和物联网的镜像，以及专用的 Raspberry Pi build，可从 [Ubuntu 网站](https://ubuntu.com/download)下载。

### Ubuntu 20.10 新特性

## Ubuntu 20.10 上的更新包

**Linux 内核**

Ubuntu 20.10 包含了 **5.8** Linux 内核。这包括自 Ubuntu 20.04 LTS 版发布 5.4 Linux 内核以来的大量更新和新增支持。一些值得注意的例子包括:

*   更好的 WiFi 连接质量的通话时间队列限制
*   Btrfs RAID1，具有 3 个和 4 个副本以及更多校验和选项
*   添加了 USB 4(雷电 3 协议)支持
*   默认情况下，X86 启用 5 级分页支持
*   英特尔第 11 代(冰湖)和第 12 代(老虎湖)显卡支持
*   对 AMD 系列 19h (Zen 3)的初始支持
*   用于系统的热压跟踪，以便在 CPU 内核上更好地放置任务
*   XFS 在线维修
*   OverlayFS 与 VirtIO-FS 配对
*   用于密钥/密钥环通知、安装更改等的通用通知队列。
*   主动状态电源管理(ASPM ),提高 PCIe 到 PCI 设备的节能效果
*   对 POWER10 的初始支持

**工具链升级**

Ubuntu 20.10 带有更新的最先进的工具链，包括 glibc 2.32、OpenJDK 11、rustc 1.41、GCC 10、LLVM 11、Python 3.8.6、ruby 2.7.0、php 7.4.9、perl 5.30、golang 1.13 的新上游版本。

**安全改进**

nftables 现在是防火墙的默认后端。

**Ubuntu 桌面**

Ubuntu 20.10 是第一个为树莓 Pi 4324提供[桌面图像的 Ubuntu 版本。](https://ubuntu.com/raspberry-pi/desktop)

**侏儒**

Ubuntu 20.10 包括 GNOME 的最新版本 3.38，具有增强的活动概述、用户体验改进、更好的性能等等。

**更新的应用程序**

*   火狐 81 版
*   库版本 7.0.2
*   雷鸟版本 78.3.2

**更新子系统**

*   BlueZ 5.55
*   网络管理器