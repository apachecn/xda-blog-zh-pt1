# 谷歌助手准备添加快速短语和动态快捷方式

> 原文：<https://www.xda-developers.com/google-assistant-quick-phrases-dynamic-shortcuts/>

谷歌今天推出了 12.22.5 版本的谷歌应用程序，它确认了两个新功能的开发，我们预计很快将在谷歌助手中登陆。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

## 快速短语

回到 4 月份，在谷歌助手的设置中，一个神秘的“语音快捷方式”页面出现在许多用户面前。该页面将用户链接到代号为“鳄梨色拉酱”的谷歌内部文档在最新的谷歌应用更新中，我们现在知道“鳄梨色拉酱”功能将被称为“快速短语”

```
 <string name="assistant_android_settings_quick_phrases_summary">Skip saying “Hey Google” for help with specific tasks</string>
<string name="assistant_android_settings_quick_phrases_title">Quick phrases</string> 
```

至于你将能够用新的“快速短语”功能做什么，你将能够跳过说“嘿谷歌”的热门词汇，用于常见的语音交互，包括响铃警报、来电或正在进行的计时器。例如，如果你启用了这个功能，你大概就不用大喊“嘿，谷歌”来解除你的闹钟了。

```
 <string name="assistant_guacamole_pill_popup_description_alarm">Skip “Hey Google” when using quick phrases like “%1$s” or “%2$s” for a ringing alarm.</string>
<string name="assistant_guacamole_pill_popup_description_call">Skip “Hey Google” when using quick phrases like “%1$s” or “%2$s” for incoming calls.</string>
<string name="assistant_guacamole_pill_popup_description_timer">Skip “Hey Google” when using quick phrases like “%1$s” for a firing timer.</string>
<string name="assistant_guacamole_pill_popup_link_text">You can update this choice in <u>Assistant Settings</u>.</string>
<string name="assistant_guacamole_pill_prompt">Say</string&gt
<string name="assistant_guacamole_ui_prompt">Try saying</string> 
```

## 动态快捷方式

在谷歌 I/O 2021 上，谷歌展示了谷歌助手的几个[新功能。很快，助手就会根据你的 app 使用模式，主动向用户推荐快捷方式。最新的谷歌应用程序更新为这一功能提供了支持，字符串表示动态快捷方式“与你正在键入的内容相关，可以基于与你设备上的应用程序的交互。”Android Nougat 引入了动态快捷方式，作为开发人员在应用程序中提供特定的上下文相关操作的一种方式。谷歌正计划让 Android 应用程序快捷方式成为谷歌助手体验的更大一部分，在 UI 中引入动态快捷方式是这一变化的一部分。](https://www.xda-developers.com/google-assistant-one-tap-shortcuts-third-party-apps/)

```
 <string name="googleapp_assistant_dynamic_shortcut_long_press_message">"This suggestion is related to what you're typing and can be based on interactions with apps on your device. You can manage activity shared with Assistant, per app, within Assistant Settings."</string>
<string name="googleapp_assistant_light_suggestion_annotation_separator">" · "</string>
<string name="googleapp_assistant_non_dynamic_shortcut_long_press_message">"This suggestion is related to what you're typing."</string> 
```

* * *

你可以从上面嵌入的谷歌 Play 商店链接下载最新版本的谷歌应用，或者你可以从 [APKMirror](https://www.apkmirror.com/apk/google-inc/google-search/google-search-12-22-5-release/) 下载 APK。我们在运行 Android 11 的 Pixel 4 和运行 Android 12 Beta 1 的 Pixel 3 XL 上安装了更新，但没有看到这些功能。我们将继续挖掘最新的谷歌应用程序版本，看看我们是否能找到更多的功能，或者我们是否能让这些功能工作。