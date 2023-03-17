# Android 12 Beta 2 暗示了新的谷歌“实时翻译”功能

> 原文：<https://www.xda-developers.com/android-12-beta-2-google-live-translate-feature/>

第二个 [Android 12](https://www.xda-developers.com/android-12/) 测试版今天早些时候登陆，我们一直在挖掘固件以寻找新功能。在最新的版本中可以发现大量的变化，并且由于缺少组件，一些变化还没有生效。Pixel 手机未来的 Android 12 版本可能会有一个功能，叫做“实时翻译”。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

用于 Pixel 5(可能还有其他 Pixel 设备)的 Android 12 Beta 2 包含新版本的 SettingsIntelligence 应用程序。SettingsIntelligence 是一个系统应用程序，它为主设置应用程序提供了附加功能和搜索词。SettingsIntelligence 的最新版本 1.1.0.372474662 包含以下新字符串:

```
 <string name="auto_translate_switch_title">Use Live Translate</string>
<string name="auto_translate_title">Live Translate</string> 
```

检查应用程序的代码，我们了解到这个“实时翻译”功能实际上将作为另一个应用程序“设备个性化服务”的一部分提供。如果用户的搜索查询包含这些术语中的一个:“自动”、“自动翻译”、“自动翻译”或“翻译”，则 SettingsIntelligence 将显示一个切换，以从设置中启用实时翻译。然而，如果以下组件不存在，切换将不会显示:`com.google.android.as/com.google.android.apps.miphone.aiai.translate.settings.settingsui.AutoTranslateSettingPortalActivity`，如果设备运行的是比 Android 12 更旧的版本，它也不会显示。最新版本的设备个性化服务没有上述组件(`com.google.android.as`是 DPS 的包名)，也没有直接提及“实时翻译”功能。

至于这个“实时翻译”功能到底会做什么，我们有几个猜测。根据名称，该功能可能会实时转录并翻译设备上检测到的语音。基本上，这是对现场字幕的扩展，目前现场字幕只能将语音转录成同一种语言的文本。谷歌翻译应用已经具备了实时翻译的能力，所以我认为谷歌会增加系统范围的实时翻译功能。

谷歌还在为 Pixel 手机开发另一项与翻译相关的功能:[应用程序的 UI 翻译](https://www.xda-developers.com/android-12-app-ui-translation/)。Live Translate 可能只是这一 UI 翻译功能的营销名称，因为[我们之前对该功能的调查](https://www.xda-developers.com/google-pixel-ui-translation-android-12/)揭示了设备个性化服务应用中另一项与翻译相关的未发布活动。在我们得到 DPS 的更新版本之前，我们无法确定，但我们将继续挖掘 Android 12 Beta 2，看看我们能找到什么。如果你对我们发现的其他东西感兴趣，你可以阅读下面链接的 Twitter 帖子，或者等待我们的摘要在 XDA 上线。

* * *

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*