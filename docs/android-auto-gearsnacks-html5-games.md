# 谷歌希望将 HTML5 游戏带到你的安卓汽车屏幕上

> 原文：<https://www.xda-developers.com/android-auto-gearsnacks-html5-games/>

前几天，Reddit/r/Android auto 社区的用户注意到一个神秘的“car 零食”图标出现在他们汽车的应用程序列表中。除了 Reddit 帖子，在网上任何地方都找不到“gear 零食”的参考资料，但在启动应用程序后，人们发现“gear 零食”包含了大量的小游戏。在深入研究了最新的 Android Auto APK 之后，我们可以确认“car 零食”可以让你在汽车的仪表盘上玩谷歌 GameSnacks 平台的 HTML5 游戏。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

redditor/u/million mile 8[昨天发布了](https://www.reddit.com/r/AndroidAuto/comments/oi5qpp/anyone_know_what_gearsnacks_isdoes/)一张截图，显示了他的 Android 汽车应用列表中的“gear 零食”。当他们启动应用程序并加载游戏时，他们[说](https://www.reddit.com/r/AndroidAuto/comments/oi5qpp/anyone_know_what_gearsnacks_isdoes/h4wyazb/)他们注意到“谷歌在底部给你带来了类似 602 (idk 实际数字)的游戏。”我们设法在应用列表中手动显示 gear 零食，感谢 Redditor [RegionRat91](https://www.reddit.com/user/RegionRat91) ，我们也有了显示通过 gear 零食可以玩的 HTML5 游戏的图像。

 <picture>![GearSnacks in Android Auto app list](img/ec3cf87ec53df42386535a7f16a47159.png)</picture> 

Credits: Mishaal Rahman

在深入研究了最新的 Android Auto 版本之后，我们发现了与 GameSnacks 直接相关的 gear 零食的多个参考文献。对于那些不知道的人，GameSnacks 是来自 120 区的 HTML5 游戏平台，120 区是谷歌的实验项目实验室。(之前的 Reddit 用户可能想到的是“120”而不是“602”。)在 2020 年初宣布，GameSnacks 提供了一口大小的 HTML5 游戏，可以在任何具有网络功能的设备上玩。每款游戏都支持触摸、键盘和鼠标输入，可以通过官方 [GameSnacks 网站](https://gamesnacks.com/embed/)在 Android、iOS 和 PC 上玩。今年早些时候，谷歌[开始在几个地区将 GameSnacks 的 HTML5 游戏整合到谷歌产品中，包括 Chrome、Google Pay、Google Assistant 和 Google Discover。在那份公告中，谷歌表示将“寻找更多机会将 GameSnacks 游戏带到更多谷歌产品中”，似乎 Android Auto 也在考虑之中。](https://blog.google/technology/area-120/gamesnacks-html5-games-google-products/)

目前，似乎 HTML5 游戏的完整目录无法通过 Android Auto 获得，一名用户[报告](https://www.reddit.com/r/AndroidAuto/comments/oi5qpp/anyone_know_what_gearsnacks_isdoes/h4v0l9g/)只有 3 款游戏可供他们使用。当我们检查 Android Auto 的代码时，我们发现了 8 个似乎正在为 Android Auto 优化的 HTML5 游戏的链接，包括[动物园热潮](https://gamesnacks.com/embed/auto/games/zooboom/)、 [Onet 连接经典](https://gamesnacks.com/embed/auto/games/onetconnectclassic/)、[炮弹 3D](https://gamesnacks.com/embed/auto/games/cannonballs3d/) 、[牵制飞碟](https://gamesnacks.com/embed/auto/games/pintheufo/)、 [2048 巨人](https://gamesnacks.com/embed/auto/games/2048giant/)、[找到 500 个差异](https://gamesnacks.com/embed/auto/games/find500differences2/)、[解锁那个](https://gamesnacks.com/embed/auto/games/unblockthat/)和[泡泡森林](https://gamesnacks.com/embed/auto/games/bubblewoods4/)。每个 Android 自动优化游戏的 URL 都包含“Auto”；在 GameSnacks 上现有 HTML5 游戏的 URL 中添加“auto”可以预见不会调整布局，这表明谷歌正在努力逐个优化游戏。

APK 内的一个字符串表示“游戏只能用你的触摸屏玩”，所以似乎只有装有触摸屏的车辆才被允许玩。值得注意的是，除非用户停车，否则 gear 零食无法启动，这是有道理的，因为谷歌不希望用户在开车时玩触屏游戏。然而，[自今年 2 月](https://www.xda-developers.com/android-password-checkup-scheduled-messages/)起，通过调用谷歌助手，可以在驾驶时玩选定的声控游戏。

谷歌还没有宣布 gear 零食，但很可能过不了多久他们就会宣布了。

Android Auto 中 games nacks/gear 零食的图片。学分:[/u/regionrat 91](https://www.reddit.com/user/RegionRat91)

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*