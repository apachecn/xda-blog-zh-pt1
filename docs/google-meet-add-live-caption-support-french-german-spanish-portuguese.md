# Google Meet 准备为法语、德语、西班牙语和葡萄牙语添加实时字幕支持

> 原文：<https://www.xda-developers.com/google-meet-add-live-caption-support-french-german-spanish-portuguese/>

谷歌在 Android 10 中引入了一个名为 Live Captions 的新辅助功能。该功能本质上是通过一次点击转录设备上播放的任何媒体中的语音，使听力受损者更容易观看视频、播客、阅读音频信息等。随着今年早些时候谷歌 Pixel 4a 的推出，谷歌在电话通话中引入了[实时字幕支持](https://www.xda-developers.com/live-caption-transcribe-phone-calls-google-pixel-4a/)，这一新功能现在也可以在[的旧 Pixel 设备](https://www.xda-developers.com/google-rolling-out-live-caption-phone-calls-more-pixel-phones/)上使用。除了媒体和电话，直播字幕也可以在 Google Meet 等应用上使用。然而，该应用程序目前只支持英语视频字幕。但 APK 对 Google Meet 的拆除显示，该应用可能很快支持更多语言的直播字幕。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Google Meet 最新版本的拆卸揭示了新的代码字符串，这表明该公司正在努力为该应用程序添加法语、德语、西班牙语和葡萄牙语的实时字幕支持。

```
 <string name="conference_captions_ftu_dialog_got_it">Got it</string>
<string name="conference_captions_ftu_dialog_settings">Settings</string>
<string name="conference_captions_ftu_message">Your captions language is set to &lt;b>{current_captions_language}&lt;/b>. You can change this in &lt;b>Settings&lt;/b>.</string>
<string name="conference_captions_ftu_title">Captions are now in more languages</string>
<string name="conference_captions_language_picker_dialog_cancel">Cancel</string>
<string name="conference_captions_language_picker_dialog_save">Save</string>
<string name="conference_captions_language_picker_message">Select the language people will use in your meetings. Captions will be shown in that language for all your meetings on this device.</string>
<string name="conference_captions_language_english">English</string>
<string name="conference_captions_language_french">French</string>
<string name="conference_captions_language_german">German</string>
<string name="conference_captions_language_mexico_spanish">Spanish (Mexico)</string>
<string name="conference_captions_language_portuguese">Portuguese</string>
<string name="conference_captions_language_spain_spanish">Spanish (Spain)</string> 
```

正如你在上面的字符串中看到的，Google Meet 将很快在应用程序设置中为用户提供一个新选项，帮助他们选择不同的语言进行实时字幕。一旦该功能推出，该应用程序将通过一条消息提醒用户这一新功能:“字幕现在有更多语言。”然后，用户可以进入应用程序设置，选择不同的字幕语言。对此新设置的描述如下:“选择人们在会议中使用的语言。您在此设备上的所有会议都将以该语言显示字幕。

该代码进一步透露，新的实时字幕语言设置将包括对四种语言的支持，包括法语、德语、西班牙语(墨西哥/西班牙)和葡萄牙语。截至目前，在最新版本的 Google Meet 中，额外的语言支持尚未对用户开放。我们会在这篇文章发布后尽快更新。这篇文章发表几个小时后，谷歌宣布了对 Meet 直播字幕的这些改动。你可以在这里阅读这个公告[。](https://www.xda-developers.com/google-meet-adds-live-captions-on-the-web-in-four-new-languages/)