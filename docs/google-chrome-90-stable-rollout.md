# Chrome 90 现在默认加载 HTTPS 版本，增加了 AV1 编码器

> 原文：<https://www.xda-developers.com/google-chrome-90-stable-rollout/>

谷歌 Chrome 90 现已在稳定频道推出。最新版本包含了许多在稳定频道中预览的功能和改进，包括支持 AV1 编码器，默认情况下将用户转发到 HTTPS 版本的网站等等。

首先，Chrome 90 中的地址栏(via[*Android Police*](https://www.androidpolice.com/2021/04/14/chrome-90/))现在默认为 HTTPS 版本。这意味着当你在地址栏输入一个网址时，Chrome 会默认将你转到 HTTPS 版本。只有当它找不到 HTTPS 版本时，它才会退回到 HTTP 版本。除了提高安全性和隐私性，这一新变化还将加快加密网站的初始页面加载时间，因为 Chrome 不再需要从 *http://重定向到 https://，*，这是早期版本中的默认行为。自今年年初以来，Chrome 一直在测试这一变化，谷歌[上个月承诺](https://www.xda-developers.com/google-chrome-default-https-version-90/)它将最终在稳定的 Chrome 90 版本中实现新的行为。

继续前进，Chrome 90 还获得了对 AV1 编码器的支持，这将大大提高基于 WebRTC 的视频会议应用程序在超慢互联网连接上的视频质量。上个月 Chrome 90 beta 版增加了对 [AV1 编码器的支持，现在稳定版已经上线。谷歌表示，AV1 编码器将允许用户在慢至 30Kbps 的连接上使用视频通话应用。](https://www.xda-developers.com/google-chrome-desktop-shipping-av1-encoder-improve-video-conferencing/)

谷歌在 Chrome 90 中测试的另一个有趣的变化是在网站上复制和粘贴文件的能力。新功能不再依赖拖放功能或使用文件选择器手动导航到文件路径，而是允许您将文件复制到剪贴板(Ctrl+c ),然后通过按 Ctrl+v 将其传输到网页。简单地说，您将能够在网站上附加和上传文件，就像您在文件夹之间复制粘贴文件一样。例如，如果你想在你的电子邮件中附加一个 PDF，只需复制文件并在邮件窗口中按 Ctrl+v。这项功能目前还没有在 Chrome 90 中开箱即用，但可以通过启用标志来试用:*Chrome://flags/# clipboard-filenames。*

除了上述变化，Chrome 90 还为 web 开发人员带来了许多改进和变化，如防止溢出的 CSS 新值，将功能策略重命名为权限策略，在 HTML 中实现影子 DOM 的新方法，等等。你可以在官方博客文章中详细阅读所有这些面向开发者的变化。

Chrome 90 已经开始在 Windows、Mac、Linux 和 Android 上推出稳定的渠道。