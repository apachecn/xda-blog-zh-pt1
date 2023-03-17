# Magisk v21.2 和 Magisk Manager v8.0.4 发布，修复了 root 访问的错误和稳定性

> 原文：<https://www.xda-developers.com/magisk-v21-2-magisk-manager-8-0-4-released-bug-stability-fixes-root-access/>

# Magisk v21.2 和 Magisk Manager v8.0.4 发布，修复了 root 访问的错误和稳定性

Magisk (v21.2)和 Magisk Manager (v8.0.4)的最新更新为 root 访问带来了几个错误修复和稳定性改进。

XDA 资深公认开发者 topjohnwu 的 Magisk 无疑是 Android 设备最受欢迎的根解决方案。有了它，给你的 Android 设备找根就像在像 [TWRP](https://www.xda-developers.com/how-to-install-twrp/) 这样的自定义恢复中刷新一个. zip 文件和安装 Magisk Manager 应用程序一样简单。该工具最近[收到了一个重大更新](https://www.xda-developers.com/magisk-v21-magisk-manager-8-0-0-released-android-11-support-app-redesign/)，引入了对 Android 11 的支持，一个应用程序的重新设计，等等。在最后一个稳定版本发布后不久，Magisk 在测试频道上收到了一个[更新，带来了对](https://www.xda-developers.com/magisk-beta-v21-1-magisk-manager-v8-0-3-pixel-5-pixel-4a-5g/) [Google Pixel 5](https://www.xda-developers.com/tag/google-pixel-5/) 和 [Pixel 4a 5G](https://www.xda-developers.com/tag/google-pixel-4a5g/) 的支持，以及其他一些小的变化。现在，topjohnwu 为 Magisk (v21.2)和 Magisk Manager (v8.0.4)推出了另一个更新，为 root 访问带来了几个 bug 和稳定性修复。

Magisk 和 Magisk Manager 的最新更新是维护更新，主要是解决错误、扩展设备兼容性和增强稳定性。以下是最新 Magisk 和 Magisk Manager 版本的完整变更日志:

### 神奇 v21.2 变更日志:

*   在传统 SAR 设备上安装`system_root`后,[MagiskInit]检测 2SI
*   [常规]确保`post-fs-data`脚本不能阻塞超过 35 秒
*   [常规]修复`magisk --install-module`命令
*   [常规]读取文件时修剪窗口换行符
*   【常规】直接记录到文件中，防止`logcat`怪异
*   [MagiskBoot]修复了标题 v3 映像的标题转储/加载

### Magisk Manager v8.0.4 changelog:

*   大量的稳定性变化和小的错误修复
*   在日志菜单中保存日志时，收集设备属性、应用程序日志和 Magisk 日志

您可以通过下面的链接下载最新版本。如果您不熟悉 Magisk，您应该查看我们关于如何使用该工具根化您的设备的深入指南。如果你碰巧遇到了最新版本的任何问题，确保在项目的 [GitHub 库](https://github.com/topjohnwu/Magisk/issues)上提交一份错误报告。此外，请查看我们的 Magisk 论坛，了解关于今天发布的最新讨论。

[**Magisk XDA 论坛**](https://forum.xda-developers.com/f/magisk.5903/)

**下载魔法(v21.2)[下载魔法管理器(v8.0.4)](https://github.com/topjohnwu/Magisk/releases/tag/manager-v8.0.4) 下载魔法管理器**