# 树莓 Pi 4 通过 OmniROM 体验 Android 11

> 原文：<https://www.xda-developers.com/raspberry-pi-4-gets-a-taste-of-android-11-via-omnirom/>

# 树莓 Pi 4 通过 OmniROM 体验 Android 11

树莓 Pi 4 获得了 Android 11 的一个端口，这要归功于 OmniROM 定制 ROM 项目。继续阅读，了解更多信息！

随着开发人员最初试图在任何可以运行 Android 11 的设备上启动 Android 11，下一个获得最新操作系统非官方移植的大人物是 Raspberry Pi 4。受欢迎的信用卡大小的计算机的 Android 11 以 OmniROM 的形式出现，由 XDA 资深成员 [maxwen](https://forum.xda-developers.com/member.php?u=4683552) 提供。目前被破坏的功能包括截屏、Wi-Fi 热点和硬件加速视频播放，这使得这款广受喜爱的设备成为 Android 11 令人印象深刻的第一个端口。

**[树莓派 XDA 论坛](https://forum.xda-developers.com/raspberry-pi)**

让这个港口印象深刻的是树莓 Pi 4 所处的环境。基于 Debian Linux 的 Raspberry Pi OS(原名 Raspbian)是这款单板电脑所有型号的官方操作系统。虽然存在对旧版本 Raspberry Pi 的 Android 支持，但 Pi 制造商还没有低级固件实现来允许它在常规版本的 Android 上运行。开发人员不得不从头开始集成开源驱动程序栈，修补封闭的源代码 blobs，并创建包装器将它们拼凑在一起，从而使设备能够正常工作。这是一个非常密集的过程，需要很多技巧和耐心。

ROM 支持从普通的 microSD 卡以及外部 USB 存储介质启动。相关参数[可以在 config.txt](https://github.com/maxwen/android_device_brcm_rpi4/blob/android-11/README) 中通过启用所需的覆盖来设置。喜欢无谷歌体验的用户可以选择 ROM 的 [MicroG](https://forum.xda-developers.com/android/apps-games/app-microg-gmscore-floss-play-services-t3217616) 版本，而每周版本与标准 GApps 包兼容。

**基于 Android 11 的 OmniROM for the Raspberry Pi 4:[下载](https://dl.omnirom.org/tmp/rpi4/) || [XDA 线程](https://forum.xda-developers.com/raspberry-pi/orig-development/omnirom-android-r-11-pi-4-t4183121)**

Raspberry Pi SBCs 对定制 ROM 场景并不陌生，因为修改者总是试图在其上运行某种形式的常规 Android。虽然在 Pi 上安装 Android 不会给你带来与直接购买 Android 电视盒子相同的体验，但这样的发展确实证明了硬件平台的“黑客友好”性质。