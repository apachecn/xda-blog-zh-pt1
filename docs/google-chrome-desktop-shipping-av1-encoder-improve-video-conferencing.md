# 谷歌桌面版 Chrome 将推出 AV1 编码器来改善视频会议

> 原文：<https://www.xda-developers.com/google-chrome-desktop-shipping-av1-encoder-improve-video-conferencing/>

谷歌桌面版 Chrome 正在接受一项重要功能，该功能将提升超慢速互联网连接上的视频通话体验。在最新的 [Chrome 90 beta](https://blog.chromium.org/2021/03/chrome-90-beta-av1-encoder-for-webrtc.html) 中，谷歌推出了 AV1 编码器，使用该编码器可以提高视频质量，并显著提高基于 WebRTC 的视频会议应用的屏幕共享效率。

作为背景，AV1 是一种免版税的开源视频编解码器，在很大程度上被视为大多数视频流媒体服务使用的 H.264/AVC 编解码器的替代品。它声称比其前身 VP9 以及 H.264 和 H.265 编解码器提供更好的压缩效率和更好的视觉质量。与 H.264 编码的内容相比，AV1 编码的内容通常以较小的文件大小保持较高的质量

同时，WebRTC 是一个支持浏览器间实时通信的框架。它被用于许多基于网络的视频会议平台，包括 Google Meet、Facebook Messenger、Discord 等等。

要播放 AV1 编码的内容，您需要安装 AV1 解码器。然而，早在两年前发布的 Chrome 70 上，谷歌桌面 Chrome 就配备了 AV1 解码器。随着最近 AV1 编码器的加入，基于 WebRTC 的实时会议客户端，如 Google Meet 和 Google Duo，可以开始以 AV1 编码视频，然后将其传输到另一端。谷歌表示，通过利用编码器，Chrome 现在可以在慢至 30Kbps 的连接上进行视频通话。

用于 WebRTC 的 [AV1 编码器正在 Chrome 90 beta 中推出。稳定的 Chrome 浏览器中还没有，但在未来的版本中应该会很快出现。如果你的互联网连接速度很慢，并且对新编码器的改进感兴趣，你可以从](https://www.chromestatus.com/feature/6206321818861568)[这里](https://www.google.com/intl/en_in/chrome/beta/)下载最新版本的 Chrome beta。

谷歌已经在 Android 上的谷歌 Duo 应用程序中实现了 [AV1 编解码器。它还计划为一系列其他谷歌产品](https://www.xda-developers.com/google-duo-av1-moment-screenshots-saving-messages/)添加[支持，包括 Stadia、Photos、Meet 和 TV。](https://www.xda-developers.com/google-av1-codec-improve-bandwidth-stadia-photos-meet-tv/)