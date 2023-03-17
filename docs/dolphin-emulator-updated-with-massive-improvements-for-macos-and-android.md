# Dolphin 模拟器针对 macOS 和 Android 进行了大量改进

> 原文：<https://www.xda-developers.com/dolphin-emulator-updated-with-massive-improvements-for-macos-and-android/>

# Dolphin 模拟器针对 macOS 和 Android 进行了大量改进

广受欢迎的任天堂 GameCube 和 Wii 模拟器 Dolphin Emulator 修复了 ARM 设备的许多问题，并增加了苹果 M1 硬件支持。

Dolphin 是玩任天堂 GameCube 和 Wii 游戏的最佳模拟器，而且它不仅仅在台式电脑上可用。Android 移植已经存在很多年了，在过去的两个月里，Dolphin Emulator 团队一直致力于一些重要的改变。Dolphin 现在可以在苹果 M1 硬件上运行，对 Mali GPUs 上的仿真的新修复意味着更多的游戏可以在 Android 设备上正常运行。

Dolphin 上个月末刚刚增加了对苹果 M1 芯片组[的本地支持，使用了该项目的 AArch64 JIT(实时)仿真核心，该核心是为 ARM 上的 Android 和 Windows 开发的。Dolphin 的 ARM 支持不像 64 位 x86 硬件上的仿真那样完整，但在大多数游戏中性能已经很好了。“不可否认，”Dolphin Emulator 团队在博客中写道，“macOS M1 硬件踢了一些严重的屁股。它完全抹杀了两年半前价格超过其三倍的英特尔 MacBook Pro，同时保持了强大的台式计算机触手可及的优势。”](https://dolphin-emu.org/blog/2021/05/24/temptation-of-the-apple-dolphin-on-macos-m1/)

 <picture>![Bar graph showing macOS M1 performance](img/9ebed100a4503f8803c5493f19880e4e.png)</picture> 

Dolphin performance comparison (Credit: Dolphin)

随着强大的基于 ARM 的硬件变得越来越普遍，Dolphin 的开发人员一直在努力修复 ARM 仿真核心中长期存在的错误和性能问题。浮点计算的修复修复了*纸上马里奥:千年门*、*塞尔达传说:天空之剑*、*声波颜色*、*声波释放*等游戏中的崩溃和图形问题。Dolphin Emulator 还修复了 Mali GPUs 上着色器的错误，这些错误影响了许多运行在 Android 手机和平板电脑上的游戏。

Dolphin 也在修复 Android 上的控件问题。控制器配置现在可以正确保存了，随着触摸屏按钮透明度的改变，在没有物理控制器的情况下玩游戏变得更容易了。查看[完整的博客文章](https://dolphin-emu.org/blog/2021/06/06/dolphin-progress-report-april-and-may-2021/),了解最新稳定的 Dolphin 模拟器版本的其他内容。