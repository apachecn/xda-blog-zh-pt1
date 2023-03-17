# Android 12.1 测试可折叠手机在像素折叠方面的改进

> 原文：<https://www.xda-developers.com/android-12-1-foldable-phone-enhancements-pixel-fold/>

根据 XDA 审阅的一份文件，Android 的下一次重大更新将于 10 月 4 日发布。 [Android 12](https://www.xda-developers.com/android-12/) 将是多年来最大的 Android 操作系统更新，带来完整的重新设计，新的主题引擎，单手模式，等等。由于更新的范围如此之广，谷歌可能没有时间添加一个或多个计划中的功能，将这些功能推到下一个版本。我们最近了解到，Android 的[下一个版本可能是一个点更新](https://www.xda-developers.com/android-12-v2-update/)，但我们当时不确定为什么。现在，我们已经了解了更多关于预计的 Android 12.1 更新的功能，它们涉及到可折叠手机体验的几项增强。

Android 12 sc-v2 版本，我们预计将被称为 Android 12.1，将在早期 Android 12 开发者预览版中首次出现的功能基础上进行改进。在 Android 12 开发者预览版 2 中，我们在 Pixel Launcher 中启用了一个[隐藏的“任务栏”功能](https://www.xda-developers.com/android-12-dp2-hidden-features/#android12dp2taskbar)，它出现在导航栏通常所在的屏幕底部，并显示一些您经常使用的应用程序和最近使用的应用程序。这种任务栏是为平板电脑等大屏幕设备开发的，平板电脑的屏幕更适合多任务处理。

然而，自从我们第一次在开发者预览版 2 中看到任务栏以来，我们还没有在后续的 Android 12 预览版中看到该功能的任何重大改进。正如我们现在所知，原因是因为谷歌正在为 Android 12.1 开发幕后功能。此外，我们了解到谷歌正在为另一类大屏幕设备开发这一任务栏功能:可折叠手机。这具有直观的意义，因为像三星 Galaxy Z Fold 3 和 T2 华为 Mate X2 这样的可折叠产品在展开时本质上就是迷你平板电脑。Galaxy Z Fold 3 在展开时甚至可以显示许多应用程序的平板版本，并且[如果传言是真的](https://www.xda-developers.com/google-pixel-foldable-samsung-display/)，谷歌 Pixel Fold 在展开时可能与三星的可折叠平板一样大，为 7.57 英寸。虽然我们不能直接确认谷歌是否正在专门为 Pixel Fold 开发 Android 的任务栏功能，但我们可以确认可折叠是该功能的一种形式。

谷歌的内部 AOSP 代码库包含了对当前准系统任务栏功能的几项改进。实现任务栏教程的代码更改描述了它的一些计划功能。首先，进入教程将显示一个被描述为“波浪”的动画，其中图标按比例放大和平移，然后再缩小。该教程然后解释了如何通过将应用程序图标拖到屏幕的一侧来在分屏视图中启动两个应用程序，触摸并按住以随时隐藏任务栏(停靠)，并将您最喜爱的应用程序/预测的应用程序添加到任务栏。一旦设置完成，任务栏会停留在屏幕底部，但当应用程序进入全屏时会自动隐藏。

实现任务栏教程的一个代码更改包括了一个正在运行的功能的图像。下面嵌入的图片显示了一部并排运行两个 Chrome 实例的可折叠手机，这一功能目前正在测试中。在两个 Chrome 窗口之间可以看到分屏的分隔线，而任务栏位于中间，横跨两个窗口的底部。

Google 在任务栏教程的最初实现中包含了这张图片，但是他们后来把它换成了更通用的渲染。谷歌不太可能因为意外展示了未发布的 Pixel Fold 而交换了图像，但图像的存在至少表明谷歌正在开发可折叠手机的功能。

不过，这并不是 Android 12.1 中唯一旨在改善可折叠手机体验的软件变化。Android 12.1 中的各种补丁为 SystemUI 中展开的动画增加了更好的处理。例如，一个补丁描述了当展开可折叠手机时，任务栏中图标的“从中心移动”动画。另一个补丁在展开动画时增加了对[铰链角度传感器](https://developer.android.com/reference/android/hardware/Sensor#STRING_TYPE_HINGE_ANGLE)的支持。另一个补丁支持在双窗格模式下从系统或预装的应用程序中打开一个活动，只要该活动从设置中[深度链接](https://developer.android.com/training/app-links/deep-linking)。

我们不知道 Android 12.1 会带来什么，但很明显，除了新的壁纸之外，我们还应该期待可折叠手机的一些改进。我们不知道谷歌是否打算在 Android 12.1 中推出 Pixel Fold，但鉴于我们在 point release 中看到的所有新的可折叠相关补丁，这是有意义的。不幸的是，Pixel Fold 是谷歌迄今最难以捉摸的 Pixel 手机，只有少数[供应链泄露](https://www.xda-developers.com/googles-foldable-pixel-phone-ultra-thin-glass-layer/)暗示其可能的显示规格。这部代号为“护照”的手机一直是一个受到严格保护的秘密，即使在 AOSP 的非公开资料库中，提到它也是罕见的。然而，一个内部代码的变化指向了 2208x1804 的屏幕分辨率和侧装指纹扫描仪，尽管我们无法验证这两种规格，因为在“passport”设备的补丁说明中没有直接提到。我们将不得不等待这款手机的发布，然后才能了解它的更多信息。

说到这里，显示供应链顾问公司(DSCC)的首席执行官罗斯·杨认为，Pixel Fold 将于今年年底推出[LTPOOLED 面板和高达 120 赫兹的可变刷新率。如果这款手机确实在 2021 年第四季度推出，我们会感到惊讶，因为谷歌在遏制泄密方面没有最好的记录。](https://twitter.com/DSCCRoss/status/1438339317470957573?s=19)