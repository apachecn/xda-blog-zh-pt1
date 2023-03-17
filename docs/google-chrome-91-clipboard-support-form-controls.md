# 谷歌 Chrome 91 将为桌面应用程序带来剪贴板支持，Android 上的新表单控件 UX

> 原文：<https://www.xda-developers.com/google-chrome-91-clipboard-support-form-controls/>

谷歌[最近在稳定频道推出了](https://www.xda-developers.com/google-chrome-90-stable-rollout/) Chrome 90，并为桌面和移动用户引入了大量新功能。更新后，浏览器现在默认加载 HTTPS 版本的网站，它包括 [AV1](https://www.xda-developers.com/av1-future-video-codecs-google-hevc/) 编码器支持，并且它给你一个新的选项，让你可以直接将[链接到网页上高亮显示的文本](https://www.xda-developers.com/google-chrome-90-share-highlighted-text-web-pages/)。除了这些功能，谷歌还在更新中包括了一些正在开发的功能，如带有实时价格下跌警报的[价格跟踪功能](https://www.xda-developers.com/google-chrome-90-price-tracking/)，它可能会在未来的版本中推出。虽然这些功能可能会也可能不会在 Chrome 91 中推出，但谷歌现在已经详细介绍了一些其他功能，这些功能将在下一个稳定的 Chrome 更新中上线。

在 Chromium 博客上最近的一篇文章中，该公司详细介绍了 Chrome 91 将推出的一些新功能和变化。该更新目前在测试版中可用，它包括以下更改:

### 桌面应用程序的剪贴板支持

Chrome 91 将给予桌面应用程序对剪贴板的只读访问权限。该功能将允许用户使用剪贴板键盘快捷键，如 Ctrl+C 和 Ctrl+V，将文件附加到电子邮件中，而不是仅仅依靠拖放方法。该功能在 Chrome 91 测试版上是活的，但它隐藏在一面旗帜后面。如果你想尝试一下，你可以前往 *chrome://flags* 并启用“剪贴板文件名”标志。

启用标志后，单击右下角的“重新启动”按钮。完成后，您就可以使用 Ctrl+C 快捷键复制系统上的文件，并使用 Ctrl+V 快捷键将它们附加到电子邮件中。

### Android 上更新的表单控件

去年 1 月，我们在 Chromium 论坛上发现了一个帖子，详细描述了 Android 上谷歌 Chrome 中表单控件的[视觉刷新。根据新的博客帖子，更新后的表单控件 UX 将向 Android 版 Chrome 91 用户推出。与微软合作开发的 UX 将提供更好的可访问性和触摸支持，更好的黑暗模式支持等等。下图展示了新旧表单控件 UI 之间的差异。](https://www.xda-developers.com/google-chromes-form-controls-getting-revamped-ui-touch-support/)

关于更新后的 UX 的更多信息，请查看[这个 CDS 讲座](https://www.youtube.com/watch?v=ZFvPLrKZywA)或微软的[博客文章](https://blogs.windows.com/msedgedev/2019/10/15/form-controls-microsoft-edge-chromium/)。

### 杂项功能/变化

Chrome 91 还将包括 Origin 试用版，以帮助 web 开发人员尝试新功能，并向 web 标准社区提供可用性、实用性和有效性方面的反馈。您可以通过点击[此链接](https://web.dev/origin-trials/)了解更多关于 Origin Trials 的信息。更新还包括一个新的 GravitySensor 接口、桌面平台上的 SharedArrayBuffers、文件系统访问 API 的建议文件名和位置、对 WebOTP API 的跨源 iframe 支持等等。想了解更多关于这些变化的信息，请访问 [Chromium 博客](https://blog.chromium.org/2021/04/chrome-91-handwriting-recognition-webxr.html)。