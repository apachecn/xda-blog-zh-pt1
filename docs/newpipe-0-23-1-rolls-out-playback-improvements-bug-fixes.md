# NewPipe 0.23.1 推出了播放改进和几个错误修复

> 原文：<https://www.xda-developers.com/newpipe-0-23-1-rolls-out-playback-improvements-bug-fixes/>

# NewPipe 0.23.1 推出了播放改进和几个错误修复

最新版本的 NewPipe (v0.23.1)现在向用户推出，它带来了播放改进和几个错误修复。

NewPipe 开源 YouTube 客户端的开发者发布了该应用的新更新。由于 DASH 支持，最新版本(v0.23.1)带来了播放改进，以及几个错误修复。在一篇关于更新的博客文章中，该团队透露，DASH 支持应该会让应用程序感觉快很多。更新后，视频加载速度应该会更快，在搜索视频时，您应该会看到明显的性能改善。

除了 DASH 支持，NewPipe 0.23.1 修复了播放 YouTube 视频时的重复缓冲，允许用户查看最近结束的 YouTube 直播流，并引入了对更多分辨率和格式的支持。请查看下面的部分，了解最新版本中所有重大变化的列表。

**NewPipe 0.23.1 变更和 bug 修复**

*   现在，DASH 被用作 YouTube 播放的首选方式，而不是渐进式 HTTP，从而改善了播放和搜索的加载时间。这让 app 快了一个数量级！点击 YouTube 视频后无需再等待！
*   根据一些用户的说法，播放 YouTube 视频时重复缓冲似乎也已经成为过去的问题。
*   最近结束的 YouTube 直播现在可以从头开始播放了。
*   在 YouTube 中，现在可以播放更多的分辨率和格式。
*   修复了只有 HLS 流的 PeerTube 视频(即大多数 PeerTube 视频)上的查找。现在 PeerTube 终于可以用了！
*   修正了只有音频的 PeerTube 视频崩溃的问题。
*   修正了 SoundCloud HLS-only 音轨的播放。

这篇博客文章进一步补充说，尽管上面提到的大部分更改都是对 NewPipeExtractor 进行的，但该团队不会在发布最新更新的同时发布新版本的 NewPipeExtractor。此外，它指出，在更新之后，用户应该能够将远程播放列表转换为本地 NewPipe 播放列表。该版本还带来了一些改进和错误修复，您可以通过点击下面的源代码链接来了解它们。

NewPipe 是 YouTube 最先进的替代品之一。如果你还没有查看，你可以从项目的 [GitHub 页面](https://github.com/TeamNewPipe/NewPipe/)下载。

* * *

**来源:** [NewPipe](https://newpipe.net/blog/pinned/release/newpipe-0.23.1/)