# Android 12 Conversations widget 根据文本调整其背景

> 原文：<https://www.xda-developers.com/android-12-conversations-widget-background-change/>

就在几天前，谷歌向我们发布了 Android 12 的第二个测试版，它带来了新操作系统中最令人兴奋的功能之一:基于你的壁纸的变色背景。但是我们发现，Android 12 Beta 2 中还有很多[新功能，包括添加了期待已久的对话小工具。在玩这个新部件的时候，我们了解到它有一个隐藏的属性:它的背景可以根据消息的内容而改变！](https://www.xda-developers.com/android-12-beta-2-features/)

正如我们在[我们的实践总结](https://www.xda-developers.com/android-12-beta-2-features/#android12beta2_conversationswidget)中提到的，Android 12 Beta 2 中的 Conversations widget 显示了联系人的个人资料图片、姓名以及上一条消息的图标或内容。Twitter 用户 [Neil Rahmouni](https://twitter.com/neil_rahmouni) 提醒我们，消息中的某些文本可以触发对话小工具的背景变化。当用户收到包含两个或更多感叹号的消息时，小部件的背景突然变成充满半透明的感叹号。

我们确认了当消息包含 2 个或更多感叹号时，对话小部件确实会改变其背景。我们还发现，当邮件中包含两个或更多的问号，或者是问号和感叹号的组合时，背景会发生变化。

此外，当重复使用表情符号时，背景也会发生变化。

深入研究 Android 12 Beta 2 的 SystemUI，我们了解到 PeopleTileViewHelper 类使用正则表达式来检查消息中的某些模式。如果有两个或更多感叹号，两个或更多问号，问号和感叹号的混合，或者两个或更多相同的表情符号，那么该文本/表情符号将应用于小工具的背景。

毫无疑问，这是一个次要的特性，但它确实很吸引你的注意力。代码表明，Conversations 小部件还将显示联系人的生日、周年纪念日、“故事”更新、游戏中的状态、位置等状态消息，但我们还没有看到这种情况的发生。但是，如果您看到了状态消息，请告诉我们！