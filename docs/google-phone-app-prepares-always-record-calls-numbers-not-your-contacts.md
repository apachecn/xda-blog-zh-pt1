# 谷歌手机应用程序准备让你总是记录电话号码不在你的接触

> 原文：<https://www.xda-developers.com/google-phone-app-prepares-always-record-calls-numbers-not-your-contacts/>

大约一年前，谷歌开始致力于为谷歌手机应用程序带来通话记录支持。该功能随后很快推广到该公司的 Pixel 系列，随后是[的几款诺基亚设备](https://www.xda-developers.com/google-phone-app-rolls-out-call-recording-nokia-phone-users-india/)和[的几款小米手机](https://www.xda-developers.com/google-phone-app-call-recording-feature-now-available-multiple-xiaomi-phone-globally/)。现在，谷歌正在努力改进这项功能，以帮助你自动记录未知号码的来电。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

谷歌手机应用程序(第 59 版)最新更新的拆卸揭示了新的代码字符串，突出了即将到来的功能。正如您所看到的，字符串提到了一些新的对话框消息，一旦该功能在未来的更新中推出，这些消息就会提醒用户。

```
 <string name="non_contact_always_record_dialog_message">"You or the other person in your call might be somewhere that requires everyone to consent to being recorded. Everyone will be notified ahead of time that the call is being recorded. It's up to you to follow laws about recording conversations. Recordings are stored only on your phone."</string>
<string name="non_contact_always_record_dialog_title">Always record calls with numbers not in your contacts?</string>
<string name="non_contact_always_record_negative_button_label">Cancel</string>
<string name="non_contact_always_record_positive_button_label">Always record</string>
<string name="non_contact_toggle_key">non_contact_toggle_key</string>
<string name="non_contact_toggle_label">Numbers not in your contacts</string> 
```

关于该功能的第一个字符串提到了一个免责声明，声明如下:

“您或通话中的其他人可能在某个地方，需要所有人都同意被录音。每个人都会被提前通知电话正在被录音。这取决于你是否遵守记录谈话的法律。录音只存储在您的手机上。”

在免责声明之后，用户将看到一个确认对话框，询问他们是否希望为不在联系人列表中的号码打开自动呼叫记录。它将包括两个选项——“总是记录”和“取消”——以启用或禁用该功能。字符串还提到了该功能的切换，一旦该功能推出，它应该会显示在应用程序设置中。

截至目前，谷歌尚未发布任何关于这项新通话记录功能的信息。我们将在未来谷歌手机更新开始时更新这篇文章。值得注意的是，虽然你可以在几乎所有的 Android 设备上安装谷歌手机应用程序，但通话录音功能仅在某些地区的特定手机上可用。

* * *

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*