# Android 12 增加了游戏仪表盘工具和游戏模式 API

> 原文：<https://www.xda-developers.com/android-12-game-dashboard-gaming-mode-apis/>

在一年一度的谷歌游戏开发者峰会上，谷歌为手机游戏玩家和游戏开发者推出了几项新功能。选择运行最新版本 Android 操作系统— [Android 12](https://www.xda-developers.com/android-12/) —的设备将可以访问新的游戏仪表盘实用程序。通过这个仪表板，用户将可以访问关键的实用程序，并可以选择游戏的性能配置文件，游戏可以通过集成 Android 的新游戏模式 API 来支持。我们已经在预发布的 Android 12 版本中瞥见了谷歌在新游戏功能上的工作，但今天谷歌终于宣布了这些功能。

## Android 12 中的游戏仪表盘

自从 Android 12 的第一个开发者预览版以来，我们一直在跟踪悬浮在屏幕上的新[游戏工具栏](https://www.xda-developers.com/android-12-hidden-gaming-mode-toolbar/)的进展。当第二个开发者预览版推出时，[我们发现](https://www.xda-developers.com/android-12-dp2-hidden-features/#android12dp2gamedashboard)这个浮动游戏工具栏是一个新的游戏面板功能的一部分。在第三个开发者预览版中，[谷歌在游戏面板上添加了](https://www.xda-developers.com/android-12-dp3-hidden-features/#android12dp3gamemode)新的游戏优化菜单，虽然它并没有起作用，但很明显谷歌计划让用户根据每个游戏来设置性能配置文件。谷歌游戏开发者峰会的新闻稿没有提供太多信息，甚至没有游戏仪表盘功能的截图，但由于之前的挖掘，我们基本上知道它在 Android 12 上为游戏玩家提供了什么。

通过点击屏幕上出现的浮动游戏工具栏，可以访问游戏仪表盘。只有当用户通过将应用程序的[类别](https://developer.android.com/reference/android/content/pm/ApplicationInfo#category)设置为清单中的[类别 _ 游戏](https://developer.android.com/reference/android/content/pm/ApplicationInfo#CATEGORY_GAME)来启动一个声明自己是游戏的应用程序时，才会出现这个游戏工具栏，这是 Android 8.0 Oreo 中添加的一个功能[。](https://www.xda-developers.com/app-categories-android-oreo/?)

Android 12 的游戏仪表盘提供了有用的工具，如屏幕记录器、屏幕截图快捷方式、FPS 监视器和勿扰开关。这些工具也可以通过悬浮在屏幕上的按钮来访问——前面提到的游戏工具栏——只有当用户通过滑动显示状态或导航栏来退出全屏模式时，它才会显示在底部附近。这个浮动工具栏让游戏玩家可以录制屏幕，捕捉屏幕截图，查看当前帧速率，或者通过打开游戏仪表板(全屏覆盖)来切换勿扰模式，而不会中断游戏。

请勿打扰开关不会全局切换 DND，而是切换*时间表*，当游戏在前台时，该时间表会打开请勿打扰模式。这意味着，只有当你在游戏中时，免打扰模式才会开启，否则它会关闭，除非你有另一个免打扰触发器或时间表来强制它重新开启。您可以在设置>通知>请勿打扰>时间表中手动切换游戏模式免打扰时间表。

游戏仪表盘还提供了三个额外的选项:一个带有性能配置文件的游戏优化菜单，一个在 YouTube 上直播游戏的快捷方式，以及一个集成了来自 [Google Play Games](https://play.google.com/store/apps/details?id=com.google.android.play.games) 的数据的小部件。用户可以从三种性能配置文件中进行选择:性能、标准和节电。性能最大化帧速率，但使用更多的电池，标准使用游戏的默认设置，电池节省降低帧速率，以节省电池寿命。性能配置文件也可以从游戏的应用程序信息页面进行更改，并且该配置文件是粘性的，这意味着一旦用户设置了它，它就不会更改。

当用户启动游戏时，底部会显示一条提示消息，告知他们是否已自动打开了“请勿打扰”模式，以及是否应用了“性能”或“电池节电”模式。

谷歌表示，这项游戏仪表盘功能将在今年晚些时候在运行 Android 12 的“精选设备”上提供。仪表板在测试版中不可用。我们预计谷歌的 [Pixel 6](https://www.xda-developers.com/google-pixel-6/) 系列将推出对该功能的支持，但该功能很可能也会在其他运行 Android 12 的 Pixel 手机上提供。

## Android 游戏模式 API

在其新闻稿中，谷歌表示，Android 新的[游戏模式 API](https://developer.android.com/games/gamemode/gamemode-api)将让开发者“对玩家为他们的游戏选择的性能配置文件做出反应——比如长途通勤的更好电池续航时间，或者获得峰值帧速率的性能模式。”Android 的新[游戏管理器](https://developer.android.com/reference/android/app/GameManager#getGameMode()) API 允许系统应用程序修改任何给定包的游戏模式，由四个游戏模式常量定义:GAME_MODE_BATTERY、GAME_MODE_PERFORMANCE、GAME_MODE_STANDARD 和 GAME _ MODE _ UNSUPPORTED。该 API 还允许开发者查询用户选择的游戏模式，但仅限于他们自己的游戏；建议开发人员在每次恢复应用程序时调用此 API。

游戏开发者必须通过在他们的应用清单中包含元数据来支持性能或省电模式。选择支持电池节电模式允许系统启用[window manager back buffer resizing](https://developer.android.com/games/gamemode/gamemode-interventions#windowmanager_backbuffer_resizing)，如果游戏以目标帧速率进行，这可以显著降低 GPU 负载甚至电池消耗。值得注意的是，原始设备制造商可以选择在有或没有开发者反馈的情况下实施游戏模式干预，因此建议您要么[向原始设备制造商提交您请求的干预](https://developer.android.com/games/gamemode/gamemode-interventions#submit_interventions_to_oems)，要么[完全退出干预](https://developer.android.com/games/gamemode/gamemode-interventions#opt-out_from_interventions)。谷歌的表格[已经开放](https://docs.google.com/forms/d/e/1FAIpQLSdCFlU6eRD5Gp8MKhCqKrg4xe9RVR_EibBTHOpktpXROsWxlw/viewform)供提交。

开发者可以通过“`cmd game`”shell 命令和[设备配置接口](https://developer.android.com/games/gamemode/gamemode-interventions#test_your_game)来测试 Android 新游戏模式 API 的行为。关于 Android 12 中游戏模式 API 的更多信息，请查看 Android 开发者网站上的文档或观看谷歌游戏开发者峰会的完整主题演讲。

\ r \ nht TPS://www . YouTube . com/watch？v=PLMl2ectm7M\r\n