# 下载并安装最新的 GApps: Open GApps、NikGApps、FlameGApps 等等

> 原文：<https://www.xda-developers.com/exodrive-brings-sd-card-support-to-everyone/>

GApps(Google Apps 的缩写)包在 Android 售后开发社区中是必不可少的。它们是为[定制 rom](https://www.xda-developers.com/most-popular-custom-roms-android/)专门制作的可选插件，可用于在您的设备上获取 Google 应用程序，如 Google Play 服务和 Play Store。如果你想知道如何在你的设备或[最好的安卓手机](https://www.xda-developers.com/best-android-phones/)上选择和安装正确的 GApps 包，这个指南应该可以帮助你。

## 为什么是 GApps？

谷歌要求每一个 Android 设备制造商遵循[兼容性定义文件](https://source.android.com/compatibility/cdd) (CDD)通过[兼容性测试套件](https://source.android.com/compatibility/cts/) (CTS)，这样他们就可以[允许他们的设备预装谷歌应用和服务](https://www.xda-developers.com/google-blocks-gapps-uncertified-devices-custom-rom-whitelist/)。然而，定制 ROM 开发者不能轻易地将这些谷歌应用和服务与他们的构建捆绑在一起。由于这些应用程序没有使用 Apache 或 GPLv2 许可证，将它们捆绑在 ROM 中存在法律挑战。

这正是 GApps 软件包的用武之地。GApps 维护人员依赖于构建脚本，这些脚本允许定期自动创建新的更新包。另一方面，ROM 开发者通常以这样一种方式构建定制 ROM，即最终用户可以在其构建的基础上闪存第三方 GApps 发行版，并无缝地获得使用谷歌 Play 商店或任何其他需要 Google Play 服务的应用程序的能力。

请记住，谷歌应用程序不需要启动或运行大多数定制的 rom。然而，许多用户发现它们有利于充分利用 Android 生态系统。

## GApps 的变体

对于一个普通用户来说，一堆第一方谷歌应用已经逐渐成为 Android 功能或外观和感觉的一部分。然后是那些喜欢绝对简约的设置，认为几乎所有东西都是臃肿的软件的人。

因为很难找到一个通用的解决方案，所以 GApps 维护者通常会提供几个版本。这就是为什么您可以找到带有“pico”、“basic”、“full”和类似标签的 GApps 包。当然，Play Store 以及强制性的 Play 服务和相关库是它们之间的共同组成部分，但捆绑的第一方谷歌应用程序的数量是关键的差异化因素。

与旧版本 Android 的兼容性是 GApps 场景中另一个有趣的方面。即使在定制 rom 的帮助下，也不是所有设备都可以运行最新和最棒的 Android 版本，这就是为什么有必要保持对旧版本的支持。此外，一些低级库依赖于 CPU 架构，所以主流维护者有时也会提供特定于架构的构建。

## 流行的 GApps 发行版

多年来，许多不同的 GApps 发行版已经流行起来。以下是售后市场开发社区中一些最受欢迎且积极维护的 GApps 产品。

### 开放式间隙

Open GApps 项目可能是在定制 rom 上下载谷歌应用程序的最受欢迎的选择，它始于 2015 年，是 ParanoidAndroid GApps 的精神继承者。这个发行版的代码库已经被分叉了无数次，这都要归功于项目的多功能性、广泛的文档和对遗留 Android 版本的丰富支持。

*   **安卓版本支持:**安卓 4.4 KitKat 到安卓 11。维护者也为 Android 12 和 [Android 12L](https://forum.xda-developers.com/posts/86595145) 提供测试包[。](https://forum.xda-developers.com/posts/85928131)
*   **平台支持:** Arm，Arm64，x86，x86-64。
*   **变体:**
    *   Pico :这个软件包是为那些希望获得绝对最小的 GApps 安装的用户设计的。
    *   Nano :这个包是为那些希望尽可能减少谷歌足迹，同时仍然享受原生的“Okay Google”和谷歌搜索支持的用户设计的。
    *   [Micro](https://github.com/opengapps/opengapps/wiki/Micro-Package) :这个包是为那些拥有小系统分区的传统设备的用户或者那些喜欢极简方式的用户设计的。
    *   [Mini](https://github.com/opengapps/opengapps/wiki/Mini-Package) :这个包是为那些使用有限的 Google apps 或者喜欢自己安装应用的人设计的。
    *   [Full](https://github.com/opengapps/opengapps/wiki/Full-Package) :如果你更喜欢使用股票/AOSP 应用程序，这个软件包就是为你设计的。
    *   [股票](https://github.com/opengapps/opengapps/wiki/Stock-Package):这个包包含了 Pixel 智能手机标配的所有谷歌应用。
    *   [超级](https://github.com/opengapps/opengapps/wiki/Super-Package):这个包是给那些想拥有所有谷歌应用的人的。它包括谷歌设备上发布的所有谷歌应用程序。
    *   Aroma 包是常规“超级”包的一个特殊版本，但是有一个图形化的前端，允许你选择安装(或不安装)哪些特定的应用程序，而不必手动编写一个 gapps-config 文件。
    *   [TVStock](https://github.com/opengapps/opengapps/wiki/TVStock-Package) :这个包是针对 Android 电视设备的。它包括 Nexus Player 标配的所有谷歌应用。
    *   TVMini:适用于 Android 电视设备的一套较小的谷歌应用程序，类似于 Mini 相对于 Stock variant 的应用程序。

### NikGApps

NikGApps 是另一个功能丰富的 GApps 发行版，它为高级用户提供了广泛的定制选项。由 XDA 资深会员 [Nikhil](https://forum.xda-developers.com/m/nikhil.4867515/) 创建，这个 GApps 项目最显著的特点之一是它专门为低端设备提供的 Android Go 包。与其他发行版不同，它还允许您随时刷新软件包。

最后但同样重要的是，用户可以将他们的定制配置上传到项目的存储库中，以创建个性化的构建。

*   **安卓版本支持:**安卓 10 到安卓 13。
*   **平台支持:** Arm64。
*   **变体:**
    *   核心:运行 Play Store 所需的最低 Google Apps 集。
    *   基本:核心的一切，加上谷歌运营商服务，谷歌拨号器(取代 AOSP 拨号器)，谷歌信息(取代 AOSP 信息)，谷歌联系人(取代 AOSP 联系人)等。
    *   Omni:一切从基本，加上 Gmail(取代 AOSP 电子邮件)，谷歌/像素设置向导，谷歌照片(取代 AOSP 画廊)等。
    *   股票:Omni 的一切，加上谷歌录音机，谷歌标记，谷歌声音，谷歌壁纸等。
    *   全:一切从股票，加上谷歌浏览器(取代 AOSP 浏览器)，谷歌助手，安卓汽车等。
    *   Go:面向低端设备。核心变体的略微增强版本。

### 火焰间隙

以前被称为 ExLiteGApps，FlameGApps 项目是 XDA 资深成员 ayandebnath 的创意。由于发行版的模块化设计，最终用户可以安装各种组件，如带有设备个性化服务的 Pixel Launcher、带有助手的 Google Search 以及使用官方附加包的设备个性化服务。

*   **安卓版本支持:**安卓 10 到安卓 12/12L。Android 13 还没有官方支持，尽管开发者[发布了一个金丝雀版本](https://sourceforge.net/projects/flamegapps/files/arm64/canary/android-13/)用于测试。
*   **平台支持:** Arm64。
*   **变体:**
    *   基本:包括核心 GApps，如 Google Play 服务(GMS)、Google 服务框架(GSF)、谷歌 Play 商店和其他基本组件。
    *   全面:包括所有必要的核心应用程序，更有用的如谷歌拨号器，谷歌联系人，谷歌信息等。

### BiTGApps

XDA 资深会员 [TheHitMan](https://forum.xda-developers.com/m/thehitman.8569961/) 的 BiTGApps 不到 90MB，是一个独特的极简发行版。除了极简主义，它还提供了一些独特的功能，例如为所有谷歌应用程序启用电池优化，从引导系统直接安装的能力，以及作为 Magisk 模块以无系统的方式安装。

*   **安卓版本支持:**安卓牛轧糖(7.1)到安卓 13。
*   **平台支撑:** Arm，Arm64。
*   **变体:**
    *   标准:目标是坚持能够提供适当的 Google 服务功能的最小设置。这个变体也支持无系统模式，前提是您已经通过 Magisk 获得了 root 访问权限。
    *   定制:如果你想坚持简单的基于旧系统的闪存，那么你可以选择基本，泛光灯，股票，全套。成分与 NikGApps 相似。

### 文学应用

LiteGApps 由 XDA 资深成员 [Wahyu6070](https://forum.xda-developers.com/m/wahyu6070.9507265/) 创建，是一个独特的发行版，涵盖了各种各样的用例。您可以通过恢复或作为 Magisk 模块安装它。

*   **安卓版本支持:**安卓 5.0 棒棒糖到安卓 13。
*   **平台支撑:** Arm，Arm64。
*   **变体:**
    *   Original:它提供了以下子变量:Lite、Basic、Core、Go、User、Basic、Nano、Micro 和 Pixel。其组成类似于开放的 GApps。
    *   Plus-Plus:您可以使用“Plus-Plus”变体来服务常规版本以及 LTS 版本(遗留 Android 版本)和 MicroG 版本。

### MagiskGapps

起源于 NikGApps 的一个分支，由[wack 1805](https://github.com/wacko1805)开发的 MagiskGapps 是一个完全无系统的 Google apps 发行版。它可以用来无缝地更改另一个 GApps 发行版的现有安装，而无需清除系统分区。

*   **安卓版本支持:**安卓 11 到安卓 13。
*   **平台支持:** Arm64。
*   **变体:**
    *   GMS:只有必要的谷歌服务和同步组件。
    *   核心:在 GMS 包上面玩商店。
    *   基本:除了核心软件包，还有一些应用程序，如谷歌拨号器、信息和联系人。
    *   股票:全像素风格的应用程序。

### MindTheGapps

由 LineageOS 贡献者 Alessandro Astone，又名 XDA 资深会员 [aleasto](https://forum.xda-developers.com/m/aleasto.4742143/) 维护的 MindTheGapps 是另一个紧凑的 Gapps 发行版。这个在社区中特别出名，因为它是由[linegeos](https://www.xda-developers.com/five-reasons-xda-loves-lineageos/)团队为其定制 ROM 正式推荐的 GApps 解决方案。

*   **安卓版本支持:**安卓 10 到安卓 13。你也可以找到 Android TV 的单独包。值得注意的是，它还托管了 Android 9 Pie 和 Android 8.1 Oreo 的遗留包。
*   **平台支持:** Arm，Arm64(也支持 x86，但只支持传统 Android 版本)。
*   **变体:**无。只有一种没有定制选项的变体。它提供了使用谷歌系统所需的一切，仅此而已。

## 如何安装 GApps

### 下载和准备

在安装 GApps 包之前，您需要选择与目标设备的 CPU 架构和您想要的定制 ROM 的 Android 基础相匹配的版本。请记住，一些原始设备制造商故意在 Arm64 设备上提供 Arm32 固件，因此请咨询定制 ROM 维护者以确定平台兼容性。如果你要闪存一个集成了 Google apps 的定制 ROM，那么你不需要安装一个独立的 GApps 包。

要了解 CPU 架构，请使用设备上的终端模拟器应用程序运行以下命令:

```
 getprop ro.product.cpu.abi 
```

粗略地说，如果你有一部相当新的智能手机，并且你打算安装一个基于 Android 13 的[定制 ROM，从前面提到的列表中下载一个用于](https://www.xda-developers.com/android-13-custom-rom-list/) [Android 13](https://www.xda-developers.com/android-13) 的 Arm64 GApps。

我们将假设您已经安装了像 TWRP 这样的自定义恢复，并且(可选)拥有实际刷新过程的 root 访问权限。如果没有，我们有关于如何给你的安卓设备安装根的指南和关于如何安装 TWRP 的指南。

### 来自 TWRP 的闪光信号

**警告:**大部分情况下，GApps 包在第一次引导进入自定义 ROM 之前必须进行闪存！总是建议进行工厂重置和格式化数据，以清除先前安装的 GApps 发行版的任何可能残留。

1.  确保你的电脑有 ADB 和 Fastboot。设置说明可在[这里](https://www.xda-developers.com/install-adb-windows-macos-linux/)找到。
2.  在你的电脑上下载**自定义 ROM 包**和**匹配 GApps 包**。
3.  使用适当的组合键或 ADB: `adb reboot recovery`将目标设备重新引导至恢复模式
4.  现在点击**清除** *、* **恢复出厂设置**，最后点击**格式化数据**继续清理过程。这将取消加密并删除存储在内部存储器中的所有文件。
5.  返回主菜单。
6.  侧装自定义 ROM ZIP 包:
    *   在目标设备上，选择**高级**，然后选择 **ADB 侧载**开始。
    *   在主机上，使用`adb sideload filename.zip`从侧面装载包装

7.  无需重启，点击返回按钮，然后对 GApps 包重复相同的过程:`adb sideload gapps.zip`
8.  目标设备上的 TWRP 屏幕应显示安装进度。
9.  一旦你成功安装了所有东西，点击**重启系统**按钮。

### 确认

如果一切顺利，你应该在重启后准备好谷歌应用和服务。

 <picture>![LineageOS 18.1 with NikGApps](img/b50fc637b8e4698e10be4fa6eb6afa27.png)</picture> 

A LineageOS installation with GApps

大多数 GApps 发行版和定制 ROM 支持 OTA 生存，这意味着当你安装 ROM 更新时没有必要刷新 GApps 包。不过，主要版本更新是另一回事，因为你必须为新的 Android 基础找到合适的 GApps 包，并在必要时进行全新安装。