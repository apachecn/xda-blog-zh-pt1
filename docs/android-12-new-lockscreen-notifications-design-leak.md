# Android 12 的新锁屏和通知用户界面可能已经泄露

> 原文：<https://www.xda-developers.com/android-12-new-lockscreen-notifications-design-leak/>

今天早些时候，谷歌发布了第一个用于 Pixel 智能手机的 [Android 12](https://www.xda-developers.com/android-12/) [开发者预览版](https://www.xda-developers.com/android-12-developer-preview-1/)，我们一直在挖掘该版本，以找到[所有新的](https://www.xda-developers.com/tag/android-12/)。下一个 Android 版本最令人期待的变化之一是一个全新的用户界面，我们已经瞥见了 Android 12 新发现的单手友好性。现在，我们已经成功启用了一个新的用户界面，用于始终显示、锁屏和通知，进一步证实了谷歌今年计划彻底改变 Android 的用户界面。

*注意:本文中显示的用户界面变化正在进行中。Android 12 开发者预览版 1 中没有新的 UI——谷歌故意在预览版中禁用了新的 UI。正如我们将在下面解释的那样，在稳定版发布之前，UI 的一些元素可能会发生变化。*

上周，我们[获得了我们认为是 Android 12 设计模型的图片](https://www.xda-developers.com/android-12-first-look-screenshots/)，展示了新操作系统[传闻中的主题系统](https://www.xda-developers.com/android-12-theming-system/)。我们分享的其中一张图片展示了通知面板的全新 UI。该模型显示了浅米色的不透明背景，通知上的圆角，摄像头和麦克风的隐私指示器，以及日期和时间的交换位置。

本周一，我们发表了一篇文章，独家报道了谷歌在 Android 12 中重新设计 Android 的努力。那篇文章详细介绍了永远显示、锁屏、锁模式视图等方面的许多变化。在分析了 Android 12 开发者预览版 1 后，我可以确认所有这些变化都在开发中，但我们还没有能够实现所有这些变化。然而，我们已经准备好分享谷歌调整总是显示、锁屏和通知的一些方法。

*Android 12 DP1 当前的锁屏和通知 UI*

正如我们之前解释的那样，谷歌正在尝试 Android 12 的锁屏设计和布局。一些可能的变化包括将数字钟放在中间的前端和中心。现在小时在分钟之上，字体巨大。同时,“一览”小部件被移到了左上角。当收到通知时，时钟会缩小并移到锁屏的右上角。在“始终显示”中，通知图标显示在概览小部件下方的左上角，而不是中央。就我个人而言，我并不喜欢当前版本的这种新设计，尽管我承认它仍然是一个 WIP，而且会有很多变化。一旦谷歌[启用锁屏时钟定制](https://www.xda-developers.com/android-q-lock-screen-clock-customization/)，这个设计可能会看起来更好，但我们还没有设法让任何其他类型的时钟出现在这个视图中。

*Android 12 正在开发的锁屏和 AOD 界面*

我们也无法让[设备控制功能](https://www.xda-developers.com/android-11-power-menu-device-controls-smart-home-dream/)显示在锁屏上，尽管我们已经证实谷歌正在努力将该功能更紧密地集成到锁屏中。我们也没有看到锁模式视图有任何根本性的变化，尽管我们在动手操作时确实发现了动画[的细微调整。](https://www.xda-developers.com/android-12-developer-preview-hands-on/#div-gpt-ad-xda-developerscom35949:~:text=Furthermore%2C%20the%20animation%20for%20the%20pattern%20unlocks%20also%20appears%20slightly%20bouncier.)

接下来，让我们先睹为快，看看 Android 12 中通知面板的一些变化。谷歌正在测试一种与你的白天/夜晚主题相匹配的不透明背景，而不是当前 UI 的大部分透明背景。一旦传闻中的 Android 12 主题系统上线，背景颜色可能会与你的壁纸相配。如果是这样，这就解释了我们发布的设计模型中展示的浅米色背景。无论如何，我们已经确认谷歌正在开发一个基于壁纸的主题化系统，代号为“莫奈”，但我们还没有激活它。

除了不透明的背景，我们还发现了之前提到的较粗的亮度条。股票 Android 目前的亮度条是细条，而新设计更多的是粗药丸。快速设置图块没有改变，尽管标签已经从这次迭代中消失了。我们知道谷歌正在研究另一个将标签放在侧面的设计，但是我们还不能让它工作。

*Android 12 的开发中通知面板界面*

我们要注意的一件事是，谷歌的一些开发中的变化在我们启用它们时破坏了通知。谷歌似乎正在开发一个新的通知管道和一个两栏式的通知用户界面，后者我们之前已经透露过了。我们无法让新的通知管道或布局与其他 UI 更改一起工作，但我们会在这次和未来的预览版中继续尝试。

我们将继续挖掘第一个 Android 12 开发者预览，看看我们能找到什么。我将会把我在推特上发现的许多变化贴在[这个正在运行的线程](https://twitter.com/MishaalRahman/status/1362462100958887940)上，这些变化是我到目前为止发现的。如果你不喜欢 Twitter 的布局，我们还会对我在 XDA 发表的所有发现进行更详细的报道。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*