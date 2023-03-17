# 通用安全网修复更新，支持 Android 12

> 原文：<https://www.xda-developers.com/universal-safetynet-fix-update-android-12-many-oem-skins/>

# 通用安全网补丁更新，支持 Android 12 和许多 OEM 皮肤

Universal SafetyNet Fix 的最新更新带来了对 Android 12 的支持，以及几个 OEM 皮肤。请继续阅读，了解更多信息。

Android 售后开发领域花了很长时间才找到一种通用的方法来绕过[硬件支持的安全网认证技术](https://www.xda-developers.com/safetynet-hardware-attestation-feature-here-to-stay/)，但经过大量的工作，XDA 高级成员 [kdrag0n](https://forum.xda-developers.com/m/kdrag0n.7291478/) [在 1 月](https://www.xda-developers.com/bypass-safetynet-hardware-attestation-unlocked-bootloader-magisk-module/)完成了这一壮举。令人欣慰的是，修复与 Android 12 兼容的时间大大减少了。开发者现在发布了一个新版本的通用安全网补丁。这个新版本标记为 v2.0.0，还增加了对几个流行的 Android OEM 皮肤的支持，并进行了大量改进。

SafetyNet 修复在 7 月更新了 [Android 12 Beta 2](https://www.xda-developers.com/android-12-beta-2/) 支持[，但它没有获得后续测试版本或即将到来的稳定版本的更新。随着 SafetyNet Fix v2.0.0 的推出，这种情况发生了变化，因为它完全支持](https://github.com/kdrag0n/safetynet-fix/releases/tag/v1.2.0) [Android 12 Beta 4](https://www.xda-developers.com/android-12-beta-4/) 和未来的版本。如果你有一部运行定制皮肤的手机，比如三星的 One UI 或小米的 MIUI，并且在使用旧版本时遇到了故障，那么你会很高兴地知道最新版本也解决了这些问题。

此版本的[完整变更日志](https://github.com/kdrag0n/safetynet-fix/releases/tag/v2.0.0)可以在下面找到:

*   增加了对重度 OEM 皮肤的支持(One UI，MIUI 等。)
*   增加了对 Android 12 Beta 4 和未来版本的支持
*   除了安全网之外，修复了中断的游戏服务功能
*   固定罕见的系统冻结所造成的播放服务破损
*   Android 12:Pixel 4 系列上固定人脸解锁
*   增加了对 Android 7.0 和 7.1 的支持
*   重写为 Riru 模块

**万能安全网修复:[下载](https://github.com/kdrag0n/safetynet-fix/releases/latest) ||| [XDA 讨论帖](https://forum.xda-developers.com/t/4217823/)**

请记住，如果您的设备是根设备，单靠修复可能不足以绕过硬件证明。如今，欺骗它有点复杂，特别是因为官方 Magisk 应用程序正在[放弃对通过 MagiskHide 隐藏 root 访问权限](https://www.xda-developers.com/magisk-development-continues-without-magiskhide/)的支持。为了应对这种情况， *kdrag0n* 已经[发布了](https://kdrag0n.dev/patreon/safetynet-fix/v2.1.0)一个版本为 v2.1.0 的热修复程序，目前他的早期支持者可以获得该程序。新版本包含隐藏根状态所需的所有 MagiskHide 相关特性。一旦补丁得到足够多的积极反馈，相关的代码就会登陆他的 GitHub repo 。