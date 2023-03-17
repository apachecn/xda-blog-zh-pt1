# 谷歌地图 10.53.1 准备增加语言转换器和谷歌助手驾驶模式

> 原文：<https://www.xda-developers.com/google-maps-10-53-1-prepares-language-changer-google-assistant-driving-mode/>

谷歌[在谷歌 I/O 2019 上首次宣布了](https://www.xda-developers.com/google-assistant-driving-mode-waze/)谷歌助手驾驶模式。一年多后，该功能终于在本月早些时候[开始向一些用户](https://www.xda-developers.com/google-assistant-driving-mode-rolling-out/)推出。然而，该模式是在部分完成的状态下推出的，它的一些功能当时并没有按预期工作。现在，谷歌地图最新版本(v 10.53.1)的拆解揭示了新的字符串，这表明谷歌仍在为更广泛的发布完善该功能。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

不知道的是，谷歌助理驾驶模式应该会取代智能手机上的 Android Auto 应用。它带来了[新的导航 UI](https://www.xda-developers.com/google-maps-tests-car-mode-ui-bigger-buttons/) ,带有大而易操作的按钮和改进的语音控制。

在我们之前的报道中，我们分享了一些新用户界面的截图。现在，我们的主编米沙·拉赫曼已经成功地从最新版本的谷歌地图中提取了谷歌助理驾驶模式的屏幕截图。在最新版本的谷歌地图中发现的新字符串也提到了上面截图中看到的选择加入对话框。

```
 <string name="NAVIGATION_ASSISTANT_DRIVING_MODE_OPT_IN_DIALOG_LEARN_MORE">Learn more</string>
<string name="NAVIGATION_ASSISTANT_DRIVING_MODE_OPT_IN_DIALOG_OPT_IN">Try it out</string>
<string name="NAVIGATION_ASSISTANT_DRIVING_MODE_OPT_IN_DIALOG_OPT_OUT">Not now</string>
<string name="NAVIGATION_ASSISTANT_DRIVING_MODE_OPT_IN_DIALOG_TEXT">Improved voice control and easy-to-tap buttons help you focus on the road.</string>
<string name="NAVIGATION_ASSISTANT_DRIVING_MODE_OPT_IN_DIALOG_TITLE">Be the first to use Assistant driving mode in Maps</string> 
```

除了谷歌助手驾驶模式的选择对话框，拆卸还发现了新的字符串，表明谷歌正在努力在 Android 上的谷歌地图中添加语言转换器。虽然你目前可以在 Android 上更改谷歌地图的语音导航语言，但该应用不包括更改应用界面语言的功能。

既然谷歌地图的网页版已经有了这样一个功能[，那么该公司把它带给安卓用户是有意义的。与这个即将到来的特性相关的新字符串表明语言转换器将允许用户改变界面语言。](https://www.republicworld.com/technology-news/apps/how-to-change-the-language-in-google-maps-on-computers-and-smartphones.html)

```
 <string name="APP_LANGUAGE_SETTINGS_CONFIRMATION_PROMPT">Maps will restart to change your app language</string>
<string name="APP_LANGUAGE_SETTINGS_CONFIRMATION_TITLE">%1$s to %2$s</string>
<string name="APP_LANGUAGE_SETTINGS_DOWNLOAD_FAILED_DIALOG_LEARN_MORE_LINK">Learn more</string>
<string name="APP_LANGUAGE_SETTINGS_DOWNLOAD_FAILED_DIALOG_TEXT">Maps will keep trying to change your language. Check again later.</string>
<string name="APP_LANGUAGE_SETTINGS_DOWNLOAD_FAILED_DIALOG_TITLE">"Can't change your language right now"</string>
<string name="APP_LANGUAGE_SETTINGS_PAGE_CATEGORY_ALL">All</string>
<string name="APP_LANGUAGE_SETTINGS_PAGE_CATEGORY_SUGGESTED">Suggested</string>
<string name="APP_LANGUAGE_SETTINGS_PAGE_TITLE">App language</string>
<string name="APP_LANGUAGE_SETTINGS_PROGRESS_SPINNER_TEXT">Changing Language…</string>
<string name="APP_LANGUAGE_SETTINGS_TITLE">App language</string> 
```

这些字符串突出显示了用户必须重新启动应用程序才能应用新的语言设置，如果语言更改不成功，还会弹出几条错误消息。此外，字符串显示语言转换器还会提供语言建议，可能基于全局设置。

值得注意的是，在当前版本的谷歌地图中，谷歌助手驾驶模式的选择对话框和语言转换器都不可用。到目前为止，我们还没有从谷歌得到任何关于发布时间表的信息。一旦这些功能进入稳定频道，我们将会更新这篇文章。

* * *

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*