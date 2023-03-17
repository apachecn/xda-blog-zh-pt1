# Google 相册会在图像库中为您准备较大文本的素材

> 原文：<https://www.xda-developers.com/google-photos-material-you-tweaks/>

在上个月的谷歌 I/O 大会上，谷歌公布了其设计语言的第三次重大迭代。 [Material You](https://www.xda-developers.com/material-you/) 为 Android 和其他谷歌开发的平台带来了更新的外观和感觉。新的设计强调定制、圆角和大标题文本。我们在 [Android 12](https://www.xda-developers.com/android-12/) 测试版中瞥见了谷歌如何调整 Android 的设计，使其更加单手友好，现在我们看到了同样的设计原则正在以微妙的方式扩展到谷歌照片应用程序的证据。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

tipster @[deviced _ im](https://twitter.com/damned_im)联系了我们，称他们在谷歌照片应用的 5.43 版本中发现了一个新设计。在他们发给我们的截图中，我们可以看到谷歌将日期的标题文本放大了很多。这些图片让我们想起了 Android 12 中的新设置应用，但有趣的是，我们的线人在第一代 Pixel 上运行 Android 10。不过，在旧版本的 Android 上看到你重新设计的应用程序应该不会太惊讶，因为它只是一种新的设计语言，而不是最新版本的操作系统的一部分。Material You 仅限于 Android 12 的唯一方面是更新的颜色提取算法，用于[根据你的壁纸](https://www.xda-developers.com/android-12-wallpaper-theme/)对系统和应用进行主题化，但即使如此，旧版本的操作系统中也存在不太健壮的颜色提取 API。(值得注意的是，实际的主题生成算法是谷歌专有的。)

无论如何，经过一点努力，我们能够重新设计我们的线人展示的 Google 相册。除了让标题文本变得更大，还有一些功能上的变化。例如，当您放大并滚动图像库时，当前图像组的拍摄日期会持续显示在左上角(下面的第二个图像)。在过去的几周里，Google 相册在顶部添加了一系列新的记忆，但该应用程序还准备将这些记忆与图片库一起显示(下面是第三和第五张图片)。如果您在某个日期创建了一个图像相册，当您在图像库中滚动时，该相册也可能会以内嵌方式显示(下面的第四个图像)。最后，Photos 应用还在测试一个溢出菜单，点击它会显示一个“选择”按钮。如果给定日期的所有图像都是在一个公认的位置拍摄的，那么溢出菜单可能还会显示一个“查看地图”按钮，快速将您带到应用程序的[地图视图](https://www.xda-developers.com/google-photos-new-logo-redesign/)。

*新设计*

*旧设计*

谷歌照片是我们发现的第一个按照你的风格重新设计的主要谷歌应用。有迹象表明，谷歌 Chrome 正在进行大规模的重新设计，但迄今为止我们看到的[变化](https://www.xda-developers.com/chrome-preps-material-you-android-12-bouncy-scrolling/)一直很微妙。我们将继续关注照片应用的更多调整，因为我们仍然没有看到最令人期待的变化之一:支持“[莫奈](https://www.xda-developers.com/android-12-wallpaper-theme/)”

* * *

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*