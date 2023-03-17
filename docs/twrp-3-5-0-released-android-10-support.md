# TWRP 3.5.0 发布，支持搭载 Android 10 的设备

> 原文：<https://www.xda-developers.com/twrp-3-5-0-released-android-10-support/>

用户来我们论坛的一个最常见的原因是刷新自定义模块、内核或 rom。但是，如果没有安装它们的手段，这些售后市场开发努力都是不可行的。这就是非常受欢迎的团队胜利恢复项目(简称 TWRP)的由来。TWRP 可以在许多安卓设备上使用，已经成为任何想要修改设备上软件的人的首选定制恢复工具。现在，该项目已经升级到 3.5.0 版本，带来了解密、错误修复和支持 Android 10 设备的许多改进。

TWRP 新主要版本的完整变更日志可以在下面找到，但对于普通用户和开发者来说，最重要的变化将是 Android 10 兼容性。直到 [TWRP 3.4.0](https://www.xda-developers.com/twrp-3-4-0-enables-ozip-decryption-realme-oppo-devices-support-legacy-devices-upgraded-android-10/) ，对 AOSP 10 [中引入的动态/逻辑分区和许多其他变化的支持还没有完全实现](https://www.xda-developers.com/twrp-lead-explains-android-10-support-custom-recovery/)。大多数限制在 TWRP 3.5.0 中不再存在，这意味着与 Android 10 一起发布的设备最终可以安装正式的 TWRP 版本。XDA 认可的开发人员 [Captain_Throwback](https://forum.xda-developers.com/m/captain_throwback.1162986/) 与 XDA 认可的开发人员 [mauronofrio](https://forum.xda-developers.com/m/mauronofrio.4712355/) 、XDA 资深成员 [noahajac](https://forum.xda-developers.com/m/noahajac.7166807/) 和 AndroidableDroid 合作，通过[从头重写 TWRP 代码库](https://github.com/TeamWin/android_bootable_recovery/commits/android-10.0)的重要部分，使之成为可能。

展望未来，TWRP 维护者在移植定制恢复时将面临两个独立的分支:使用 Android 10 发布的设备将在 [*android-10*](https://github.com/TeamWin/android_bootable_recovery/tree/android-10.0) 分支下得到支持，而传统设备将在 [*android-9.0*](https://github.com/TeamWin/android_bootable_recovery/tree/android-9.0) 分支下构建。此外，TWRP 团队的两名主要成员，XDA 资深公认开发人员 [Dees_Troy](https://forum.xda-developers.com/m/dees_troy.912474/) 和 [bigbiff](https://forum.xda-developers.com/m/bigbiff.2638973/) ，已经在致力于 Android 11 的发布，谷歌 Pixel 5 预计将在不久的将来推出。

以下是更新的完整变更日志:

### twp 3 . 5 . 0 变更日志

*   安卓 9
    *   修复 android-5.1 树中的构建
    *   新的 QTI 触觉支持- AndroidableDroid
    *   新型 TSPDriver 触觉支持- LameMonster82
    *   Selinux 还原问题- AndroidableDroid
    *   OEM 版本修复- Fighter19
    *   Gui 文件选择器中更多的文件扩展名支持
    *   FBE 修复- CaptainThrowback
    *   Ozip 解密- Mauronofrio
    *   不要对恢复日志使用 persist-bigbiff
    *   必要时延迟触摸启动- bigbiff
    *   西班牙语翻译更新- R0rt1z2
    *   修复仅插槽 A 设备上的缓存擦除- AndroidableDroid
    *   从备份中排除 dumpsys 目录- DarthJabba9
    *   Gerrman 翻译更新- 4ndyZ
    *   运行时硬件旋转(不影响触摸屏)- webgeek1234
    *   API 24 修复程序- AndroidableDroid
    *   卸载时出现 vold_decrypt 错误- CaptainThrowback
    *   多用户-当用户未被解密时发出警告- noahajac
    *   FDE 加密修复- CaptainThrowback
    *   加密状态修复- nebrassy
    *   中文翻译更新- Whyle
    *   配合 android-10 发布的主题更新:CaptainThrowback
    *   将 TWRP 应用程序安装移动到高级页面- Dees_Troy
    *   更新俄语翻译- f2065
*   安卓 10
    *   你可以在 [Github](https://github.com/TeamWin/android_bootable_recovery/commits/android-10.0) 看到变化列表

您可以从以下链接的官方网站为您的设备下载最新版本的定制恢复。目前，3.5.0 版本将只为基于 Android 9 Pie 和 Android 10 的设备构建，因此如果您的设备目前正在维护，那么您应该会在几个小时或几天内看到更新。请务必查看您设备的 XDA 论坛，因为您设备的 TWRP 维护者可能会在版本上线时发布更新。

**[为您的设备下载 TWRP](https://twrp.me/Devices/)**

如果你想从你的设备上下载 TWRP 的最新版本，你应该从 Google Play 上查看 TWRP 的官方应用。

[应用程序框 Google play me . twp . twp . twp 纸]