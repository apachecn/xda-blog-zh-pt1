# OpenGApps 发布 Android 11 定制 rom 的谷歌应用包

> 原文：<https://www.xda-developers.com/opengapps-android-11-packages/>

没有多少人愿意在无法访问谷歌 Play 商店和其他谷歌应用的情况下使用安卓手机，这就是为什么大多数安卓手机都预装了谷歌应用。然而，由于谷歌应用是专有的，许多定制 ROM 开发者并不将它们与他们的构建捆绑在一起，所以他们反而告诉用户 flash 社区制作的谷歌应用捆绑包，通常被称为“GApps”包。XDA 最受欢迎的 GApps 包之一叫做 OpenGApps，项目背后的团队现在提供兼容 [Android 11 定制 rom](https://www.xda-developers.com/android-11-custom-rom-list/)的谷歌应用包。

兼容 Android 11 的谷歌应用包现在可以从 opengapps.org 网站获得。目前，所有四种受支持的架构(ARM、ARM64、x86 和 x86_64)仅支持“nano”和“pico”版本。这些软件包是最小的，因为它们只包含启动和运行谷歌 Play 商店、Google Play 服务和其他关键 Google 服务所需的最少内容。[据团队成员 nezorflame](https://forum.xda-developers.com/t/gapps-daily-open-gapps-for-android-all-android-versions-devices.3098071/page-353#post-85317791) 称，OpenGApps 团队仍在测试包含更多谷歌应用的更大版本，尽管你可以从 Play Store 下载大多数谷歌应用。然而，Android Auto 需要预装，这就是为什么最近的“pico”版本被更新为包括其存根包，Play Store 版本在其上更新。

OpenGApps 团队[在 2020 年 1 月发布了](https://www.xda-developers.com/open-gapps-android-10-roms/)兼容 Android 10 的谷歌应用包，比 Android 10 的稳定发布晚了 4 个月。兼容 Android 11 的谷歌应用程序包在 Android 11 稳定发布后 10 个月发布——这比以前的等待时间长得多——但请记住，该项目的**维护者都是志愿者**在空闲时间做这些工作，所以我们必须放他们一马，因为他们不欠我们任何东西。

虽然 OpenGApps 是最受欢迎和最知名的非官方 GApps 包，但在更新的 OpenGApps 包不可用时，定制 ROM 开发者向用户指出了其他受欢迎的 Google 应用包。例如，LineageOS 为 [LineageOS 18.1](https://www.xda-developers.com/lineageos-18-1-review/) 安装推荐 MindTheGapps，尽管[现在也在他们的](https://review.lineageos.org/c/LineageOS/lineage_wiki/+/313591) [wiki](https://wiki.lineageos.org/gapps.html) 中列出了open gaps。

至于为什么人们可能想要使用 OpenGApps，开发人员在支持多种架构方面做得很好，保持他们的 Google app 包最新，压缩他们的文件，并通过智能检查来构建他们的安装程序脚本，以确保兼容性，自动备份，以及[允许定制](https://github.com/opengapps/opengapps/wiki/Advanced-Features-and-Options)。将谷歌应用程序加载到 AOSP ROM 中并不像将应用程序复制到系统分区中那么简单——安装程序脚本还必须设置权限，添加覆盖，并做其他事情来确保应用程序正常运行。