# 谷歌在 Android 中增加了一个超宽带(UWB) API

> 原文：<https://www.xda-developers.com/google-adding-ultra-wideband-uwb-api-android/>

**更新 1(美国东部时间 01/25/2021 @ 02:20PM):**谷歌在 [Android 12](https://www.xda-developers.com/android-12/) 发布时及时添加了支持超宽带传感器的 API，但它们可能不会用于第三方应用。[点击这里了解更多信息。](#update1)文章发表于 2020 年 11 月 10 日，下面保留。

自智能手机早期以来，我们一直依赖 Wi-Fi 和蓝牙无线技术来满足短程连接需求。超宽带(UWB)被广泛认为是无线技术领域的下一件大事，有望为智能家居设备提供高精度的室内定位和高速点对点数据传输。苹果的 iPhone 11 是第一款支持超宽带技术的现代智能手机。三星紧随其后推出了 Galaxy Note 20 和 Note 20 Ultra，成为第一家采用新技术的 Android OEM 厂商。小米还宣布了加入 UWB 技术的计划，[展示了它如何利用该技术](https://www.xda-developers.com/xiaomi-demos-intuitive-smart-home-controls-with-uwb-ultra-wide-band-technology/)控制其智能家居生态系统。随着未来几天越来越多的智能手机预计将采用这一新的无线协议，谷歌正在 AOSP 添加一个新的 API，以更好地支持未来 Android 智能手机上的 UWB 技术。

随着官方 Android API 的引入，开发人员将能够创建在不同的具有 UWB 硬件的 Android 智能手机上无缝工作的应用程序，而不是使用来自不同 OEM 的不同 API 集。

谷歌[合并了 Android 开源项目(AOSP)的多个提交](https://android-review.googlesource.com/q/UWB)，增加了一个超宽带(UWB) API。例如， [UwbManager 类](https://android-review.googlesource.com/c/platform/frameworks/base/+/1453876)“*提供了一种执行 UWB 操作的方法，例如查询设备的能力，确定本地设备和远程设备之间的距离和角度。*" API 实现遵循 [IEEE 针对低速率无线网络的 802.15.4z](https://standards.ieee.org/standard/802_15_4z-2020.html) 标准。

提醒一句:这个 API 仍在开发中，不能保证它能及时为 Android 12 准备好。仅仅因为这个 API 被添加到 Android 并不意味着下一个 Pixel 将配备 UWB 硬件。

如前所述，目前唯一拥有超宽带(UWB)硬件的 Android 设备是三星 Galaxy Note 20 和 Note 20 Ultra，唯一使用该硬件的应用程序是三星的 SmartThings 应用程序[，用于 SmartThings Find 功能](https://www.xda-developers.com/smartthings-find-helps-find-lost-samsung-galaxy-devices/)。

UWB 仍处于起步阶段，虽然它有很大的潜力，但它在现实世界中的实用性和应用还有待充分实现。

*由 [xnimrodx](https://www.flaticon.com/authors/xnimrodx "xnimrodx") 从 Flaticon* 制作的图标

* * *

## 更新 1:合并为系统 API

在上周晚些时候合并的提交中，谷歌将 Android 的超宽带 API 标记为 T2 系统 API T3。链接到 Android SDK 的第三方应用程序无法访问 SystemAPIs。因此，第三方应用程序将无法访问这些 API。尚不清楚为什么这些 API 仅限于系统应用程序，但有可能谷歌认为这些 API 还没有准备好供公众使用。谷歌对 RCS API 做了[类似的事情，第三方消息应用程序仍然无法使用。](https://www.xda-developers.com/google-rcs-api-3rd-party-apps/)