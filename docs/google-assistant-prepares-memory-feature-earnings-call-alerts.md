# 谷歌助手准备了一个新的“记忆”功能和收益电话提醒

> 原文：<https://www.xda-developers.com/google-assistant-prepares-memory-feature-earnings-call-alerts/>

**更新 1 (03/24/2021 @ 04:32 PM ET):** 我们已经成功启用了该功能，为您带来了一些谷歌助手中记忆功能的截图。[点击这里了解更多信息。](#update1)这篇发表于 2021 年 3 月 24 日的文章被保存在下面。

谷歌一直在努力扩展谷歌助手的功能，并定期为虚拟助手试验新的功能和技能。去年 10 月，我们[发现了与一个叫做“辅助记忆”的功能相关的字符串](https://www.xda-developers.com/google-app-preps-assistant-memory-and-at-a-glance-media-recommendations/)当时，还不清楚这项功能的用途。但在谷歌应用的最新更新中，我们发现了许多关于这一功能的新字符串、资源和布局。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

其中一个字符串将助理内存描述为“一种保存和查找您的内容的简单方法。”本质上，它会让你要求谷歌助手记住或保存对你来说重要的东西，并且它会为它创建一个记忆。但新功能的范围将比助手目前提供的笔记和提醒功能广泛得多。

用户将能够保存笔记、提醒、照片、截图、链接等，并将它们整齐地组织在不同的标签下。保存的内容将被添加到一个内存列表中，该列表将在一个地方显示所有内容，以便于访问。

```
 <string name="stash_enter_record_payload_message">What do you want to remember?</string>
<string name="stash_open_memory_chip_text">Open Memory</string>
<string name="stash_record_creation_successful">"I'll remember that!"</string>
<string name="stash_save_chip_text">Save</string>
<string name="stash_toast_error_message">Sorry, something went wrong.</string> 
```

保存提醒时，您还可以附加一张截图或照片，以获得更多信息。

```
 <string name="assistant_memory_record_editor_payload_hint">Add note</string>
<string name="assistant_memory_reminder_open_button_onboarding_title">Reminders now get saved to Assistant Memory</string>
<string name="assistant_memory_reminder_remove_context_onboarding_subtitle">"If you want to remove the attached screen content, tap the little 'X' button"</string>
<string name="assistant_memory_reminder_remove_context_onboarding_title">Reminders now get saved with screen content to Assistant Memory</string>
<string name="assistant_memory_screen_capture_disabled_text">Screen capture not enabled</string>
<string name="assistant_memory_screen_capture_open_settings_text">Open Settings</string>
<string name="assistant_memory_take_photo_button_description">Take photo</string> 
```

这个功能可以让你在记忆达到目的后清空它们，并且还可以让你从清空文件夹中恢复它们。

```
 <string name="assistant_stash_empty_trash_confirmation_dialog_message">"All items will be permanently deleted. This can't be undone."</string>
<string name="assistant_stash_empty_trash_confirmation_dialog_negative_button_title">Cancel</string>
<string name="assistant_stash_empty_trash_confirmation_dialog_positive_button_title">Empty Trash</string>
<string name="assistant_stash_empty_trash_confirmation_dialog_title">Empty Trash?</string>
<string name="assistant_stash_empty_trash_failure_snackbar_text">Failed to empty trash. Please try again.</string>
<string name="assistant_stash_empty_trash_progress_dialog_message">Emptying Trashâ€¦</string>
<string name="assistant_stash_empty_trash_subtitle">Any Memories you delete will appear here</string> 
```

当保存一些东西时，比如你正在游览的一个新地方的照片，你可以选择将你的位置和它一起保存，这样你就可以很容易地在谷歌地图上再次找到它。

```
 <string name="assistant_stash_location_card_subtitle_text">Give Assistant permission to store your location when you save things, to make it easy to find them again. You can disable this at any time</string>
<string name="assistant_stash_location_card_title_text">Allow Location</string>
<string name="assistant_stash_location_permission_allowed_failure">Failed to enable location</string>
<string name="assistant_stash_location_permission_allowed_success">Location enabled</string>
<string name="assistant_stash_maps_action_title">Open Maps</string> 
```

为了更快地访问，用户还可以选择在主屏幕上添加一个助手记忆快捷方式。

```
 <string name="assistant_stash_shortcut_banner_start_button_text">Add to Home screen</string>
<string name="assistant_stash_shortcut_banner_subtitle">Add a shortcut for faster access</string>
<string name="assistant_stash_shortcut_banner_title">Make Memory just a tap away</string>
<string name="assistant_stash_shortcut_card_image_content_description">Shortcut image</string>
<string name="assistant_stash_shortcut_card_primary_button_label">Add to Home screen</string>
<string name="assistant_stash_shortcut_card_secondary_button_label">No Thanks</string>
<string name="assistant_stash_shortcut_card_subtitle_text">Add a shortcut for faster access</string>
<string name="assistant_stash_shortcut_card_title_text">Make your Memory just a tap away</string> 
```

助理内存被标记为“狗粮功能”，这意味着它目前正在内部测试，需要一个白名单中的谷歌帐户才能访问。

除了 Assistant Memory，我们还发现了另一个新功能的字符串，它将通知用户有关收入的电话。这些字符串表明，每当你在股市上跟踪其股票的公司召开季度收益电话会议时，谷歌应用程序都会提醒你。

```
 <string name="earnings_call_during_event_title_with_dynamic_time">%1$s now</string>
<string name="earnings_call_pre_event_title_with_dynamic_time">%1$s in %2$s</string>
<string name="earnings_call_title_with_static_time">%1$s at %2$s</string> 
```

助理记忆和耳听呼叫提醒仍在开发中，最终用户无法使用。我们将密切关注任何进一步的发展，当它们上线时，我们会让您知道。

* * *

## 更新 1:谷歌助手中“记忆”的截图

经过一点点修改，我们设法在谷歌应用中启用了新的记忆功能。以下是入职流程的截图:

这里是主界面的截图:

Android 应用程序开发人员和逆向工程师 Alessandro Paluzzi 也成功启用了新功能，在谷歌应用程序中分享了更多该功能的截图。这项功能仍被标记为“狗粮”功能，谷歌助手的普通用户还无法使用。一旦推出，我们会让你知道。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*