# 基于 Android 11 的 Bliss OS 14 的第一个 alpha 版本即将推出

> 原文：<https://www.xda-developers.com/bliss-os-14-android-11-x86-desktop-pc/>

Bliss OS 14 的第一个 alpha 版本已经发布，使其成为首批支持 x86 环境的基于 Android 11 的 rom 之一。构建显然不稳定，但它证明了开发人员正朝着正确的方向前进。对于那些不知道的人来说，Bliss OS 是一个基于 Android-x86 的开源项目，可用于大多数 x86 PCs，并集成了许多前沿功能和扩展的设备支持。简而言之，它为您老旧的笔记本电脑、台式机或平板电脑设备注入了新的活力。

[最新版本](https://forum.xda-developers.com/t/android-generic-project-pc-gsi-build-automation-toolkit.4132031/page-4#post-84148333)包括一个使用内核 5.8、mesa 20.1.0 等的“最小”版 Bliss OS。开发人员已经设法从谷歌的模拟器图像中提取出 libndk_translation 和 GApps。虽然这是一项正在进行的工作，但开发人员也成功克服了一些早期问题，以便在 PC 版本上运行 ARM 和 ARM64 应用程序。源代码可以在[这里](https://gitlab.com/android-generic/android_vendor_google_emu-x86)获得。

Android 11 不允许用户隐藏导航条。因此，作为一个变通办法，“*我们必须使用旧的 qemu.hw.mainkeys 作为备份计划，所以有一个脚本(toggle_nav.sh)可以用来禁用/启用软导航条和使用任务栏，如果你喜欢。请记住，您将需要以 RW (mount -o remount，rw /dev/loop(0) /)的身份重新挂载/使用 cat proc/mounts 来查看/安装在何处。*

作为 Bliss OS 团队的最新成员和 Gearlock 的创造者之一，@AXIM0S 也在 ROM 中添加了 [Rusty-Magisk](https://github.com/AXIM0S/rusty-magisk/releases/tag/v0.1.3) ，允许内置与 Magisk 的兼容层。话虽如此，大多数 Magisk 模块并不实用，但开发仍在进行中。最近，Bliss 团队将 Bliss OS 更新到了 11.12 和 11.13 版本，支持 ARM64 仿真和 [Magisk](https://www.xda-developers.com/magisk-beta-v21-1-magisk-manager-v8-0-3-pixel-5-pixel-4a-5g/) 。

这也是通过官方论坛帖子分享的构建信息:

所有版本包括:

*   已更新至内核 5.8
*   禁用导航栏的脚本
*   任务栏(桌面模式启动器)
*   Launcher3(普通平板模式启动器)
*   更多内容，请查看变更日志

已知的新问题:

*   睡眠状态在一些机器上不能正常工作。有些会导致 SystemUI 重新启动。
*   一些机器仍然有音量/声音问题，使用第三方均衡器或音量控制。
*   某些设备上的蓝牙
*   旋转在某些设备上不起作用
*   大多数 magisk 模块
*   一些 ARM/ARM64 应用程序仍然无法运行。给我日志
*   这一轮没有 Alt-f1/f7 控制台。如果您需要作为 RW 挂载，或者需要访问根控制台，请在调试模式下引导，或者添加 DEBUG=(0/1/2)作为日志记录级别。
*   一些声卡仍然启动静音 AF，请使用 Goodev 的 Volume Booster 之类的 EQ 应用程序，或者按照 Android-x86 文档/组中的最后说明操作。
*   Widevine 还不能工作，暂时享受大多数其他视频格式
*   Firefox 浏览器在某些机器上强制退出。

在您的机器上试用 Bliss OS 并分享您的体验！