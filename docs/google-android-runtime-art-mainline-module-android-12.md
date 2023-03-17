# 谷歌将把 Android 运行时(ART)作为 Android 12 的主线模块

> 原文：<https://www.xda-developers.com/google-android-runtime-art-mainline-module-android-12/>

[项目主线](https://www.xda-developers.com/android-project-mainline-modules-explanation/)是 Android 近年来最大的变化之一。虽然你作为消费者可能没有注意到这一变化，但它从根本上改变了 Android 作为开源操作系统的运作方式，现在谷歌手中的权力比以往任何时候都多。这种控制权的增加是好是坏是另一个辩论的话题。现在，谷歌计划将 Android 运行时(ART)作为可更新的主线模块包含在 [Android 12](https://www.xda-developers.com/android-12/) 中。

## 什么是 Android 运行时(ART)？

Android Runtime，或 ART，是 Android 上的默认运行时，它是在 2013 年与 Android 4.4 Kitkat 一起推出的。正如谷歌提到的，ART 是“Android 上的应用程序和一些系统服务使用的*托管运行时”。这是 2014 年的一段 XDA 电视视频，它参照从前的达尔维克 VM 带来的变化来解释艺术:*

长话短说，ART 本质上是将 Android 应用的字节码翻译成本机指令。它使用提前编译，在安装时直接将应用程序编译成本机代码。正如你所猜测的，这是一个非常重要的功能，理想情况下应该在整个 Android 生态系统中以相同的方式执行。

## 艺术作为主线模块

正如 XDA 知名开发者 [*luca020400*](https://forum.xda-developers.com/member.php?u=5778309) 所发现的，一位[谷歌工程师透露](https://android-review.googlesource.com/c/platform/system/sepolicy/+/1465897/20#message-bd9ae7aa989c8ab3feda9bddcc6b1b347e090e7e)该公司计划将 Android 运行时(ART)作为 Android S/Android 12 中一个可更新的主线模块。

通过让 ART 成为主线模块，谷歌将能够对它进行更多的控制，这符合主线模块的总体主题。正如我们在项目主线的[主要讲解者中提到的:](https://www.xda-developers.com/android-project-mainline-modules-explanation/)

项目主线延伸了项目三重的努力。虽然 Treble 降低了原始设备制造商对 SoC 供应商进行每一次操作系统更新的依赖程度，但 Mainline 降低了谷歌对原始设备制造商提供关键操作系统组件安全更新的依赖程度。Project Mainline 将三重理念扩展到 Android 框架的更关键部分，将 OEM 从这个等式中移除。Project Mainline 的目的是让 Google 从原始设备制造商手中夺取对安全性和维护开发一致性至关重要的框架组件和系统应用程序的控制权。Project Mainline 被恰当地称为自 Project Treble 以来对 Android 的最大改变。

ART 作为一个主线模块将允许谷歌更新它，而不需要系统 OTA 更新。如果谷歌强制要求原始设备制造商预装谷歌签名的 ART 模块(很可能以 APEX 的形式交付)，那么谷歌将能够保留在所有 Android 设备上推送 ART 更新的控制权。谷歌将能够通过谷歌 Play 商店推送对 ART 的更新，而原始设备制造商将无法对 ART 进行修改。这反过来又会逐步实现第三方应用开发者所期望的整个生态系统的行为一致性。