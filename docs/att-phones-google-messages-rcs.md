# 美国电话电报公司的安卓手机将使用谷歌信息进行远程控制

> 原文：<https://www.xda-developers.com/att-phones-google-messages-rcs/>

Rich Communication Services，简称 RCS，是 SMS 的继任者，SMS 是大多数运营商用于文本消息的协议。与 SMS 不同，RCS 支持高级消息功能，如群聊管理、更高质量的文件共享、阅读回执、键入指示符和[端到端加密](https://www.xda-developers.com/end-to-end-encrypted-google-messages/)。RCS 必须得到运营商网络、手机和手机消息应用的支持，毫不奇怪，运营商在采用新技术方面落后了。由于对运营商的缓慢采用感到失望，谷歌将自己的 RCS 服务融入了谷歌消息应用，并一直在推动运营商将其作为安卓手机上的默认消息服务。今天，AT & T 宣布网络上所有的 Android 手机将使用谷歌消息进行短信和 RCS。

今天早些时候，[*《The Verge》*](https://www.theverge.com/2021/6/30/22556686/att-android-phones-rcs-google-messages)首先分享了这一消息，并在[谷歌云博客](https://cloud.google.com/blog/products/workspace/att-android-customers-to-have-messages-app-by-default)上得到证实，在此之前，T-Mobile 在三月份也发布了类似的公告[。该声明意味着 AT & T 上的 Android 手机将默认带有谷歌消息应用，用于通过 SMS 和 RCS 发送短信。AT & T 有自己的 RCS Universal Profile 1.0 实现，名为 Advanced Messaging，但是](https://www.xda-developers.com/t-mobile-bets-big-on-google-services-and-pixel-phones/)[只有少数 Android 设备](https://www.xda-developers.com/att-list-of-compatible-phones/)——没有一部 iPhone——支持它。此外，AT & T 的实现不能与其他运营商互操作，这意味着拥有支持高级消息传递的手机的客户只能与拥有支持手机的其他客户进行消息传递。另一方面，Google Messages 中的 RCS 可以在所有 Android 设备上运行，并且不依赖于运营商，因为 Google 正在处理后端。

谷歌消息中的 RCS 可以通过下载应用程序并在设置中打开“聊天功能”来启用。如果您的设备受支持，该应用程序还会提示您打开聊天功能。目前，谷歌[还没有开放 API](https://www.xda-developers.com/google-rcs-api-3rd-party-apps/) 让第三方消息应用可以实现 RCS 支持，所以你现在必须使用谷歌消息应用。

威瑞森现在是美国唯一一家不使用谷歌消息发送短信和 RCS 的运营商。一旦他们这样做了，美国的安卓用户将最终有一个苹果 iMessage 的合适对手被植入他们的手机。(苹果尚未在 iOS 中采用 RCS 支持，鉴于 iMessage 在将用户留在围墙花园中的重要性，他们不太可能这样做。)采用 RCS 还将更好地保护用户的短信[不被运营商读取](https://www.xda-developers.com/carrier-injecting-ads-two-factor-sms/)，因为用户可以为每次对话开启端到端加密。