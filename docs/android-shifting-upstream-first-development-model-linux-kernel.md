# Android 转向“上游优先”模式，支持新的 Linux 内核特性

> 原文：<https://www.xda-developers.com/android-shifting-upstream-first-development-model-linux-kernel/>

当你在同一句话里看到“Android”和“碎片化”这两个词的时候，你的脑海里很可能立刻跳转到 [Android 版本分布图](https://www.xda-developers.com/android-version-distribution-statistics-android-studio/)。当大多数人抱怨 Android 操作系统更新全面推出缓慢时，他们会指责一些实体，但谷歌能做的只有这么多，以迫使*OEM 厂商更快地开发和推出更新。然而，谷歌能做的是减少开发时间，从而降低更新的成本。*

谷歌减少开发负担的长期项目中的第一个重大举措是项目三倍。该项目于 2017 年与 Android 8.0 Oreo 一起发布，通过将操作系统框架与供应商实现(HALs 和特定于设备的 Linux 内核分叉)分离，实现了三重模块化 Android。这使得 Android OEMs 厂商更容易在最新的 AOSP 框架上重新构建他们的操作系统，因为他们可以启动最新版本，而不需要从供应商那里更新代码。因此，原始设备制造商可以比以前更快地准备好他们的定制 Android 分支，进而更快地推出主要的操作系统更新。

谷歌计划的下一步是简化 Android 关键组件的更新交付。谷歌在 2019 年推出 Android 10 时，将这一举措称为项目主线。谷歌实际上控制了关键的操作系统组件，并禁止原始设备制造商修改它们。然后，他们通过 Google Play 建立了一个交付机制，这样他们就可以远程发布这些关键组件的更新，而不必等待原始设备制造商自己应用补丁。Mainline 大大提高了设备接收重要操作系统组件更新版本的速度，从而提高了整个 Android 生态系统的安全性。

但接下来的事情更加重要，可以说是谷歌长期战略中最重要的部分。当我们早些时候指出如何通过将操作系统框架从供应商实现中分离出来使 Android 模块化时，我们将“特定于设备的 Linux 内核分叉”作为供应商代码的一部分。任何熟悉桌面上的 Linux 的人都会意识到一个问题:为什么它和闭源供应商的代码混在一起？问题是，虽然 Android 设备确实搭载了 Linux 内核，但该内核有大量的树外代码。

我们是如何到达那里的？正如谷歌软件工程师托德·乔斯(Todd Kjos)在今年的 Linux 管道工会议(通过 [*ArsTechnica*](https://arstechnica.com/gadgets/2021/09/android-to-take-an-upstream-first-development-model-for-the-linux-kernel/) )上概述的那样，这个问题是因为主线 Linux 内核在装载到 Android 设备上之前被分叉了几次。Google 将每个主线 Linux 内核分成一个“ [Android Common Kernel](https://source.android.com/devices/architecture/kernel/android-common) ”分支，该分支密切跟踪主线版本，但添加了一些特定于 Android 的补丁。像高通、联发科和三星这样系统芯片供应商为他们生产的每一个系统芯片分配内核。然后，原始设备制造商采用特定于 SoC 的内核，并添加额外的补丁，以实现对他们想要发运的特定硬件的支持。

根据谷歌的说法，由于这些变化，“在设备上运行的多达 50%的代码是树外代码(不是来自上游的 Linux 或 AOSP 通用内核)”。这些设备上的大量树外代码使得合并上游变更成为一个漫长而具有挑战性的过程。这对设备安全是有害的，因为原始设备制造商需要更加努力地对 Linux 内核中发现的漏洞实施补丁。此外，这使得大多数 Android 设备仍然使用多年前发布的内核，这意味着它们错过了新的 Linux 内核特性。

为了解决这个问题，Google 正在开发 Android 通用内核映像(GKI ),它本质上是一个直接从 ACK 分支编译而来的内核。GKI 将 SoC 供应商和 OEM 定制隔离到插件模块，消除了树外代码，并允许 Google 将内核更新直接推送到最终用户。一年多来，谷歌一直致力于通过 Play Store、[使用主线模块](https://android-review.googlesource.com/c/platform/system/extras/+/1371347)来发布 GKI 更新。

根据我们的消息来源，搭载 Android 12 和 Linux 内核 5.10 的设备必须部署谷歌签名的启动映像。谷歌自己的 [Pixel 6](https://www.xda-developers.com/google-pixel-6/) 系列将推出开箱即用的 Android 12，并搭载 Linux 内核 5.10，因此这两款手机可能是首批搭载 GKI 的大众市场设备。

此外，谷歌的 Todd Kjos 透露，该公司计划为新的 Linux 内核功能转向“上游优先”的开发模式。这将有助于谷歌确保新代码首先登陆主流 Linux 内核，这将减少未来更多的树外代码登陆 Android 设备所产生的技术债务。

在本周的 Linux 管道工会议上，Kjos 说，*“由于树外模块对我们的用例非常重要，我们希望我们总是会有一组导出和一些不同的东西，或者除了上游的东西之外，但这整个项目是一个多年的项目，致力于尽可能多地消除树外补丁，并尽可能地与上游保持一致。”*谷歌的目标是在 2022 年底前完成现有功能的上游化和隔离供应商变化的工作，从 2023 年开始，该公司计划采用这种“上游优先”的开发模式，以避免未来出现此类问题。