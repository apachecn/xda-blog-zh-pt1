# “Live Space”可能是谷歌“一览”小工具的一次重大升级

> 原文：<https://www.xda-developers.com/live-space-widget-replace-at-a-glance/>

谷歌的“一览”小工具可以显示当前的日期/时间和天气信息，但它也可以显示即将到来的日历事件、航班、通勤提醒、定期提醒或天气警报。这个小工具[被嵌入到谷歌应用](https://www.xda-developers.com/pixel-at-a-glance-widget-google-app/)中，并持续显示在 Pixel 启动器上，没有关闭它的选项。然而，我们对谷歌应用程序的 12.23.11.23 版本和 Android 12 的最新版本 Pixel Launcher 进行了一些挖掘，发现“一览”小工具有很多变化，从名称改为“Live Space”开始

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

## 生活空间

谷歌应用程序的 12.23.11.23 版本今天早些时候推出，它包含以下新字符串，提到了谷歌助手的新“实时空间”功能。

```
 <string name="ambient_settings_bc_page_desc">Your Assistant shows you what you need, right when you need it, on your home screen and lock screen.</string>
<string name="ambient_settings_bc_title">Live Space</string>
<string name="ambient_settings_personalize_section_bc_desc">Get the most of your Live Space updates by enabling location, setting home and work address, and more.</string>
<string name="assistant_settings_indexing_ambient_assistant_bc_keywords">live space</string>
<string name="bc_feature_section_title">Proactive moments</string> 
```

这些字符串很好地描述了“一目了然”小部件已经可以实现的功能，但是使用了一个新的“实时空间”名称。事实上，在我们激活“实时空间”的设置页面后，我们发现它已经取代了“一览”的设置。唯一真正新的功能是“在商店”开关，当你在受支持的商店时，它会显示“购物清单和 Google Pay 奖励卡”底部的耳机图标没有附带说明，但我们相信它与我们去年发现的“媒体建议”功能有关。

我们深入研究了谷歌应用程序的代码，发现谷歌正致力于显示更多个性化信息，包括与体育、股票和生日相关的信息。这些信息目前都没有显示在一览窗口小部件中，我们在“实时空间”设置页面中也找不到它们的切换。

“实时空间”功能还没有对用户开放，但当它开放时，我们会让你知道。这可能是谷歌对 [Android 12](https://www.xda-developers.com/android-12/) 中的小工具进行更广泛的[改革的一部分。谷歌展示了即将出现在 Pixel 手机上的新部件，作为你重新设计的](https://www.xda-developers.com/google-android-12-widgets-overhaul/)[材料的一部分，但这些部件还没有一个已经在设备上推出。](https://www.xda-developers.com/material-you/)

## 关闭“一目了然”

另外，谷歌还在努力让用户从 Pixel Launcher 设置中关闭“一览”小工具。在大多数设备上，“一览”小工具是一个可选的附加功能，但在 Pixel 手机上，它会持续显示在主屏幕的顶部。一旦新的 Pixel Launcher 设置页面对用户开放，这种情况可能很快就会改变。点击“一目了然”会出现一个对话框，让用户在主屏幕和锁屏中隐藏小工具。

## 较新的谷歌镜头图库

最后，谷歌正在对谷歌镜头服务进行微调。几个月前，Google Lens 增加了一个内置图库，可以更快地选择图像。很快，画廊可能会让你向下滑动退出，而不是按下返回。图库图标在这次测试中也有了细微的变化。

*新*

*老*

如前所述，在最新版本的谷歌应用程序上，这些功能都没有对用户开放。谷歌总是在测试新功能，但它们可能需要几周或几个月的时间才能到来。有时候，这种事永远不会发生。“生活空间”功能几乎肯定会登陆，但我们不知道这是否会是它的最终名称。如果我们发现新的信息，我们会通知你的。

* * *

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*