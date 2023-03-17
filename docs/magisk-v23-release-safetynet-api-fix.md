# Magisk v23.0 带来了 SafetyNet API 修复，但放弃了对传统 Android 的支持

> 原文：<https://www.xda-developers.com/magisk-v23-release-safetynet-api-fix/>

# Magisk v23.0 带来了 SafetyNet API 修复，但放弃了对传统 Android 的支持

Magisk 稳定版本(v23.0)的最新版本附带了大量针对 root 访问和 SafetyNet API 的错误修复。看看吧！

Magisk 对于 Android 高级用户来说是一个不可思议的工具。这是一个独特的无系统界面，由 XDA 的资深公认开发人员 [topjohnwu](https://forum.xda-developers.com/m/topjohnwu.4470081/) 创建，可用于不仅仅是给你的设备找根。该界面帮助用户修改系统设置，而无需实际更改系统文件。Magisk 受欢迎的另一个原因是其绕过谷歌安全网(T3)的潜在能力，谷歌安全网阻止某些应用在根设备上运行。Magisk 的最新更新以 Magisk 版本 23.0 的形式发布，它带来了几个针对 root 访问的错误修复。

**[Magisk XDA 论坛](https://forum.xda-developers.com/f/magisk.5903/)**

开发者今天在 Twitter 上宣布了新的更新，称重点是稳定性的提高。如果您将 Magisk 应用程序仅用于 SafetyNet 认证检查，并且您发现该功能在过去几周内被破坏，那么您会很高兴地知道这个版本也解决了这个问题。

以下是 Magisk v23.0 的[完整变更日志](https://topjohnwu.github.io/Magisk/changes.html#v230):

*   [App]更新 snet 扩展。这修复了 SafetyNet API 错误。
*   [App]修复存根应用程序中导致 APK 安装失败的错误
*   [App]当隐藏为存根时，隐藏日志中令人讨厌的错误
*   [App]修复当应用程序隐藏时修补 ODIN tar 文件的问题
*   [常规]移除所有 Android 5.0 之前的支持
*   [常规]更新 BusyBox 以使用正确的 libc
*   [常规]修复 C++未定义的行为
*   [常规]几个策略规则复制/安装修复
*   [MagiskPolicy]删除不必要的策略规则
*   [magis hide]更新包和进程名验证逻辑
*   [magis hide]一些防止合子死锁的变化

您可以通过下面的链接下载最新版本。如果您不熟悉 Magisk，您应该查看我们关于如何使用该工具根化您的设备的深入指南。如果你碰巧遇到了最新版本的任何问题，确保在项目的 [GitHub 库](https://github.com/topjohnwu/Magisk/issues)上提交一份错误报告。

**[下载魔法 v23.0](https://github.com/topjohnwu/Magisk/releases/tag/v23.0)T3**

需要注意的一点是，随着这个版本的发布，Magisk 终于停止支持比 Android 5.0 Lollipop 更老的 Android 版本。如果你仍然有一个运行 Android KitKat 或 Jelly Bean 的设备，并希望使用 Magisk 来支持它，你必须坚持使用[传统版本](https://www.xda-developers.com/magisk-v22-1-update/)。