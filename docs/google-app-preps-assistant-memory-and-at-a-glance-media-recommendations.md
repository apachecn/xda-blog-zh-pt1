# 谷歌应用程序准备“助理记忆”，一目了然媒体推荐

> 原文：<https://www.xda-developers.com/google-app-preps-assistant-memory-and-at-a-glance-media-recommendations/>

看起来谷歌正准备为其谷歌应用程序引入新功能，新字符串指向“助理记忆”功能和概览小部件中的媒体推荐。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

新字符串是在谷歌应用程序 11.34.7.29 中发现的。首先是一个“辅助记忆”功能，strings 将其描述为一种保存和查找内容的简单方法。还不清楚它将如何工作，但听起来你可以在图片旁边保存笔记和提醒，以帮助唤起你的记忆。说到内存，这个功能可能与一个“内存辅助锁”功能有关，这个功能[已经在](https://www.androidpolice.com/2018/08/03/google-app-v8-15-beta-hints-memory-aid-locker-conversational-translation-smart-displays-categories-top-apps-apk-teardown/)工作了一段时间。当这个功能的字符串第一次出现在谷歌应用程序中时，我们并不确定它的用途。有可能谷歌搁置了这一功能，现在终于回归，或者他们从零开始开发新功能。

```
 <string name="opa_memory_card_attach_photo_promotion_subtitle">"If you want to delete the screen capture and replace it with a photo, tap the little 'X' button."</string>
<string name="opa_memory_card_attach_photo_promotion_title">Did you know you can attach photos?</string>
<string name="opa_memory_card_first_use_promotion_subtitle">"Add a note or reminder below, or tap the 'Open Memory' button to learn more."</string>
<string name="opa_memory_card_first_use_promotion_title">Assistant Memory is an easy way to save and find your stuff!</string> 
```

无论情况如何，Assistant Memory 都希望加入谷歌提供的许多笔记和提醒功能中的一个，从专用的谷歌 Keep 应用程序到谷歌助手已经允许你创建的提醒/列表。

另一个新特性的字符串与概览小部件中的媒体推荐相关。根据新的字符串，小工具可能会基于上下文显示媒体推荐，比如当你将耳机连接到设备时。因此，假设您经常连接耳机，启动您喜欢的音乐服务，并播放锻炼播放列表。一目了然小工具似乎可以学习这种行为，并在连接耳机后立即推荐启动您最常用的媒体播放器。

```
 <string name="smartspace_media_recommendation_summary">Media suggestions when headphones connected</string>
<string name="smartspace_media_recommendation_title">Media suggestions</string> 
```

尚不清楚这些功能何时/是否会为谷歌应用的用户上线。这可能需要几天，几周，甚至几个月。我们将尝试并激活这些功能来展示它们，但与此同时，我们将密切关注它们的正式推出。