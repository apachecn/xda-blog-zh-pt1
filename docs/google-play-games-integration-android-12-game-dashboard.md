# Google Play Games 增加了与 Android 12 游戏仪表盘的集成

> 原文：<https://www.xda-developers.com/google-play-games-integration-android-12-game-dashboard/>

手机游戏是一个价值数十亿美元的行业，然而除了为游戏开发者提供新的 API 和服务，谷歌并没有给 Android 本身增加许多面向用户的游戏功能。直到定于今年秋天晚些时候发布的 Android 12。当 Android 12 推出时，它将带来一个新的游戏仪表盘功能。这个仪表板提供了对屏幕记录器、FPS 监视器等有用工具的快速访问，它还有一个显示 Google Play 游戏成就和排行榜数据的小部件。谷歌在今年早些时候的谷歌游戏开发者峰会上预览了游戏仪表盘及其 Play Games widget [，现在它已经开始推出了。](https://www.xda-developers.com/android-12-game-dashboard-gaming-mode-apis/)

Google Play Games 应用程序的 2021.07.28550 版本现在正在通过 Play Store 推出，在我运行 Android 12 Beta 4 的 Pixel 3 XL 上安装它后，每当我加载一个支持 Play Games 的游戏时，Google Play Games 小工具终于出现在游戏仪表盘中。*海绵宝宝:比基尼之战复水*举例来说，让我看到我完成了多少成就。如果游戏有排行榜，排行榜的数量也会显示在这里。

点击小工具会打开另一个页面，显示您在 Play Games 上的用户名、您的 Google 帐户的电子邮件地址，以及指向成就、排行榜和 Play Games 中的个人资料和隐私设置页面的卡片。成就卡显示了你解锁的最后一项成就，我推测排行榜卡也预览了更多信息(我不在任何排行榜上，所以我不能说。)点击成就或排行榜卡，无需打开 full Play Games 应用程序，即可显示更多关于可用成就和排行榜的信息，让游戏仪表盘成为查看游戏进度/状态的便捷方式。

当谷歌[上个月宣布](https://www.xda-developers.com/android-12-game-dashboard-gaming-mode-apis/)游戏仪表盘功能时，他们表示该功能将在今年晚些时候在运行 Android 12 的“精选设备”上可用。他们还表示，它将不会在测试版中提供，但我们发现，这并不完全正确。在过去的几个版本中，可以通过设置>通知>请勿打扰>日程来访问游戏仪表盘。点击“游戏”时间表旁边的 cog 图标会将您带到“游戏设置”页面，其中包含游戏仪表板的全局切换和“游戏勿扰功能”。这个“游戏设置”页面也可以在发布时通过设置>应用程序访问。在 Beta 4 中，每当人们启动一个适当分类的游戏时，浮动游戏覆盖就开始向他们显示，这使得用户可以从游戏中访问游戏仪表板。

随着 Google Play 游戏集成的加入，游戏仪表盘的功能已经接近完成。现在缺少的只是游戏优化设置，但这依赖于支持 Android 12 中新的[游戏模式 API](https://developer.android.com/games/gamemode/gamemode-api)的应用程序。一旦发生这种情况，我们将能够在每场比赛的基础上选择一个性能档案。