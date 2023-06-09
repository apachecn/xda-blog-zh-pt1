# Android 12 Beta 1 实践:对 Android 进行彻底的重新设计

> 原文：<https://www.xda-developers.com/android-12-beta-1-hands-on/>

随着 Android 12 Beta 1 的发布，谷歌(以及许多其他合作伙伴 OEM 厂商)发布了第一个适用于 T2 谷歌 Pixel 智能手机 T3 的可安装测试版。虽然它离成品还很远(并且缺少很多将在未来测试版中添加的功能)，但它让我们领略了未来的发展——最终版本将在今年晚些时候发布。我在我的[谷歌 Pixel 5](https://www.xda-developers.com/google-pixel-5-review/) 上安装了 Android 12，以下是我使用它的第一印象。

如果你感兴趣的话，我们有一篇关于如何在你的谷歌 Pixel 或其他 Android 设备上下载和安装 Android 12 Beta 1 的便利文章，尽管如果你持观望态度，我们已经安装并试用了它！

**[Android 12“雪锥”:关于谷歌下一次大更新](https://www.xda-developers.com/android-12/)** 我们目前所知的一切

## 随着 Android 12 Beta 1 的发布，用户界面经历了一次大规模的革新

Android 团队认为 Android 12 是自 Android 5.0 以来最大的重新设计，老实说，我能看出为什么。*一切*都不一样了。这就是谷歌称之为“[材料你](https://www.xda-developers.com/material-you/)”——一个为你建造的材料设计的迭代。这或多或少是一次彻底的重新设计。锁屏不一样，通知和快捷设置不一样，连设置 app 都不一样。还有一个新的模式和 pin 解锁屏幕。

动画也是 Android 12 的一大部分，因为在整个 UI 中都添加了新的动画。例如，点击某些 UI 元素会生成一个向外流动的动画，产生一种“涟漪”效果。

滚动到列表底部(就像在设置应用程序中一样)也会产生弹跳效果。

[video width = " 303 " height = " 624 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/05/Android-12-Beta-1-over scroll . MP4 "]

边上还有一个新的音量控制滑块，有一个新的动画，可以在请勿打扰、振动和铃声之间切换。

[video width = " 303 " height = " 624 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/05/Android-12-Beta-1-New-Volume-panel . MP4 "]

最后，甚至有一个新的屏幕上和屏幕下的动画。

[video width = " 303 " height = " 624 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/05/Android-12-Beta-Screen-on-and-off-anim . MP4 "]

深入研究设置，我发现有几个部分还没有被重新设计，但鉴于这是一个测试版，这肯定会在未来发生变化。我还注意到 UI 元素[还没有改变颜色来适应壁纸](https://www.xda-developers.com/android-12-wallpaper-theme/)。颜色提取功能是新的“你的材料”重新设计的最大方面之一，它将在今年晚些时候出现在 Pixel 手机上(希望之后会出现在其他手机上)。

## 这只是一个测试版，测试版并不完美

浏览每一个菜单，很明显，系统在设计变化背后有某种形式的单一用户界面影响，非常注重单手使用。暗模式在像素 5 上也不再是黑色，而是一种相当亮的灰色。我希望谷歌至少会把它变暗，因为它现在很亮，在黑暗中看起来会不舒服。虽然有一个新的辅助选项，允许你在已经达到最低亮度的基础上进一步调暗屏幕，这在某种程度上弥补了它。一旦打开，它会在快速设置中添加一个屏幕变暗选项，您可以在任何地方启用该选项。

在删除的功能方面，谷歌似乎已经在电池设置中删除了按时查看屏幕的功能，尽管它可能会在未来的更新中重新出现。

然而，我在谷歌 Pixel 5 上使用 Android 12 的最大收获是，大多数功能还没有出现。像[隐私仪表盘](https://www.xda-developers.com/android-12-privacy-private-compute-core-privacy-dashboard/)和[重新设计的小工具](https://www.xda-developers.com/google-android-12-widgets-overhaul/)这样的新功能还没有出现，尽管你可以在请求位置许可的应用上禁用“使用精确位置”。谷歌表示，新的隐私仪表盘和摄像头/麦克风访问阻止将在第二次测试更新中进入 Android 12，预计将在未来几个月内推出。当一个应用程序读取你的剪贴板时，一个通知也将出现在第二个测试版中。谷歌还提到，快速设置将为你的家庭和谷歌支付提供控制，尽管这也还没有出现。谷歌表示，它已经在 beta 1 中添加了[应用休眠](https://www.xda-developers.com/android-12-hibernate-unused-apps/)，它将自动删除未使用应用中的临时文件，以节省存储空间。他们还增加了按住电源按钮触发谷歌助手的功能，同样的，在背面双击，然而，这还不能用。最后，他们错过了[期待已久的滚动屏幕截图功能](https://www.xda-developers.com/android-12-finally-adds-scrolling-screenshots-natively/)，尽管谢天谢地它很快就会到来，因为它在官方博客帖子中提到过。

所有这些功能都将出现在秋季谷歌 Pixel 手机的最终 Android 12 版本中，但就目前而言，我们还不能使用它们。看起来这个第一个测试版是为了让新的 Android 版本进入开发者的手中，并推出新的 UI。这是有道理的，因为我已经看到有人抱怨 Twitter 如何在他们的 Android 12 谷歌 Pixel 5 上崩溃。虽然我没有经历完全相同的行为，但我注意到 Twitter 应用程序的用户界面看起来很奇怪。我还贴了一张照片来测试，Twitter 应用程序在我贴了五分钟后拒绝启动。如果你是一个狂热的 Twitter 用户(像我一样！)那么仅仅因为那个就值得远离。由于过度滚动动画，用户界面跳来跳去，底部的动画由于涟漪效应看起来很奇怪。

\ r \ nht TPS://www . YouTube . com/watch？v=LTZySY-Hk_M\r\n

总的来说，谷歌 Pixel 5 上的 Android 12 Beta 1 是可用的，但还远非完美。虽然我曾想过将 Pixel 5 用作我的新日常驱动程序，但我决定反对它，因为添加的功能数量不足以忍受我将遇到的潜在问题。我已经知道 Twitter 处于不可用的边缘，我预计其他应用程序也可能会出现同样的情况。因此，我不建议安装它，除非你真的*想让*摆弄它，或者如果你有一个你不介意使用的辅助设备。我喜欢它的外观，我期待着在未来测试所有的新功能！