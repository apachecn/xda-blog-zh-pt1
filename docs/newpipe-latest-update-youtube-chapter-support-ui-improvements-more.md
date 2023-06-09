# 最新的 NewPipe 更新带来了 YouTube 章节支持和更多！

> 原文：<https://www.xda-developers.com/newpipe-latest-update-youtube-chapter-support-ui-improvements-more/>

NewPipe 是一个受欢迎的、[开源 YouTube 客户端](https://www.xda-developers.com/newpipe-0-20-3-improves-youtube-video-loading-speed-adds-two-finger-swipe-gesture/)，刚刚更新到 v0.20.10，带来了几个新功能、UI 改进和错误修复。对于那些不了解情况的人来说，NewPipe 是不喜欢 YouTube 官方应用程序或没有安装 Google Play 服务的用户的替代选择。简单来说，NewPipe 解析 YouTube 网站提取数据，播放视频，但是没有限制，也没有广告。

NewPipe 的[新更新](https://newpipe.net/blog/pinned/release/newpipe-0.20.10-released/)的主要亮点之一是支持 [YouTube 章节](https://www.xda-developers.com/youtube-test-video-chapters-jump-forward-parts/)，这是谷歌去年 5 月推出的一项功能。章节让用户可以快速跳转到给定视频的特定部分，而不必摆弄搜索栏。在最新的更新中，NewPipe 现在也支持这一新功能，用户可以在视频播放器中单击章节按钮，打开内容创建者选择的章节列表。

另一个值得注意的变化是在按钮行中添加了两个新按钮，允许用户在浏览器中打开视频或与其他应用程序共享视频。您还可以添加第三个“播放 Kodi”按钮，将视频直接传输到 Kodi。现在底部还有一个新的标签布局，可以让你轻松地在评论、相关视频和视频描述之间跳转。

最后，更新还为 PeerTube 添加了一个名为 [Sepia Search](https://framablog.org/2020/09/22/sepia-search-our-search-engine-to-promote-peertube/) 的新搜索引擎。点击搜索栏右侧的三点菜单可以进入 Sepia Search，它可以更容易地发现 PeerTube 上发布的视频，peer tube 是一个免费的分散式视频共享平台。

那些已经在 Android 设备上使用 NewPipe 应用程序的人应该会收到更新提示，告诉他们下载最新版本。如果你还没有收到提示或者是新用户，你可以从 Team NewPipe 的 GitHub 页面[这里](https://github.com/TeamNewPipe/NewPipe/releases)下载最新版本。

以下是 NewPipe o.20.10 的完整变更日志:

*   **新**
    *   [YouTube]增加了对播放器控件中章节的支持
    *   向视频细节片段添加了辅助控制面板和选项卡
    *   [PeerTube]添加了棕褐色搜索
*   **改进后的**
    *   如果亮度手势被禁用，则禁用恢复亮度
    *   更新显示的许可证
    *   使用 Android 系统 WebView 时禁止向 Google 发送指标
    *   在全屏播放器中用硬件空间按钮切换播放/暂停
    *   添加列表项以在 Kodi 上播放视频。
    *   VideoDetailFragment:在 tablet UI 中旋转时不要退出全屏
    *   更新了令人反感的实例列表
    *   减少 API 对新管道更新检查的请求
*   **固定**
    *   修正了不播放带有时间戳的网址
    *   修复了播放按钮方法中的空指针异常
    *   动态获取包名，修复安装多个新管道的问题。
    *   修正了队列活动中错误的速度指示器
    *   修正了没有设置默认浏览器时的崩溃，并改进了共享对话框(在某些设备上)