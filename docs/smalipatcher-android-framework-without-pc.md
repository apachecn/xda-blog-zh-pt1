# SmaliPatcher 允许你在没有 PC 的情况下对 Android 框架应用 Smali 补丁

> 原文：<https://www.xda-developers.com/smalipatcher-android-framework-without-pc/>

# 轻松地将 Smali 补丁应用到 Android 框架，而无需使用此脚本的 PC

SmaliPatcher for Android 是一个脚本，让您无需 PC 即可将 Smali 补丁应用于 Android 框架。继续阅读，了解更多信息！

定制在 Android 世界是一件大事。你可能已经见过或侧装了修改过的应用程序，例如带有自定义解析支持的补丁拨号器。然而，在不必使用 [Apktool](https://www.xda-developers.com/tag/apktool/) 反编译和重新编译 framework-res.apk 的情况下，对 Android 设备的框架值进行更改是另一回事。来自 XDA 少年成员[的一个名为 *SmaliPatcher for Android* 的新脚本让你做到这一点甚至更多。它允许您直接从 Android 手机向系统框架应用现成的补丁。该脚本还能够生成 Magisk 模块，因此您可以无系统地安装修改后的框架包。](https://forum.xda-developers.com/member.php?u=10071420)

顾名思义，该工具主要基于 XDA 知名开发商 [fOmey](https://forum.xda-developers.com/member.php?u=1620550) 创建的 [Smali Patcher](https://forum.xda-developers.com/apps/magisk/module-smali-patcher-0-7-t3680053) 项目。CreepycCrafter24 决定对代码库进行逆向工程，以消除对 Microsoft Windows 的依赖。[生成的 fork](https://gitlab.com/JFronny/smalipatcher) 完全兼容 Linux，这意味着你也可以通过一些调整在 Android 上执行它。Android 变体托管在同一个 GitLab repo 上，你应该能够在任何标准的终端仿真器应用程序下运行它，例如 [Termux](https://www.xda-developers.com/termux-the-ultimate-linux-terminal-emulator-for-android-xda-spotlight/) 。该脚本提供了一个运行在 Android 应用程序沙箱范围内的 Linux 环境。它通过利用一个名为 [*PRoot*](https://wiki.termux.com/wiki/PRoot) 的软件来实现这一点，这是 Linux 的 *chroot* 功能的用户空间重新实现。

以下是 Smali Patcher 提供的所有内置补丁程序:

*   模拟位置-隐藏模拟位置状态，允许 Pokémon GO 等应用程序将其视为真正的位置更新。
*   安全标志-允许安全应用程序中的屏幕截图/屏幕共享。
*   签名验证-禁用签名验证，允许修改/执行已签名的系统应用程序。
*   签名欺骗-启用签名欺骗应用程序权限。
*   恢复重启-从 powermenu 直接重启恢复。
*   三星诺克斯-绕过三星诺克斯跳闸保护，只确认安全文件夹的工作。
*   高音量警告-禁用高音量弹出对话框。

查看下面的论坛帖子以了解更多信息，并前往 GitLab repo 立即开始！

**安卓版 SmaliPatcher:[下载](https://gitlab.com/JFronny/smalipatcher/-/tree/master/android) || [XDA 线程](https://forum.xda-developers.com/apps/magisk/module-smali-patcher-native-android-t4183061)**