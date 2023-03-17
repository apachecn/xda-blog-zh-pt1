# NewPipe 0.21.0 现在允许你从 Bandcamp 播放无数字版权管理的音乐

> 原文：<https://www.xda-developers.com/newpipe-0-21-0-stream-drm-free-music-bandcamp/>

广受欢迎的 Android 开源 YouTube 客户端 NewPipe 在过去几个月里一直在稳步增加新的特性和功能。在最近的更新中，应用程序[带来了对 YouTube 章节](https://www.xda-developers.com/newpipe-latest-update-youtube-chapter-support-ui-improvements-more/)的支持，几个 UI 改进，等等。现在，该应用程序正在进行全新更新，增加了对 Bandcamp 的支持，改善了整体用户体验，并修复了令人讨厌的错误。

NewPipe 0.21.0 的主要亮点是[对 Bandcamp](https://newpipe.net/blog/pinned/release/newpipe-0.21.0-released/) 的支持，Bandcamp 是一个在线音乐分发平台，允许用户购买、下载和流媒体播放他们喜欢的艺术家的音乐。从 [Bandcamp](https://bandcamp.com/) 购买的音乐是无数字版权管理的，这意味着你可以完全控制专辑和曲目，并可以自由下载和传输你的音乐到你喜欢的任何地方，不像 Spotify 和 iTunes 那样不允许你在他们的应用程序之外访问你的音乐。

在更新到 NewPipe 0.21.0 后，用户现在可以从下拉列表下的汉堡菜单中访问 Bandcamp 服务。像粉丝页面和评论这样的东西暂时还不支持，但是大部分基本的功能包括流媒体，搜索，广播等等都有。还支持下载，这是官方 Bandcamp 应用程序 T1 所没有的。

除了集成 Bandcamp，新的更新还增加了对基于系统主题自动更改应用主题的支持，通过硬件 space 按钮(通过蓝牙键盘或 scrcpy)播放/暂停视频的能力，在 SoundCloud 中选择 64Kbps 流媒体的能力等等。

如果你使用的是旧版本，你应该会在应用程序中收到一个提示，要求你下载 NewPipe 0.21.0。或者，你也可以从 [F-Droid](https://f-droid.org/) 或者 NewPipe 的 [GitHub 页面](https://github.com/TeamNewPipe/NewPipe/releases)下载最新版本。

新管道 0.21.0 的完整变更日志如下:

*   **新**
*   **改进后的**
    *   为应用程序添加了一个设置，以遵循设备主题。你也可以指定你是否希望你的深色主题只是黑色或漆黑一片。
    *   改进的错误面板和新的重试按钮
    *   该应用程序现在可以让你知道你无法打开的视频/音频是地理限制、年龄限制、私人、付费还是只对高级用户开放。
    *   添加了一个祝酒词来通知用户下载已经开始。
    *   添加了一个解决方法，使 NewPipe 能够在 SoundCloud 上播放 HLS 曲目。这实质上意味着除了通常的 128kbps MP3 流，您还可以选择播放 64kbps 的 Opus 流！
*   **固定**
    *   修正了有时候突然出现的缩略图太小的问题(呵呵，geddit？视频详细信息屏幕中的“突然出现”)。
    *   修正了在背景播放器中启动一系列流时，迷你播放器中显示的错误/空标题。
    *   修复了纵横比存储不正确的问题(适合/填充/缩放)。现在这就像用户期望的那样工作了。
    *   修复了与上面相同的错误，但适用于 Youtube 混合播放列表。
    *   修正了趋势信息亭的错误/无限加载。
    *   修正了 PeerTube 上的播放列表提取。