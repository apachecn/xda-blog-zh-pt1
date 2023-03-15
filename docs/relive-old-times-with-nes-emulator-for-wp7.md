# DuckStation 是 PlayStation 1 游戏的最佳模拟器

> 原文：<https://www.xda-developers.com/relive-old-times-with-nes-emulator-for-wp7/>

证明 Android 作为一个操作系统有多开放的一个证据是，你可以从谷歌 Play 商店上安装多得令人难以置信的软件。模拟器是使 Android 成为强大的移动操作系统的重要组成部分，因为它可以从几乎任何旧的控制台或手持设备上玩游戏。Playstation 1 就是这样一款游戏机，是两者的最爱，令人印象深刻的游戏目录，只是一些简单的怀旧。虽然谷歌 Play 商店上已经有了针对 Playstation 1 的模拟器(并且已经做了很多年)，但鲜为人知的 DuckStation 是你能得到的最好的模拟器。

## 为什么不用 ePSXe 呢？

ePSXe 是一个神奇的模拟器，绝对没有任何问题。它有很大的支持，但它非常旧，而且需要钱，最后一次更新是在 2019 年 12 月。DuckStation 是免费的、开源的，有很多现代仿真特性和修复。它支持 [Vulkan 图形 API](https://www.xda-developers.com/dolphin-emulator-fixes-vulkan-api-android-pie-wii-remote-pointer-emulation/) ，升级到 4K，甚至升级到 8K。甚至有一个 libretro 内核可以用作 RetroArch 中 PSX 仿真的后端。DuckStation 有很多*设置。*

DuckStation 中的一个重要修正是 PXGP，它修正了 3D 几何图形中的大量跳跃和抖动。你可以在下面的视频中看到一个明显的例子，它显示了游戏*寂静岭*在有和没有 PXGP 的情况下运行。

https://www.youtube.com/watch?v=92DqVFzcM9Q

DuckStation 也可以在 Windows 10(x86 和 ARM64)、macOS 和 Linux 上运行。然而，目前还不支持 Android TV。

DuckStation 的目标是尽可能精确，同时仍然保持适合低端设备的性能。默认配置应该支持几乎所有的游戏，只有一些增强有兼容性问题。你还需要自己的 BIOS，尽管这在 PSX 仿真中并不新鲜。您可以从自己的 PlayStation 转储一个，DuckStation 将支持任何硬件版本或地区的 BIOS。

## 测试坞站

我在 OPPO Find X2 Pro 上测试了 DuckStation，发现其 4 倍内部分辨率的性能非常出色，唯一的增强功能是 PGXP 几何校正。我测试了*速成鼠 3* 和*飞龙 Spyro*。

https://www.youtube.com/watch?v=yl6lXHdFYyI

https://www.youtube.com/watch?v=mNkJdAxR2jc

正如你从上面两个视频中看到的，仿真几乎是完美的。你可以在任何地方，在你的智能手机或笔记本电脑上轻松地玩 PlayStation 1 的所有顶级游戏。你可能需要一部稍微强大一点的安卓智能手机来在 ePSXe 运行 DuckStation，但如果可以的话，这是值得的。它易于使用，功能齐全。如果你想了解一下，可以在 GitHub 上查看 [DuckStation！](https://github.com/stenzek/duckstation)