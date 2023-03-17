# Magisk v22.1 带来了改进的日志编写器、resetprop bootloop 修复等等

> 原文：<https://www.xda-developers.com/magisk-v22-1-update/>

# Magisk v22.1 带来了改进的日志编写器、resetprop bootloop 修复等等

Magisk (v22.1)的最新稳定更新已经发布，包含大量的错误修复和功能改进。继续阅读，了解更多信息！

Magisk 由 XDA 知名开发商 [topjohnwu](https://forum.xda-developers.com/m/topjohnwu.4470081/) 开发，在过去的几年里变得如此流行，以至于现在没有必要介绍了。但是如果您需要的话，Magisk 最初是作为一个无系统的 root 方法开始的，并且已经逐渐发展成为一个比普通 root 更加多样化和强大的工具。使用它最好的一点是，它允许用户修改系统设置，而不需要实际修改系统文件。Magisk 的最新主要版本，对应于第二十二版(v22)，是在二月发布的[，对界面进行了一些有趣的更新。现在，开发人员发布了 v22.1，其中包括对 Magisk 内部组件和 Magisk 应用程序的更多更改和错误修复。](https://www.xda-developers.com/magisk-v22-release-samsung-galaxy-s21-support/)

**[Magisk XDA 论坛](https://forum.xda-developers.com/f/magisk.5903/)**

根据发行说明，更新对 resetprop 模块进行了改进，支持在启动映像中保留和修补 AVB 2.0 结构/头，支持 cgroup 迁移，以及旨在解决崩溃和死锁的重写日志编写器组件。

这是 Magisk v22.1 的官方变更日志:

*   [App]防止多个安装会话并行运行
*   [App]在检查 PXA 启动映像上的启动签名时防止内存不足崩溃
*   [常规]正确的 c 组迁移实施
*   [常规]从头开始重写日志编写器，应该可以解决任何崩溃和死锁问题
*   [常规]许多脚本更新修复回归
*   [magis hide]防止信号到达时可能出现的死锁
*   [magis hide]必要时部分匹配进程名
*   [MagiskBoot]保留并修补启动映像中的 AVB 2.0 结构/头
*   [MagiskBoot]正确去除数据加密标志
*   [MagiskBoot]防止可能的整数溢出
*   [MagiskInit]修复`sepolicy.rule`安装策略
*   [resetprop]总是在更新之前删除现有的`ro.`道具。这将修复由于修改设备指纹属性而导致的引导错误。

如果您想了解 v22.1 的全部细节，请从下面的 GitHub 链接下载到您的设备上。你所要做的就是[将下载文件的扩展名从 APK 改为 ZIP](https://www.xda-developers.com/install-magisk-manager-without-separate-zip/) ，并通过自定义恢复(最有可能是 TWRP)刷新它。

**[下载魔法 v22.1](https://github.com/topjohnwu/Magisk/releases/tag/v22.1)T3**

值得一提的是，Magisk v22 是最后一个支持 Android Jellybean 和 Kitkat 的主要版本。[正如 topjohnwu](https://twitter.com/topjohnwu/status/1379393206157197315) 所说，下一个版本将只支持 Android 5.0 Lollipop 及更高版本。