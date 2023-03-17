# 谷歌信息正准备让你把对话钉在顶部

> 原文：<https://www.xda-developers.com/google-messages-preparing-pin-conversations/>

在过去的几个月里，谷歌信息获得了几个新功能，包括[日历事件建议](https://www.xda-developers.com/google-messages-suggest-add-calendar-event/)，[预定信息支持](https://www.xda-developers.com/android-password-checkup-scheduled-messages/)，[自动 OTP 删除](https://www.xda-developers.com/google-messages-auto-otp-delete/)，一个[统一表情菜单](https://www.xda-developers.com/google-messages-unified-emoji-gifs-sticker-menu/)，以及一个[改进的三星手机用户界面](https://www.xda-developers.com/google-messages-galaxy-s21-one-ui-design/)。最重要的是，最近该应用程序的卸载表明，谷歌正在为该应用程序开发更多有用的功能，如用于平板电脑的分屏视图，支持使用配对手机发送消息，等等。虽然这些功能尚未在稳定频道上向用户推出，但我们现在已经在谷歌消息 8.1.050 的拆解中发现了更多即将推出的功能。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Google Messages 8.1.050 刚刚开始通过 Play Store 向用户推出。最新更新的拆卸揭示了指向两个新功能的新字符串——支持固定对话和标记特定消息的能力。新字符串表明，即将推出的锁定对话功能将允许您将对话锁定在对话列表的顶部，让您一打开应用程序就可以轻松访问它。

```
 <string name="action_pin_to_top">Pin to top</string>
<string name="action_unpin_from_top">Unpin from top</string>
<string name="pin_limit_message">You can pin up to %1$d conversations</string>
<string name="pin_success_message">Pinned %1$d of %2$d conversations</string> 
```

正如你在附件截图中看到的，这个应用程序可以让你锁定 3 个对话。但由于字符串包含一个变量值，谷歌可能会在该功能向用户推出时增加或减少固定对话的数量。

除了固定对话功能，我们还发现了指向即将推出的带星号的消息功能的新字符串。这些字符串表明，Google Messages 将很快让你为特定的消息加星，你将能够在以后通过应用程序的搜索功能找到加星的消息。

```
 <string name="action_search_starred_messages">Starred</string>
<string name="search_starred_messages_title">Starred</string>
<string name="star_badge_on_click_snackbar_action">Undo</string>
<string name="star_badge_on_click_snackbar_message">Star removed</string> 
```

字符串进一步表明，所有带星号的邮件都将显示一个新的星号标记，以帮助您快速识别它们，但我们不确定它将在最终版本中出现在哪里。一旦我们能够手动启用该功能，我们将立即分享截图。

请注意，这些功能在当前版本的 Google Messages 中不可用。一旦他们开始向用户推出未来的更新，我们将立即更新这篇文章。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*