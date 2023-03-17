# 使用通用的 Android Debloater 从您的手机中删除膨胀软件和不需要的应用程序

> 原文：<https://www.xda-developers.com/universal-android-debloater-remove-unwanted-bloatware-apps/>

# 通用安卓解包器帮助你摆脱手机上不想要的应用程序和臃肿软件

你讨厌 Android 设备上的膨胀软件或预装应用吗？以下是如何使用通用 Android 去涂层器移除它们的方法。

我们已经在很多场合谈论过预装应用，也就是“膨胀软件”。众所周知，运送这种非必要的应用程序是运营商/OEM 商业政策的重要组成部分。考虑到这些应用程序可以在你的手机上收集的诊断和使用数据的数量，人们可以很容易地推断出运营商和原始设备制造商这样做是为了增加收入和控制平台。诚然，膨胀软件是一个相当主观的术语，但无法通过传统方式卸载甚至禁用这些预装的系统应用程序无疑是 Android 用户群的一个障碍。

幸运的是，有一些社区制作的去模糊工具可以帮助摆脱这些应用程序。不久前，我们还[写了一个指南](https://www.xda-developers.com/disable-system-app-bloatware-android/)，教你如何使用 [Android Debug Bridge](https://www.xda-developers.com/install-adb-windows-macos-linux/) (ADB)从你的 Android 智能手机或平板电脑的主要用户帐户中卸载任何预装的应用程序。如果你不想经历所有的手动 ADB 命令，XDA 成员 [w1nst0n_fr](https://forum.xda-developers.com/m/w1nst0n_fr.10413801/) 已经整理了一个脚本来帮助用户以一种更安全的方式解锁他们的设备。认识一下**Universal Android Debloater**——一个列表驱动的 de bloater 项目，它不仅可以禁用 OEM 和运营商安装的不想要的臃肿软件，而且如果你有 root 权限，还可以删除 apk。

**[通用安卓解封器 XDA 线程](https://forum.xda-developers.com/t/script-2021-01-30-v2-9-universal-android-debloater.4069209/)**

该项目的核心是一个名为`debloat_script.sh`的 Bash 脚本，这意味着它与 Linux 和 macOS 兼容。但是，Windows 用户需要首先安装一个兼容的 Unix 终端才能使用该工具。该脚本依赖于幕后的众包去模糊列表。您可以找到几个现成的 OEM 和运营商特定的列表，而项目[的开源性质使得提交额外的条目来贡献](https://gitlab.com/W1nst0n/universal-android-debloater/-/wikis/home#how-to-contribute)变得非常容易。

以下是通用 Android Debloater 提供的功能概述:

*   在 Android 设备的所有包中快速搜索
*   卸载系统/用户软件包(手动或使用去保列表)
*   系统软件包的重新安装(手动或使用去模糊列表)
*   ADB 备份/恢复
*   设备品牌检测和自动选择合适的制造商去模糊列表
*   日志记录:**解包 _ 包. txt** ，**剩余 _ 包. txt** ，**删除 _apks.txt** (针对 root 用户)
*   根支持(有 Magisk 的系统和无系统)

如果你有兴趣尝试解封层脚本，你可以在这里找到最新版本。那些想看看代码库并做出贡献的人可以访问[该项目的 GitLab 资源库](https://gitlab.com/W1nst0n/universal-android-debloater)。

**[通用安卓解封器 XDA 线程](https://forum.xda-developers.com/t/script-2021-01-30-v2-9-universal-android-debloater.4069209/)**