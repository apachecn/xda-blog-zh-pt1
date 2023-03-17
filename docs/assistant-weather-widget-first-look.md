# 谷歌正在为 Android 开发一款新的助手天气小工具

> 原文：<https://www.xda-developers.com/assistant-weather-widget-first-look/>

**更新 1 (09/21/2021 @美国东部时间下午 2:06):**谷歌应用的更新带来了一个新的助手天气小工具——在谷歌 I/O 上被取笑的那个。[点击这里了解更多信息。](#update1)文章发表于 2021 年 9 月 14 日，下面保留。

在被忽视多年后，小工具终于将在 [Android 12](https://www.xda-developers.com/android-12/) 中得到急需的彻底改革。谷歌在谷歌 I/O 2021 上展示了 Android 12 的重新设计的小工具。在过去的几个月里，我们已经看到许多这些小部件在 Android 12 测试版中上线。上周推出的最后一款 [Android 12 Beta 5](https://www.xda-developers.com/android-12-beta-5-changelog/) 带来了改进后的时钟小工具，以及“油漆芯片”小工具和部分可用的“生活空间”小工具。现在，在 Android 12 公开发布之前，我们已经发现了一个全新的天气助手的证据。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

谷歌应用 12.36.15 测试版刚刚在谷歌 Play 商店推出，它包含了一个新的助理天气小工具的字符串。

```
 <string name="assistant_weather_widget_config_dialog_enable_btn">Get Started</string>

<string name="assistant_weather_widget_config_dialog_exit_btn">No Thanks</string>

<string name="assistant_weather_widget_config_dialog_location_rationale">"Please grant the location permission \"Allow all the time\" for accurate weather info.

App info > App permission > Location permission to \"Allow all the time\""</string>

<string name="assistant_weather_widget_config_dialog_title">Location Permission Required</string>

<string name="assistant_weather_widget_no_location_permission_text">Location Permission Required</string>

<string name="assistant_weather_widget_offline_text">"You're offline. Check your connection."</string>

<string name="assistant_weather_widget_oops_text">Oops, something went wrong</string> 
```

助手天气小部件似乎还没有推出，但我们手动启用了接收器，并让它显示在小部件选择器中。它看起来是这样的:

正如你在上面的截图中看到的，这个设计看起来很有灵感。它还不支持动态颜色，尽管它似乎尊重全系统的黑暗主题。该小部件显示当前天气、您的位置以及最高和最低温度。它与谷歌 I/O 上展示的不太匹配，所以可能还有其他形式的小工具在开发中。

这就是我们目前所知道的关于谷歌应用中即将推出的助手天气窗口的所有信息。如果我们在接下来的几周里了解到任何关于这个小工具的新信息，我们一定会让你知道。

* * *

多亏了谷歌应用的新版本——准确地说是 12.37.19.29 版本——我们现在可以访问在谷歌 I/O 上展示的新的长方形天气小部件。此外，天气小部件现在支持动态颜色。

新的助手天气小工具还没有向用户推出，但我们会让你知道什么时候推出。