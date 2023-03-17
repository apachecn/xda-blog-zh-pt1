# 在具有未锁定引导加载程序的设备上绕过安全网证明

> 原文：<https://www.xda-developers.com/bypass-safetynet-hardware-attestation-unlocked-bootloader-magisk-module/>

在过去的几年里，绕过安全网认证的挑战已经从谷歌和改装社区之间的简单猫捉老鼠游戏演变成一场充满模糊障碍的新兴战斗。由于[硬件支持的证明技术](https://www.xda-developers.com/safetynet-hardware-attestation-hide-root-magisk/)的兴起，绕过引导映像完整性验证例程和隐藏 root 访问变得非常困难。单独安装 Magisk 不足以绕过最新的 SafetyNet 更新，尤其是在较新的设备上。这正是通用安全网修复 Magisk 模块的用武之地。

虽然传统设备所有者以及定制 ROM 用户经常利用像[magis hide Props Config](https://forum.xda-developers.com/t/module-magiskhide-props-config-safetynet-prop-edits-and-more-v5-4-0.3789228/)这样的模块来欺骗 CTS 配置文件以通过基本证明，但只要该方法依赖于设备和型号名称、构建指纹以及安全补丁级别的有效组合，就不能保证根隐藏技巧在未来仍然有用。这是因为在许多情况下，Google Play 服务开始使用硬件证明进行 CTS 配置文件验证，即使选择了基本证明。

用更专业的术语来说，即使来自 GMS 的安全网证明 API 响应将报告使用了基本证明，也总是使用硬件证明，而不管所报告的状态如何，以便实施完整性。因此，密钥证明报告中存在引导加载程序解锁状态会导致安全网证明无法通过。

如果您的 Android 设备有一个未锁定的引导加载程序(或使用自定义验证的引导密钥锁定)，因此没有通过硬件认证，那么通用安全网修复 Magisk 模块可能会修复这一问题。该模块由丹尼·林(又名高级成员 [kdrag0n](https://forum.xda-developers.com/m/kdrag0n.7291478/) 创建，利用硬件证明例程的机会主义性质工作。引用开发商的话:

> #### ...如果密钥证明无法运行，it(硬件证明)会退回到基本证明，并阻止 GMS 在框架级别使用密钥证明。这导致它优雅地退回到基本证明，并通过带有解锁引导加载程序的 SafetyNet。
> 
> ...
> 
> 来自 Keymaster 的“未实现”错误代码用于模拟最真实的故障条件以逃避检测，即缺少密钥证明支持的旧设备。

该解决方案已经预集成在来自同一开发商的 [ProtonAOSP ROM](https://www.xda-developers.com/pixel-5-first-custom-rom-protonaosp/) 中，允许您在相当现代的设备(如 Google Pixel 5)上通过 SafetyNet 而无需 Magisk。如果你是一个定制的 ROM 维护者，并且你希望将这种方法集成到你的构建中，你可以通过从[这个库](https://github.com/kdrag0n/safetynet-fix/tree/master/patches)中挑选必要的补丁来实现。另一方面，最新版本的准备闪存 Magisk 模块变体可以在[这里](https://github.com/kdrag0n/safetynet-fix/releases/latest)找到。注意，如果目标设备是根设备，MagiskHide 仍然是必需的。

**通用安全网修复: [XDA 线程](https://forum.xda-developers.com/t/magisk-module-universal-safetynet-fix-1-1-0.4217823/) ||| [GitHub 回购](https://github.com/kdrag0n/safetynet-fix)**