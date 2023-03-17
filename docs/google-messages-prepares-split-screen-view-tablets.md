# 谷歌信息准备为平板电脑添加分屏视图

> 原文：<https://www.xda-developers.com/google-messages-prepares-split-screen-view-tablets/>

Google Messages 正在慢慢获得用户的青睐，这在一定程度上要归功于过去几个月应用程序中的所有新功能。仅在今年，这款应用就收到了不少更新，比如[日历事件建议](https://www.xda-developers.com/google-messages-suggest-add-calendar-event/)、[预定消息](https://www.xda-developers.com/android-password-checkup-scheduled-messages/)、[自动 OTP 删除](https://www.xda-developers.com/google-messages-auto-otp-delete/)，以及三星手机上的[改进用户界面](https://www.xda-developers.com/google-messages-galaxy-s21-one-ui-design/)。为了保持这一势头，谷歌正在为这款应用开发更多新功能。我们在最新的谷歌信息更新中发现了一些即将推出的功能，下面是它们的样子:

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

### 平板电脑的分屏视图

Google Messages 8.0.054 刚刚开始在 Google Play 上推出，我们发现了指向平板电脑新分屏 UI 的新字符串。字符串显示，该应用程序将很快获得一个名为“列表详细视图”的新设置。一旦启用，此设置将在对话旁边显示您的对话列表。我们设法激活了这个特性来展示它在发布时的样子。

正如你在所附的截图中看到的，列表细节视图将屏幕分成两半，左边是你所有对话的列表，右边是你当前的对话。这种新的 UI 针对大屏幕设备进行了优化，允许应用程序更好地利用额外的屏幕空间。

```
 <string name="split_view_pref_key">split_view_pref_key</string>
<string name="split_view_pref_summary">Show conversation list next to the conversation</string>
<string name="split_view_pref_title">List detail view</string> 
```

### 从配对的手机发送短信

除了分屏视图，最新的谷歌信息更新现在还包括新的字符串指向一个功能，可以让你使用配对的手机发送信息。这项功能可能与即将推出的以平板电脑为中心的布局有关，它可能会让你选择从平板电脑(如果它支持移动数据)发送文本还是从配对的手机发送文本。

对于不知道的人来说，三星手机和平板电脑上的谷歌消息已经提供了类似的功能。这项名为“通话和信息连续性”的功能可以让 Galaxy 设备用户使用同一个电话号码同时在智能手机和平板电脑上收发短信。看起来谷歌现在正在努力扩展这一功能，以支持更多原始设备制造商的设备。

### 与从配对手机发送文本相关的新字符串

```
 <string name="switcher_json">switcher_animation.json</string>
<string name="switcher_pair_device_title_text">Text with paired phone</string>
<string name="switcher_positive_button_text">Continue</string>
<string name="switcher_title_text">Choose how to send &amp; receive messages</string>
<string name="switcher_use_device_sim_number">(%s)</string>
<string name="switcher_use_device_sim_title_text">Text with this device’s SIM</string> 
```

### 更改主要类别

去年 10 月，Google Messages [获得了一个新功能](https://www.xda-developers.com/google-messages-app-test-categorize-conversations/)，可以根据内容自动对对话进行分类。它的工作方式有点像微软的[短信管理应用](https://play.google.com/store/apps/details?id=com.microsoft.android.smsorganizer)，将文本分类成几个类别，包括所有、个人、交易、动态口令、报价等等。然而，不像短信组织者，它没有给用户选择默认类别的能力。

以下字符串表明，谷歌现在终于带来了一个设置，让用户改变主要类别。此设置将允许您从上述选项中选择一个默认类别，每次 Google Messages 都会打开所选的类别。

```
 <string name="primary_view_banner_all_title_text">Your primary view is All</string>
<string name="primary_view_banner_body_text">Manage or change this in Settings</string>
<string name="primary_view_banner_negative_button_text">Settings</string>
<string name="primary_view_banner_personal_title_text">Your primary view is Personal</string>
<string name="primary_view_banner_positive_button_text">Got it</string> 
```

上面提到的功能目前正在开发中，它们并没有出现在最新版本的谷歌消息中。目前，我们不知道这些功能何时会在稳定的频道上推出。但是我们会尽快更新这个帖子。