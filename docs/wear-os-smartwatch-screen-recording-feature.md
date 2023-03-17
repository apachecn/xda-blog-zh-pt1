# Wear OS 2.45 准备添加屏幕录制功能

> 原文：<https://www.xda-developers.com/wear-os-smartwatch-screen-recording-feature/>

# 您的 Wear OS 智能手表可能会接收屏幕录制功能

在 Wear OS companion 应用 2.45 版本中，我们发现了一些新的字符串，表明谷歌正在准备添加屏幕录制功能。

你的[戴上操作系统驱动的智能手表](https://www.xda-developers.com/wear-installer-sideload-wear-os-apps/)可能很快就会支持屏幕录制功能。在最新版本的 Wear OS companion 应用程序中，我们发现了一些新的字符串，表明谷歌正准备为其智能手表 OS 添加屏幕录制功能。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

以下是我们在 [Wear OS](https://play.google.com/store/apps/details?id=com.google.android.wearable.app) 版本 2.45(安装在手机上的配套应用)中发现的新字符串:

```
 <string name="screen_recording_email_subject">Wear OS Screen Recording</string>
<string name="screen_recording_wearable_notification_text">Tap to send.</string>
<string name="screen_recording_wearable_notification_title">Ready to send watch screen recording.</string> 
```

看字符串，似乎用户将能够使用 Android Sharesheet 菜单发送或共享屏幕记录。进一步检查应用程序的代码，我们了解到该文件将被保存为“screen-recording.mp4”。Wear OS 长期以来一直支持使用配套应用程序对手表 UI 进行截图，这项新功能很可能也会以类似的方式实现。

除了 UI 演示和特定于开发人员的用例，我想不出屏幕录制功能对普通用户有多大用处。尽管如此，看看谷歌计划如何在智能手表上利用它还是很有趣的。

应该注意的是，屏幕录制功能尚未对 Wear OS 用户开放。我们也不知道谷歌计划如何以及何时向大众推出这一功能。我们将密切关注该功能的进一步发展，如果我们了解到任何新情况，一定会让您知道。