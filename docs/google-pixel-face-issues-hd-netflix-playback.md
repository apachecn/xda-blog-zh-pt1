# 一些谷歌像素用户面临高清网飞播放问题

> 原文：<https://www.xda-developers.com/google-pixel-face-issues-hd-netflix-playback/>

**更新 1(美国东部时间 04/09/2021 @ 05:50PM):**谷歌已确认意识到该问题，并正在积极为受影响的 Pixel 用户修复该问题。[点击这里了解更多信息。](#update1)文章发表于 2021 年 4 月 6 日，下面保留。

在最近的更新之后，许多谷歌 Pixel 手机用户报告了从 L1 将 Widevine 级别降级到 L3 的问题，导致受 DRM 保护的内容无法以高清分辨率播放。例如，网飞现在的上限是 540 便士。

许多用户向我们抱怨这个问题。Telegram 上的情报人员 argruar、HydroPetro 和 MSFJarvis 表示，他们在 Pixel 4a 和 Pixel 5 上遇到了这个问题。Tipster Devang Chhabria 将 Reddit 主题与一些报告相同问题的 Pixel 4a、Pixel 4 和 Pixel 5 用户联系起来。

与此同时，Pixel 论坛上的一个支持帖让用户抱怨这个问题。我们回顾了几个月前的 Reddit，实际上[发现人们](https://www.reddit.com/r/GooglePixel/comments/lvn17a/netflix_in_sd_quality_on_pixel_5/)已经[遇到高清网飞播放问题](https://www.reddit.com/r/GooglePixel/comments/jyta62/pixel_5_widevine_issue_preventing_hdhdr_content/)有一段时间了。一些用户表示，他们在 2021 年 4 月更新后遇到了这个问题，而其他人则报告说这个问题已经发生了几个月。

当手机降级到 Widevine L3 时，DRM 加密的内容不再在可信执行环境(TEE)中解码。在大多数情况下，Widevine 保护的内容只能以 480p 播放，这不是流媒体内容的最理想情况。

为了检查 Widevine DRM 级别，您可以[遵循本指南](https://www.xda-developers.com/check-widevine-drm-status-android/)。正如我们所报道的，大多数由谷歌认证的优质 Android 设备支持 Widevine L1，有时与其他 DRM 方法结合使用。但是，改装手机或未经认证的手机可能仅支持 L3 或 L2。软件更新也可能导致 Widevine DRM 恢复到 L2 或 L3。

像网飞这样的服务已经对所有像素设备进行了高清认证，这是 L1 的 Widevine，Pixel 3 及以上也获得了 HDR 的认证。目前还不清楚是什么导致了这个问题，用户似乎没有从谷歌那里得到任何具体的答案，无论这是否包括未来的软件修复或用户可以做的事情。

并非每个车主都遇到过这个问题。在同一个支持论坛上，一些 Pixel 4a 和 Pixel 5 用户声称他们仍然在 L1 上，所以它不会影响到每个人。但是为什么有些人会遇到这个问题，而有些人不会，这仍然不清楚。

* * *

## 更新 1:谷歌意识到并正在修复 Pixel 手机

谷歌已向 [*Android Police*](https://www.androidpolice.com/2021/04/09/some-pixels-are-experiencing-poor-netflix-quality-after-recent-updates-heres-how-to-check-if-youre-affected/) 证实，它已意识到用户报告的 Widevine DRM 级别降级至 L3 的问题。该公司正在积极研究受影响的 Pixel 手机的解决方案，但没有提供修复程序何时可用的确切时间表。显然，这个问题也可能影响到其他制造商的手机，所以它可能比预期的更广泛。