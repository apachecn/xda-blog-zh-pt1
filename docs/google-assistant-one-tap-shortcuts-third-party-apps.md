# Google Assistant 将很快从您喜爱的应用程序中添加一键快捷方式

> 原文：<https://www.xda-developers.com/google-assistant-one-tap-shortcuts-third-party-apps/>

谷歌助手今天在屏幕底部显示了一组动作建议，帮助你快速执行一个动作或了解更多关于响应的信息。例如，当我在我的设备上启动 Assistant 时，前两个操作建议是“我的购物清单上有什么”和“天气如何”，因为这是我问 Assistant 最多的两件事。根据在 [Google I/O 2021](https://www.xda-developers.com/google-io-2021-recap/) 上的“Android shortcuts for Assistant”演讲，谷歌正准备预览一项名为建议芯片的新功能，该功能基本上是深度链接到第三方应用程序的行动建议。

这些建议芯片将被放置在与助手 UI 底部的现有动作建议相同的位置。这项新功能建立在谷歌最近在 10 月份为助手添加的快捷支持之上。今天的第三方应用程序可以显示谷歌助手可以启动的快捷方式，但目前，这些快捷方式只能通过语音命令启动，一旦用户在助手设置中设置它们。有了新的建议芯片功能，用户只需轻轻一点，就可以进入到应用程序中相关页面的深层链接。例如，谷歌在助手中显示了一个“查看趋势”的快捷方式，当点击它时，会打开 Reddit 应用程序的趋势选项卡。

应用程序在其 shortcuts.xml 文件中定义的任何静态或动态快捷方式都将被 Google Assistant 读取，并在助手设置中自动显示给用户。该助手将根据使用模式主动向用户推荐快捷方式，开发者也可以在应用程序中添加快捷方式建议，建议用户在应用程序中添加快捷方式，而不是等待他们通过谷歌助手本身发现快捷方式。

此外，Android 12 解锁了 Android 的 ShortcutManager APIs 设置的限制。现在，开发者可以建立一个无限的快捷方式集，而不仅仅局限于 10 个。

最后，谷歌表示，它将把应用程序建议作为快捷方式显示在搜索栏下方。这可能会被捆绑到新的通用应用搜索功能中，谷歌[正在 Pixel Launcher 上测试](https://www.xda-developers.com/android-12-device-search-api-third-party-launchers/)。

您可以从 YouTube 观看 Android 快捷键助手的完整会话:

\ r \ nht TPS://www . YouTube . com/watch？v=zMs7DgniUqs\r\n