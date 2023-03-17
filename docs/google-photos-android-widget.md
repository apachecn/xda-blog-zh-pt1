# Android 版 Google 相册为你的回忆准备了一个主屏幕小工具

> 原文：<https://www.xda-developers.com/google-photos-android-widget/>

# Android 版 Google 相册准备为你的回忆添加一个主屏幕小工具

Android 版 Google Photos 应用程序可能很快会让你在主屏幕上添加一个小工具，循环播放你最喜欢的记忆。

早在 10 月，谷歌[发布了](https://blog.google/products/google-on-ios/google-features-new-iphone/)iOS 版[谷歌照片](https://www.xda-developers.com/tag/google-photos/)应用的更新，增加了一个主屏幕小工具。此 widget 会循环浏览“照片”自动生成的“回忆”相簿。在安卓系统上，回忆可以在“照片”标签的顶部看到，但谷歌正准备让用户通过一个小工具在安卓主屏幕上看到它们——就像在 iOS 上一样。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

谷歌照片应用程序的 5.49 版本在 Android 上推出，快速浏览 APK 可以发现一个小工具正在准备中。新字符串引用了一个“谷歌照片”小工具，让你“从谷歌照片中重新发现瞬间”

```
 <string name="photos_widget_account_not_found">Account not found</string>
<string name="photos_widget_description">Rediscover moments from Google Photos</string>
<string name="photos_widget_label">Your memories</string>
<string name="photos_widget_loading">Loading…</string>
<string name="photos_widget_no_logged_in_account">Please add your Google Account before setting up the Google Photos widget</string>
<string name="photos_widget_one_year_ago_title">1 year ago</string>
<string name="photos_widget_select_an_account">Select an account</string>
<string name="photos_widget_this_week_subtitle">This week</string> 
```

虽然字符串和 widget 预览图像表明 Memories 相册将只显示去年本周的照片，但 widget 可能会像在 iOS 上一样工作。也就是说，您将能够添加一个小部件，在所有自动生成的记忆相册中循环。

虽然必备的接收者和活动都列在应用程序的清单中，但我无法将这个小部件添加到主屏幕上，因为它似乎被动态禁用了。也许谷歌将通过未来的更新或切换服务器端标志来启用该功能。一旦该小工具在 Android 版 Google 相册应用中可用，我们会通知您。你可以从 Google Play 下载最新版本的应用[，尽管 5.49 版本可能还没有向所有人推出。](https://play.google.com/store/apps/details?id=com.google.android.apps.photos)