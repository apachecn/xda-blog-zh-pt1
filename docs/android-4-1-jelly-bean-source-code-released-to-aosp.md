# 2023 年最受欢迎的 Android 定制内核

> 原文：<https://www.xda-developers.com/android-4-1-jelly-bean-source-code-released-to-aosp/>

安卓智能手机市场有大量的选择。由于 Android 生态系统对开发者友好，除了原始设备制造商提供的选项之外，还有无数选项可以定制和修改您的手机。由于 Android 在其核心使用 Linux 内核，内核源代码是繁荣的售后社区的基石之一，允许开发人员构建自定义内核、[rom](https://www.xda-developers.com/most-popular-custom-roms-android/)等等。

请记住，你不能只拿着[主线 Linux 内核](https://www.xda-developers.com/oneplus-6-6t-mainline-linux-kernel-support/)就指望它在你的 Android 设备上启动。谷歌有一个用于 Android 的[通用内核树](https://android.googlesource.com/kernel/common/)，像高通这样的 SoC 制造商利用这棵树并在此基础上构建他们的补丁。接下来是原始设备制造商，他们从 SoC 制造商那里获得树，然后在此基础上开发特定的硬件补丁。

由于这种设计，创建一个定制的 Android 内核并不是一件简单的工作。开发人员需要获取特定于设备的源代码，清理所有的调试符号，添加额外的功能，(可选地)从较新的内核版本反向移植特性，最后将所有东西打包到一个 flash 包中。

由于内核对系统有完全的控制权，所以为你的 Android 设备选择一个合适的定制内核是很重要的。下面你可以为几款[流行的安卓手机](https://www.xda-developers.com/best-android-phones/)找到一些安卓售后开发场景中最流行的定制内核。与普通内核相比，这些定制内核不仅提供了更长的电池寿命和更高的性能，而且在社区中以其稳定性和安全性而闻名。

**注意:**定制内核生态系统是关于知识共享的。许多开发人员进行了广泛的研究，以修复 OEM 提供的源代码中的缺点并实现新功能，这些新功能随后被用于跨不同设备的售后内核项目中。在本文中，我们将只强调几个正在积极维护并可用于多种设备的定制内核。这并不意味着对这一特定核心的认可，也不是说其他人的工作应该被忽视。我们只是限制我们链接的内容，以防止这篇文章变得太长。请访问您的设备的 XDA 论坛，看看是否有其他可能更通用、功能更丰富的内核可用。

* * *

## 苏丹仁

如果你曾经拥有过最初几代一加设备中的一款，并考虑过对它进行改造，那么你很有可能见过 XDA 公认的开发者 Sultanxda 的作品。虽然开发者目前不支持当前一代旗舰设备，但他仍在为[谷歌像素 4](https://forum.xda-developers.com/t/4219247/) 和[谷歌像素 4 XL](https://forum.xda-developers.com/t/4219243/) 维护名为 Sultan Kernel 的定制内核。

与典型的定制内核不同，Sultan 内核并不是由用户定制的。更确切地说，它通过引入几个底层增强功能，将自己表现为股票内核的真正替代品。它的许多功能，如名为[简单 LMK](https://github.com/kerneltoast/simple_lmk) 的定制低内存杀手，用于改善图形和整体性能的 Devfreq boost 驱动程序，[安全网引导加载程序解锁检查旁路](https://www.xda-developers.com/sultanxda-bypasses-new-safetynet-unlocked-bootloader-check-on-latest-cm13-builds-for-op3/)，以及许多其他功能都通过精选找到了其他定制内核项目的方法。

* * *

## arter97 Kernel

Juhyung Park，又名 XDA 认可的开发人员 [arter97](https://forum.xda-developers.com/m/arter97.4898097/) 因其在众多设备的定制内核方面的工作而在社区中闻名。arter97 自定义内核以其论坛句柄命名，对 OEM 内核进行了多项改进，包括来自高通的比常规标签更先进的变化，完全中立的 OEM“优化”，更好的 TCP 网络拥塞控制等。

**[访问 arter97 内核官方下载入口](https://arter97.com/browse/)**

如果你的智能手机支持 arter97 内核，那么你应该在相应的设备分论坛找到官方支持线程。

* * *

## 元素 x 内核

ElementalX 定制内核项目是 XDA 知名开发者 [flar2](https://forum.xda-developers.com/member.php?u=4684315) 的创意。内核不仅为提供更长的电池寿命进行了优化，而且还提供了许多定制功能，以最大限度地调整设备的性能。ElementalX 支持的各种设备上常见的一些功能有唤醒手势、Adrenoboost 选项、高级颜色控制、常规上游和 CAF 修复。

**[访问 ElementalX 内核](https://elementalx.org/)官网**

在我们的论坛上有活跃的支持线程，如果有错误，你可以联系开发人员本人，或者联系其他社区成员以获得最佳调整。开发人员还提供了一个名为“EX 内核管理器”的专用配套应用程序，用于定制内核参数。

[app box Google play " flar 2 . exkernelmanager "]

* * *

## blu_spark 内核

blu_spark 由 XDA 资深会员 [eng.stk](https://forum.xda-developers.com/m/eng-stk.3873953/) 维护，以其稳定性和高效性成为一加社区最著名的内核之一。开发者还将这个内核移植到了谷歌 Pixel 4a 上，并带来了相同的优化，包括高级颜色控制、 [WireGuard VPN](https://www.xda-developers.com/google-adds-wireguard-vpn-android-12-linux-kernel-5-4/) 支持等等。

如前所述，blu_spark 内核可用于几款一加智能手机。前往[开发者的 GitHub 简介](https://github.com/engstk)查看它是否适用于你的设备。官方支持线程也可以在 XDA 的设备相关论坛。最后但同样重要的是，内核提供了与著名的 Franco 内核管理器应用程序的集成，因此您可以获得自动更新程序以及调整各种内核参数的好方法。

[app box Google play " com . Franco . kernel "]

* * *

## 桐樱仁

XDA 公认的开发者 Freak07 已经提出了 Kirisakura 定制内核，目的是通过保持大多数子系统更新来产生一个适当的库存内核的替代品。无论是安全爱好者想要的[内核控制流完整性(Kernel-CFI)](https://www.xda-developers.com/kirisakura-custom-kernel-for-the-oneplus-8-pro-enables-control-flow-integrity-cfi-for-better-security/) ，还是满足您所有游戏需求的最新 CAF-State GPU 驱动程序，Kirisakura 内核都能满足您的需求。

查看你的设备的 XDA 论坛，看看这个令人敬畏的内核是否适用于你的设备，如果是，你可以开始更新和调整它。

* * *

## 荣誉提及:擎天柱醉仁

作为地面零开源项目的一个组成部分，Optimus Drunk 内核可用于一系列设备——包括新的和旧的——并具有许多优化和特性。您可以获得 WireGuard VPN、粒度颜色控制、对唤醒锁阻止的支持，以及这个自定义内核的更多功能。

XDA 认可的开发商 [GtrCraft](https://forum.xda-developers.com/m/gtrcraft.5293805/) 正在为各种设备维护 Optimus Drunk 内核，并为你对他们的 XDA 线程的大部分疑虑提供支持。一定要为你的智能手机检查一下。

* * *

安装一个定制内核通常很简单，只需下载特定于设备的包，并通过像 [TWRP](https://www.xda-developers.com/how-to-install-twrp/) 这样的定制恢复来刷新它。现在去看看我们的论坛，找出最适合你的设备的定制内核！