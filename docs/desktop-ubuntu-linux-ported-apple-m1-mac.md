# Linux 现在可以在装有苹果芯片的 Mac Mini 上运行

> 原文：<https://www.xda-developers.com/desktop-ubuntu-linux-ported-apple-m1-mac/>

自从苹果公司推出搭载该公司新的高性能 ARM 芯片的新款 MAC 电脑以来，第三方软件开发商一直在努力开发替代操作系统，并在新的硬件上运行。上个月初，一些开发人员[通过虚拟化在 M1 的 Mac 电脑上启动了 Windows 10 和 Fedora Linux](https://www.xda-developers.com/apple-silicon-mac-boot-windows-10-and-linux-virtualization/) ，但是 M1 Mac 电脑替代操作系统开发的最大突破来自 Corellium 的团队，Corellium 是一家专门从事 ARM 设备虚拟化的公司。该团队已经成功移植了 Linux，并使其在 M1 Mac Mini 上“完全可用”。

在一篇博客文章中，Corellium 展示了他们如何将 Linux 移植到新的 MAC 电脑上。该公司利用其开发 Sandcastle 项目的经验——该项目[能够在容易受到 checkm8 漏洞攻击的旧 iphone](https://www.xda-developers.com/install-android-10-apple-iphone-7-plus-project-sandcastle-checkra1n-jailbreak/)上引导 Android 为新的苹果 SOC 编写 Linux 驱动程序。幸运的是，苹果官方允许在苹果硅 MAC 上引导定制内核，所以没有必要利用漏洞来引导未签名的内核。不涉及本质细节——[Corellium 的博客文章](https://corellium.com/blog/linux-m1)在这方面做得很好——苹果芯片的固件接口和启动过程与其他 64 位 ARM SoCs 相比非常不同。通过一点工作，Corellium 团队设法增加了对足够硬件接口的支持，以便在 M1 Mac Mini 上启动 Ubuntu Linux。

在 M1 MAC 电脑上启动 Linux 所需的补丁记录在[这里](https://github.com/corellium/linux-m1)，而启动处理器内核所需的预加载程序的源代码可以在[这里](https://github.com/corellium/preloader-m1)找到。变更[已经被推向上游](https://lkml.org/lkml/2021/1/20/481)，尽管在代码合并之前还需要做更多的工作。幸运的是，Linux 社区的其他成员正在努力支持 M1 MAC 上的 Linux。最值得注意的是，[众筹的朝日 Linux 项目](https://asahilinux.org/)——旨在将 Arch Linux 移植到苹果硅 MAC 电脑——背后的团队[正在对 GPU 架构](https://rosenzweig.io/blog/asahi-gpu-part-1.html)进行逆向工程，以实现硬件加速。为了在 M1 MAC 电脑上直接启动 Linux，使用 PongoOS 作为引导程序的工作正在进行中。

如果你有兴趣在你自己的 M1 Mac Mini 上试用 Linux，Corellium 分享了如何启动 Ubuntu 的指导。你可以在这里找到完整的说明，但总的来说，你需要下载他们的实时映像(对 Raspberry Pi 的 ARM64 Ubuntu 版本略有修改)，将映像复制到外部 USB 驱动器(容量至少需要 16GB)，将 USB 驱动器连接到 Mac Mini 的 USB-C 端口，启动到恢复操作系统，安装自定义内核(Corellium 提供了一个设置脚本)，然后使用默认凭据登录。

正如你所看到的，安装过程不是很用户友好，所以不建议初学者在他们的 Mac Mini 上摆弄 Linux。此外，没有 GPU 加速或支持 M1 的机器学习核心，所以不要指望玩游戏或运行 ML 任务。尽管如此，这对任何对 PC 硬件和 Linux 感兴趣的人来说都是令人兴奋的消息。苹果硅 MacBooks 的性能和电池寿命是首屈一指的，因此这些机器将是移动编程的完美选择。甚至连莱纳斯·托沃兹也同意。