# Android 基准测试的 Windows 子系统揭示了它的性能

> 原文：<https://www.xda-developers.com/wundows-subsystem-android-benchmarks-solid-performance/>

新出现的基准测试让我们第一次看到了 Android 的 Windows 子系统的性能。微软在首次宣布新操作系统时宣布 Windows 11 将支持 Android 应用程序，但我们仍有很多不知道的。这将由 Android 的 Windows 子系统实现，该子系统基于 Windows 10 中添加的 Linux 的 Windows 子系统。这意味着它是通过仿真运行的，而仿真通常是以牺牲性能为代价的。

微软还没有分享任何关于 Android 应用程序将如何运行的信息，我们也还不能自己尝试，所以直到现在，还不可能知道 Android 应用程序在 Windows 上的表现如何。通过 [Twitter 用户@AlurDesign](https://twitter.com/AlurDesign/status/1436372189033422848) (通过 [*MSPowerUser*](https://mspoweruser.com/benchmarks-of-microsofts-windows-subsystem-for-android-suggests-it-will-be-pretty-snappy/) )发现的基准测试分数，我们第一次瞥见了 Linux 的 Windows 子系统的性能。结果——你可以在下面看到——差别很大，但它们是有希望的。

一些结果之间存在巨大差异，但结果的高端单核分数在 820 左右徘徊，多核分数在 3000 左右。这将使性能与高通骁龙 865 驱动的手机相一致，这确实很棒。这是一款旗舰处理器，用于三星 Galaxy S20 系列(在一些市场)、一加 8、OPPO Find X2 Pro 和 2020 年的其他旗舰手机。你可以找到 Android 的 Windows 子系统的完整分数列表，并将其与[的顶级 Android 性能指标评测](https://browser.geekbench.com/android-benchmarks)进行比较。

然而，结果的变化可能有点令人担忧。没有办法确定这些基准运行在什么硬件上，因为它们是被模拟的。一些列表显示了高通处理器，而其他的只有一个占位符名称。但是，请注意，高通处理器的名称也可能是虚构的，因为这都是通过仿真实现的。此外，时钟速度都是 0MHz。一个很容易观察到的趋势是，与这种准高通芯片相关的结果是得分最高的结果。占位符分数可能来自软件的早期版本，在进行优化之前。您可以看到，即使一些设备显示有 12 个处理内核，它们的得分仍然远远低于其他 8 核处理器。

无论如何，性能也会随着硬件的不同而有所不同，没有人知道真正运行这些基准测试的 CPU 是什么。如果你需要一个台式机级别的 CPU 来获得这样的分数，这意味着如果你有一台笔记本电脑，性能可能不会很好，特别是如果它是一台超极本。

这些基准测试结果大约在一周前开始出现，这可能表明微软正准备向内部人士提供这些信息。我们还看到 Android 的 Windows 子系统出现在微软商店上，这是另一个潜在的暗示，表明公开发布可能很快就会到来。自然，普通用户将不得不等待更长的时间，我们知道当 Windows 11 在 10 月 5 日推出时，[功能将不可用。](https://www.xda-developers.com/android-windows-11-delayed/)