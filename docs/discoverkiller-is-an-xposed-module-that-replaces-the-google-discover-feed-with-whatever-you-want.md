# 探索黑仔用你想要的任何东西取代谷歌探索频道

> 原文：<https://www.xda-developers.com/discoverkiller-is-an-xposed-module-that-replaces-the-google-discover-feed-with-whatever-you-want/>

**更新 1 (08/18/2021 @ 12:57 PM ET):** 发现黑仔 mod 收到了一个重大更新，让你可以用嵌入式助手快照页面取代谷歌发现 feed。[点击这里了解更多信息。](#update1)文章发表于 2020 年 6 月 29 日，下面保留。

谷歌 Pixel 系列和许多其他运行接近库存版本 Android 的智能手机上的默认启动器应用程序提供了与[谷歌发现](https://www.xda-developers.com/google-discover-dark-theme-pixel-launcher/)的便捷集成。作为 Google Feed 的继任者[，Discover 的启动器集成允许用户滑动到默认主屏幕的左侧，方便地访问最新的新闻报道、视频推荐等等。这一功能也被著名的 Android 皮肤版本所采用，如华硕的 ZenUI、](https://www.xda-developers.com/google-feed-rebrand-discover/)[小米的 MIUI](https://www.xda-developers.com/miui-launcher-hidden-google-discover-integration/) 和[一加的 OxygenOS](https://www.xda-developers.com/oneplus-launcher-google-discover-not-shelf-oneplus-8/) 。然而，一些用户抨击谷歌在 Discover 中显示 clickbaity 内容，同时在 feeds 中显示广告。

XDA 知名开发者 Quinny899 现在提出了一个有趣的模式“用你想要的任何东西替换你主屏幕上的谷歌发现页面”。被称为**发现黑仔**的 mod 以一个曝光模块的形式出现。启用后，该模块可以用谷歌助手的“更新”屏幕或几乎任何其他第三方应用程序无缝替换发现页面，这取决于您如何定制它。

Discover 部分由 Google app 提供支持，因此该模块直接挂钩到它而不是启动器。这种设计允许黑仔探索与任何能够显示谷歌探索提要的第三方启动器兼容，无需额外配置。如果您选择显示“更新”屏幕而不是“发现”页面，该模块还提供向右滑动关闭选项。

作为使用该模块的强制性先决条件，您需要在使用 Magisk 启动您的设备后安装带有 Riru Core 的 [EdXposed。注意,《发现黑仔》的最初版本并没有经过](https://www.xda-developers.com/xposed-framework-unofficial-port-android-pie/)[太极](https://taichi.cool/doc/)的验证。你可以从它的 XDA 线程(下面链接)下载该模块的预编译 APK，而源代码是在开发者的 GitHub 概要文件上可以获得的[。](https://github.com/KieronQuinn/DiscoverKiller)

**[发现黑仔曝光模块— XDA 下载讨论线程](https://forum.xda-developers.com/xposed/modules/app-discoverkiller-replace-google-t4120997)**

* * *

## 更新 1:发现从头重写的黑仔

经过一年多的开发，XDA 认可的开发者 Quinny899 发布了一个 T2 的新更新 T3。这个 Xposed 模块的 2.0 版本已经从头开始重写，不再使用模糊的类名或字段名，这应该希望意味着它不需要不断更新来跟上谷歌应用程序的更新。更新的另一个重要功能是支持嵌入谷歌助手快照页面，这可能是主屏幕上谷歌发现“减一”页面的最佳替代。当然，你仍然可以用其他任何东西替换发现页面，包括其他应用程序。在运行 [Android 12](https://www.xda-developers.com/android-12/) 的设备上，由于新的闪屏功能，应用程序的启动看起来几乎是无缝的。

想了解更多关于探索黑仔 mod 的信息，请查看 XDA 论坛上 Quinny899 的[帖子。你可以从论坛线程或者](https://forum.xda-developers.com/t/app-xposed-16-08-discover-killer-replace-the-google-discover-page-on-your-home-screen.4120997/#post-85489853)[项目的 GitHub 页面](https://github.com/KieronQuinn/DiscoverKiller)下载该模块。