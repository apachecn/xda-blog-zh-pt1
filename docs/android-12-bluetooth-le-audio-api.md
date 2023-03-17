# Android 12 增加了支持蓝牙 LE 音频配置文件的 API

> 原文：<https://www.xda-developers.com/android-12-bluetooth-le-audio-api/>

除非你从昨天起就生活在岩石下，否则你知道谷歌 I/O 2021 正在进行中。这是谷歌今年最大的活动，尽管它更关注开发者而不是消费者，但其中的声明与两种人口统计数据都相关。其中一个公告是关于 [Android 12](https://www.xda-developers.com/android-12/) 增加蓝牙 LE Audio 的 API，这是一个重要的公告，将极大地增强终端用户使用蓝牙耳机和其他音频设备的体验。

隐藏在大量公告中的是对蓝牙 LE Audio API 的揭示，它提供了控制 LE Audio 配置文件的公共 API。API 中提到，Android 一次只支持一套连接的蓝牙 LE 音频设备。

在我们深入了解它的重要性之前，让我们先回顾一下。

## 什么是蓝牙乐音响？

[蓝牙低能耗音频](https://www.xda-developers.com/bluetooth-sig-introduces-le-audio-lc3-codec-support-multi-stream-audio-hearing-aids-audio-sharing/)去年由蓝牙 SIG 在 CES 2020 上宣布，作为蓝牙低能耗音频传输的新标准。该标准独立于蓝牙 5.1 和蓝牙 5.2，尽管蓝牙 5.2 包括使 BLE 音频成为可能的基石(同步信道)。

蓝牙 LE Audio 允许设备通过低能量频谱传输声音。它利用了一种新的压缩算法，称为低复杂度通信编解码器(LC3)，将保持与您目前从蓝牙获得的相同的高音频质量。得益于此，制造商将能够开发出播放时间几乎是目前两倍的设备，而不会牺牲音频质量。

此外，BLE 音频还包括对助听器的支持，将蓝牙音频的好处带给需要助听器的人。

## 哪些音频设备支持蓝牙 LE 音频？

对于支持蓝牙 LE 音频的音频设备(称为音频接收器)，它需要具有支持 LE 音频配置文件的更新的蓝牙芯片。

去年年底，高通推出了面向中端和入门级 TWS 耳塞的 QCC305x 芯片，该芯片将支持蓝牙 LE 音频。该芯片还增加了对其他高级音频技术的支持，但在本文的背景下，蓝牙 le 音频是其亮点之一。

## 哪部智能手机支持蓝牙 le 音频

蓝牙 LE 音频支持是通过[高通 FastConnect 6700 和 FastConnect 6900 芯片](https://www.xda-developers.com/qualcomm-fastconnect-6900-fastconnect-6700-wifi-6e-bluetooth-5-2-high-end-android-devices/)添加的，这是智能手机的组合 WiFi 和蓝牙芯片。

在其他功能中，FastConnect 6900 和 FastConnect 6700 芯片为 Android 智能手机带来了蓝牙 5.2。这些芯片也是蓝牙乐音频就绪。所以如果你的智能手机有这两个芯片中的任何一个，就满足了你享受蓝牙 LE 音频所需的条件之一。

请注意，这些 combo 芯片没有集成到骁龙 SOC 中。正因为如此，简单地拥有一个配备骁龙 888 SoC 的高端设备并不一定能保证手机支持蓝牙 LE 音频。这款手机需要安装一个支持这项新技术的蓝牙芯片，如果它是一款高端设备，这种情况更有可能发生——它只是不能保证自己安装一个特定的 SoC。

## Android 12 的蓝牙 LE 音频 API 意义如何？

FastConnect 6900 和 6700 芯片带来了支持蓝牙 LE 音频的音频源。QCC305x 芯片支持这项新技术，带来了音频接收器功能。现在，Android 操作系统支持音频配置文件，完成了这个等式。

请记住，Bluetooth LE Audio 的新 LC3 编解码器不会对每 see 的音频质量有太大的改善。相反，它将有助于提高电池寿命和信号强度。这将为大多数用户带来更好的用户体验。