# Magisk (Beta) v21.1 和 Magisk Manager v8.0.3 支持 Pixel 5

> 原文：<https://www.xda-developers.com/magisk-beta-v21-1-magisk-manager-v8-0-3-pixel-5-pixel-4a-5g/>

# Magisk (Beta) v21.1 和 Magisk Manager v8.0.3 带来了 Pixel 5、Pixel 4a 5G 支持等等

XDA 的 topjohnwu 发布了 Magisk (Beta) v21.1 和 Magisk Manager v8.0.3，为 Pixel 5 和 Pixel 4a 5G 提供了支持。

XDA 资深公认开发者 [topjohnwu](https://forum.xda-developers.com/member.php?u=4470081) 发布了 Magisk (Beta) v21.1 和 Magisk Manager v8.0.3，带来了对 Pixel 5 和 Pixel 4a 5G 的支持。Magisk 为用户提供了一个简单的解决方案来根化你的 Android 设备。TopJohnwu 之前[发布了 Magisk 应用的更新](https://www.xda-developers.com/magisk-v21-magisk-manager-8-0-0-released-android-11-support-app-redesign/)，带来了对 Android 11 的支持。

Topjohnwu 今天在 Twitter 上宣布了新的更新，称重点主要是稳定性改进和漏洞修复。但是如果你有一个(或者两个都有！)的最新旗舰产品中，Magisk (Beta) v21.1 现在可以与这些设备一起工作。以下是 Magisk (Beta) v21.1 的完整变更日志:

## 神奇(Beta) v21.1 变更日志

*   [MagiskBoot]支持引导头 v3(像素 5 和 4a 5G)
*   【MagiskBoot】区分`lz4_lg`和`lz4_legacy`(像素 5 和 4a 5G)
*   [MagiskBoot]支持供应商启动映像(用于开发，与 Magisk 安装无关)
*   【MagiskInit】支持内核命令行`androidboot.fstab_suffix`
*   [MagiskInit]支持旧 SAR 上内核初始化的 dm-verity
*   [常规]显著拓宽策略.规则兼容性
*   [常规]执行引导脚本时，将 Magisk 二进制文件添加到`PATH`
*   【通用】更新`--remove-modules`命令的实现
*   【通用】让 Magisk 在 Android 11 上恢复出厂设置后正常存活
*   【MagiskSU】在链接`libsqlite.so`时将 APEX 包`com.android.i18n`添加到`LD_LIBRARY_PATH`
*   [magis hide]支持隐藏二级用户中安装的应用程序(如工作档案)
*   [magis hide]使受精卵检测更加稳定

Magisk Manager v8.0.3 还包括一些稳定性更改和错误修复:

## Magisk Manager v8.0.3

*   切换到新的 Magisk 模块回购设置，准备允许第三方回购
*   在超级用户请求对话框中添加窃听保护
*   稳定性更改和错误修复

如果你不熟悉 Magisk，我们有一个完整的指南，带你通过[如何根你的设备](https://www.xda-developers.com/how-to-install-magisk/)。如果你遇到任何问题，你可以在项目的 [GitHub 库](https://github.com/topjohnwu/Magisk/issues)上提交错误报告。不要忘记参考我们的 Magisk XDA 论坛，了解关于今天发布的最新讨论。

**[Magisk XDA 论坛](https://forum.xda-developers.com/apps/magisk)**

[下载魔法(beta)v 21.1](https://github.com/topjohnwu/Magisk/releases/tag/v21.1)[下载魔法管理器 v8.0.3](https://github.com/topjohnwu/Magisk/releases/download/manager-v8.0.3/MagiskManager-v8.0.3.apk)