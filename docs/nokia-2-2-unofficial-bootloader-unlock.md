# 头盔显示器全球的诺基亚 2.2 现在可以引导加载解锁

> 原文：<https://www.xda-developers.com/nokia-2-2-unofficial-bootloader-unlock/>

回到 2019 年，HMD Global 在生产预算友好型智能手机方面的努力产生了[诺基亚 2.2](https://www.xda-developers.com/nokia-2dot2-launched-india/) 。尽管该公司大力宣传这款设备的“Android One”优点，但发烧友们并不以为然。让 XDA 用户犹豫购买的第一件事是 HMD Global 对 bootloader 解锁的怪异立场。是的，你可以打电话，浏览网页，[获得快速更新](https://www.xda-developers.com/hmd-global-rolls-out-the-android-10-update-for-the-nokia-2-2/)等等，但诺基亚 2.2 在售后市场开发方面仍然受到限制。

然而，看起来事情终于对诺基亚 2.2 的所有者有所好转，因为 XDA 高级成员 [hikari_calyx](https://forum.xda-developers.com/m/hikari_calyx.7601808/) 最近取得了突破，并设法解锁了这款设备的引导加载程序。由于这是一种非官方的解锁引导程序的方法，过程相当复杂，但光彻底详细地描述了每一个动作，指导用户完成每一步。

简而言之，这个过程包括备份你手机的一堆分区，刷新接受标准`fastboot flashing lock_critical`和`fastboot oem unlock`命令的修改后的引导加载程序，降级到 Android 9 Pie，[通过漏洞](https://www.xda-developers.com/mediatek-su-rootkit-exploit/)获得 root 访问权限，最后恢复分区备份。在这之后，您可以大胆地进入 root、定制 rom 和内核的世界，而不涉及任何其他复杂的过程！

如果你有一个诺基亚 2.2，并想尝试一下，前往论坛线程的详细步骤引导加载程序解锁和根访问使用 Magisk。虽然该方法不需要[任何形式的拆卸](https://www.xda-developers.com/nokia-3-2-nokia-4-2-bootloader-unlock-method/)，但是存在风险，因此请仔细阅读说明，并以最大的精确度执行所有步骤。

**[诺基亚 2.2 非官方 bootloader 解锁方法— XDA 线程](https://forum.xda-developers.com/t/guide-how-to-unlock-the-bootloader-for-nokia-2-2.4244039/)**

随着主要障碍(即锁定的引导加载程序)被打破，下一步是为诺基亚 2.2 开发一个定制的 ROM。目前，光已经[分享了](https://forum.xda-developers.com/t/guide-how-to-unlock-the-bootloader-for-nokia-2-2.4244039/post-84622441)安装 [AOSP GSI](https://www.xda-developers.com/developer-boots-android-11-22-older-devices-project-treble-gsi/) 的过程。无论如何，这确实是一个受欢迎的进步，在此之前，手机的前景似乎是暗淡的。快乐闪烁！