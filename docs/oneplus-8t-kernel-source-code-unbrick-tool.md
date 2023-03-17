# 一加 8T 内核源代码和 unbrick 工具现已推出

> 原文：<https://www.xda-developers.com/oneplus-8t-kernel-source-code-unbrick-tool/>

一加 8T 于 10 月 14 日[宣布](https://www.xda-developers.com/oneplus-8t-specifications-features-pricing-availability/)。智能手机是对[一加 8](https://forum.xda-developers.com/oneplus-8) 的中期更新。这款手机上市还不到两周，我们已经看到一加通过发布内核源代码来推动该设备的第三方开发。这并不奇怪，因为 OEM 一直以来都乐于接受开发者社区的需求。此外，特定于设备的 unbrick 包，通常被称为“MsmDownloadTool”，也可供使用。

**[一加 8T 论坛](https://forum.xda-developers.com/oneplus-8t)**

**[一加 8T 回顾:有道理的 T 升级](https://www.xda-developers.com/oneplus-8t-review/)**

及时的内核源代码发布允许开发人员和高级用户更深入地研究运行设备的代码，找出不同的方法来修改配置参数。正确记录的内核源代码版本也有助于基于 AOSP 的定制 ROM(如 LineageOS)的设备启动过程以及定制恢复(如 TWRP ),这反过来又为进一步的定制 ROM 体验奠定了基础。由于一加 8T(代号“kebab”)是随着基于 Android 11 的 OxygenOS 11 开箱而推出的，该公司在与一加 8/8 Pro 的 Android 11 版本相同的分支中发布了这款设备的内核源代码，而不是在自己的分支下。您可以通过点击下面的按钮在内核源代码树中找到实际的提交。

**[一加 8T 内核来源](https://github.com/OnePlusOSS/android_kernel_oneplus_sm8250/commit/6b0c4467b173026171efe9d033e387f9b18b14e1)**

谈到 unbrick 工具，它是一个低级的闪存实用程序，可以恢复单个一加设备。闪光器利用高通的**E**emergency**D**own**l**oad 模式(EDL)，这意味着即使你无法访问快速启动界面，你也可以恢复你的设备。该工具还可以用于将用户的手机回滚到 OxygenOS 的以前版本。它应该适用于中国、印度、欧洲和北美的解锁版手机。

**[一加 8T](https://forum.xda-developers.com/oneplus-8t/how-to/op8t-unbrick-tool-to-restore-device-to-t4180837)T3【解卡工具】**

不过，如果你选择了 T-Mobile 的变种，你需要一个不同的 unbrick 包。从功能上来说，它与用于国际版手机的 unbrick 工具相同。

**[一加 8T (T-Mobile 变体)的解卡工具](https://forum.xda-developers.com/oneplus-8t/how-to/op8t-unbrick-tool-to-restore-device-to-t4180981/)**