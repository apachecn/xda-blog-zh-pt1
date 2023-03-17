# Google Home 应用为 Nest Hello 准备了安静时间和快速响应

> 原文：<https://www.xda-developers.com/nest-hello-doorbell-more-controls-google-home-app/>

Google Home 应用是您控制所有支持 Google Assistant 的设备的一站式商店，包括 Google 自己的 Nest 品牌产品。谷歌仍在将功能从 Nest 应用程序迁移到 Home 应用程序，这一过程[始于一年多前](https://www.xda-developers.com/google-launches-nest-aware-subscription-service/)，今天推出的最新版本的谷歌 Home 应用程序显示，更多的 Nest Hello 控件将进入 Home 应用程序。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Google Home 2.40.1.10 今天早些时候在 Google Play 上推出，快速浏览一下 APK 的资源就会发现新的字符串。这些字符串表明，Nest 应用程序的“安静时间”和“快速响应”功能将被添加到 Home 应用程序中。具体来说，它们将出现在 Home 应用程序中 Nest Hello 的实时视频底部的一个标签中。

```
 <string name="camera_mode_more_action_emergency_title">Emergency</string>
<string name="camera_mode_more_action_quiet_time_title">Quiet Time</string>
<string name="camera_mode_more_action_responses_title">Quick Responses</string>
<string name="camera_mode_more_connecting_status">Connecting</string>
<string name="camera_mode_more_option">More</string>
<string name="camera_mode_more_option_camera_title">CAMERA</string>
<string name="camera_mode_more_option_off_status">Off</string>
<string name="camera_mode_more_option_on_status">On</string>
<string name="camera_mode_option_a11y">%1$s, tab, %2$d of %3$d.</string>
<string name="camera_mode_option_explore">History</string>
<string name="camera_mode_option_live">Live</string>
<string name="camera_mode_toggle_cell_a11y">%1$s is %2$s. Adjustable.</string> 
```

对于那些不熟悉的，安静的时间让你静音室内钟声和访客公告 30 分钟，60 分钟，90 分钟，2 小时，或 3 小时。通过点击 Nest Hello 门铃的视频源，然后点击右下角带有钟声图标的“安静时间”按钮，可以从 Nest 应用程序中访问它。

```
 <string name="quiet_time_bottom_sheet_button_set">Set</string>
<string name="quiet_time_bottom_sheet_countdown_body">Quiet time</string>
<string name="quiet_time_bottom_sheet_options_body">Choose how long you want to mute your indoor chime and visitor announcements</string> 
```

快速响应让您在访客按您的门铃时快速播放预先录制的语音消息。你可以让 Nest Hello 门铃说“你可以留下它”、“我们马上就到”或“没人能来开门”，方法是当有人按门铃时，在你的手机上出现的通知中点击所需的响应。你不能在 Nest 应用或 Home 应用中定制快速响应，然而，似乎你至少可以通过 Google Home 应用发送它们，而不仅仅是通过 Nest 应用发送给你的通知。

我们已经成功启用了新的“更多”标签，并在 Google Home 应用程序中显示了安静时间和快速响应设置，如下面嵌入的截图所示。这些功能在 Google Home 应用程序的 2.40.1.10 版本中不对用户开放，但它们很可能会作为服务器端更新的一部分很快推出。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*