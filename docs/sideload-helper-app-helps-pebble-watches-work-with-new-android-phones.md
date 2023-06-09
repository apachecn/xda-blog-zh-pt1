# 该应用程序帮助 Pebble 手表与新的 Android 手机配合使用

> 原文：<https://www.xda-developers.com/sideload-helper-app-helps-pebble-watches-work-with-new-android-phones/>

Pebble 是 2012 年在 Kickstarter 上推出的首批现代智能手表之一。它因其超长的电池寿命、庞大的应用程序库和开放的软件而广受欢迎，后来又推出了几款型号。Pebble [在资金耗尽后于 2016 年](https://web.archive.org/web/20161207152451/https://blog.getpebble.com/2016/12/07/fitbit/)关闭，但此前该公司更新了手表，以便在没有中央服务器的情况下继续运行。社区运营的“Rebble”项目继续通过更新软件保持手表的活力，现在 Rebble 发布了一个新的应用程序，以保持 Pebble 手表在新设备上的功能。

在 Pebble 关闭之前，Android 和 iOS 移动应用程序已经更新，允许从文件中下载 Pebble 应用程序。然而，Pebble 应用程序在现代 Android 设备上通常不被视为 Pebble 文件的处理程序，因此应用程序和 watchfaces 不容易转移到手表上。Pebble 的创始人埃里克·米基科夫斯基(Eric Migicovsky)最近甚至遇到了这个问题。

为了解决这个问题，Rebble 项目的开发人员爱丽丝·格雷和 T2·拉文德·格拉博创建了一个 Android 应用程序，名为 Rebble 的 Sideload Helper。该应用程序可以在现代 Android 设备上打开 Pebble 文件，然后将其传输到 Pebble 官方应用程序进行安装。

Rebble 博客写道，“除了侧装。pbw (watchface/watchapp)。pbl(语言)，和。pbz(固件)文件，该应用程序还处理 Rebble appstore 链接——事实上，如果用户设置了 Rebble Web 服务，它甚至可以翻译传统 Pebble appstore 链接。最后，该应用将有助于最终过渡到 Rebble 自己正在开发的移动应用。”

该团队表示，该应用程序仍需在更多语言中本地化，如果你准备好迎接挑战，现在有一个众包翻译的众包页面。与此同时，该应用程序在 Play Store 和 F-Droid 上都可以下载，[的源代码在 GitHub](https://github.com/pebble-dev/rebble-sideloader) 上。

https://f-droid.org/en/packages/io.rebble.charon/