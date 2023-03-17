# Google Fit 准备增加一项新的步行活动

> 原文：<https://www.xda-developers.com/google-fit-prepares-new-paced-walking-activity/>

在过去的几个月里，Google Fit 应用程序获得了多项改进。去年年底，谷歌[为该应用推出了一个改进的主屏幕](https://www.xda-developers.com/google-fit-android-revamped-home-screen-new-wear-os-features/)和一些[新的 Wear OS 功能](https://www.xda-developers.com/new-google-fit-design-features-coming-wear-os/)。该公司随后在今年 2 月为 Google Fit on Wear OS 引入了另一项新功能，即[自动检测锻炼何时结束](https://www.xda-developers.com/google-fit-wear-os-automatically-detect-workout-finished/)。此后不久，谷歌 Fit 应用程序获得了使用 Pixel 手机内置传感器监测心率和呼吸频率的能力。现在，我们已经发现该应用程序有两个更有用的功能。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Google Fit v2.57.16 最近开始通过 Play Store 推出。最新更新的拆卸揭示了暗示以下特征的新字符串:

### 踱步

下面提到的新字符串显示，Google Fit 应用程序将很快获得新的步伐行走功能。这个功能可以让你设置*“散步的速度”*，然后它会播放节拍器声音效果来帮助你保持速度。对即将推出的功能的描述是:*“跟着节拍走，把走路变成一种简单有效的锻炼方式。”*我们在《拆卸》中发现了与此功能相关的四种音效，它们有不同的节奏，可以帮助用户选择最适合他们需求的节奏。

```
 <string name="paced_walking_card_action_button">Try paced walking</string>
<string name="paced_walking_card_content">Follow along with the beat to turn walking into a simple, effective way to exercise.</string>
<string name="paced_walking_card_title">Set a pace for your walks</string>
<string name="paced_walking_edu_cancel_button_text">Cancel</string>
<string name="paced_walking_edu_finish_button_text">Done</string>
<string name="paced_walking_edu_next_button_text">Next</string>
<string name="paced_walking_edu_previous_button_text">Previous</string>
<string name="paced_walking_edu_screen1_body">Brisk walking is an easy way to fit exercise into your day, and counts towards your activity goals.</string>
<string name="paced_walking_edu_screen1_title">Get more from your daily walks</string>
<string name="paced_walking_edu_screen2_body">A brisk walk should leave you a little out of breath. For most people, this is around 100 steps per minute.</string>
<string name="paced_walking_edu_screen2_title">Set the pace you want to walk at</string>
<string name="paced_walking_edu_screen3_body">Step along with the beat to keep up the pace. You can still play podcasts, playlists, or other audio as you go.</string>
<string name="paced_walking_edu_screen3_title">Your chosen pace plays in the background</string> 
```

strings 进一步补充说，该应用程序将在主屏幕上显示一张新的卡片，要求你在未来发布时尝试新的步伐行走功能。您还可以选择步伐行走作为应用程序中的一项活动。还值得一提的是，在活动启用时，您仍然可以播放您最喜爱的音乐、播客或其他音频，声音效果将与其他音频一起播放。

### 血糖跟踪

根据最新更新中发现的新字符串，Google Fit 可能会在未来的版本中支持血糖跟踪。由于 Fitbit 应用程序[最近增加了](https://blog.fitbit.com/fitbit-blood-glucose-tracking-feature/)手动血糖跟踪，即将推出的功能可能旨在帮助你从 Fitbit 应用程序输入数据。或者，它可能是 Google Fit 自己的手动血糖跟踪功能。

```
 <string name="blood_glucose_label">Blood glucose</string>
<string name="blood_glucose_long_format">{value, plural, =1 {1 millimole per litre} other {# millimoles per liter}}</string>
<string name="blood_glucose_long_unit">millimoles per liter</string>
<string name="blood_glucose_range_long_format">Between {firstValue} and {lastValue} millimoles per liter</string>
<string name="blood_glucose_range_short_format">{firstValue} – {lastValue} mmol/L</string>
<string name="blood_glucose_short_format">{value, plural, =1 {1 mmol/L} other {# mmol/L}}</string>
<string name="blood_glucose_short_unit">mmol/L</string> 
```

值得一提的是，Fit API [支持血糖数据类型](https://developers.google.com/fit/scenarios/write-blood-glucose-data)，以帮助应用程序将用户的血糖水平存储为其谷歌帐户的一部分。但现在看来，谷歌 Fit 应用程序本身将允许用户手动设置这些数据。

目前，上面提到的新功能还没有出现在最新的 Google Fit 版本中。一旦谷歌推出未来的更新，我们会尽快通知你。