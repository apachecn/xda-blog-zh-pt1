# 一名开发人员让 Ubuntu Linux 在苹果 iPhone 7 上启动

> 原文：<https://www.xda-developers.com/apple-iphone-7-ubuntu-linux-checkra1n-project-sandcastle/>

# 一名开发人员让 Ubuntu Linux 在苹果 iPhone 7 上启动

一名开发人员在苹果 iPhone 7 上实现了用图形界面启动 Ubuntu 20.04 的惊人壮举。继续阅读，了解更多信息！

早在 2020 年 3 月，当 Corellium 展示了使用 [checkra1n 越狱](https://www.xda-developers.com/jailbreak-apple-iphone-using-checkra1n-rooted-android-phone/)在苹果 iPhone 7 上启动 Android 的[项目 Sandcastle](https://www.xda-developers.com/install-android-10-apple-iphone-7-plus-project-sandcastle-checkra1n-jailbreak/) 时，它引发了人们对传统 iPhone 机型上操作系统级售后开发潜力的希望。除非硬件出现故障，否则如果高级用户可以在这些设备上安装任何常规的 GNU/Linux 发行版，它们中的许多设备可能还会使用很多年。事实上，最近的一项发展引起了我们的注意，这将有助于为延长这些旧 iPhone 设备的寿命铺平道路。

Reddit 上一位名为“ [newhacker1746](https://www.reddit.com/user/newhacker1746/) 的开发者正在接受挑战，将 iPhone 7 变成一部基于 Linux 的智能手机。除了在 iPhone 7 上启动 Ubuntu 20.04 LTS 的 ARM64 版本，开发人员还设法在设备上运行 GNOME 桌面环境的完整图形外壳。

请记住，开发人员没有替换内部 NAND 的内容，而是设法使用来自 Sandcastle 项目的[定制 Linux 内核来网络引导 Ubuntu 实例。开发者](https://github.com/corellium/linux-sandcastle)[分享了一份关于如何制作自己的“iPhone 7 Ubuntu 版”的非常详细的指南](https://www.reddit.com/r/linux/comments/kux9xx/success_iphone_7_with_dead_nand_netbooting/)，你甚至可以按照指南进行操作，而不用担心破解设备。然而，试图让你的 iPhone 7 在 Ubuntu 上运行对于没有经验的用户来说可能不是一个非常令人满意的体验，因为你仍然需要事先手动编译内核，并使用 checkra1n 访问 [pongoOS](https://github.com/checkra1n/pongoOS) 预引导执行环境。

一个试图在苹果 iPhone 7 上运行 Ubuntu 的修改者并不奇怪，因为这个系列对 Linux 内核并不陌生。我想到了 postmarketOS 项目，正是这个项目[将 Linux 带到了 iPhone 7 和 7 Plus](https://wiki.postmarketos.org/wiki/Apple_iPhone_7/7%2B_(apple-iphone7)) 。虽然在 iPhone 上安装像 Ubuntu 这样的 GNU/Linux 发行版不会给你带来和直接运行 iOS 一样的体验，但是从旧设备中挤出像样的性能，直到它出现物理故障，这将是非常有用的。记住，本着[传奇 HTC HD2](https://www.xda-developers.com/htc-hd2-refuses-to-die-now-runs-windows-rt/) 的精神，这不是关于实际运行软件，而是关于证明它可以做到。

* * *

**来源:r/linux ( [1](https://www.reddit.com/r/linux/comments/kux9xx/success_iphone_7_with_dead_nand_netbooting/) ， [2](https://www.reddit.com/r/linux/comments/kvmsfd/success_iphone_7_booting_ubuntu_2004_to_full/) )**