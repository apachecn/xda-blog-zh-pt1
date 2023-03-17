# Android 12 DP2 Changelog:我们发现的所有隐藏功能！

> 原文：<https://www.xda-developers.com/android-12-dp2-hidden-features/>

谷歌今天早些时候发布了 [Android 12](https://www.xda-developers.com/android-12/) 的[第二次开发者预览](https://www.xda-developers.com/android-12-developer-preview-2/)，它包括了几个应该会让用户兴奋的新功能。首先，正如我们[上个月第一次报道](https://www.xda-developers.com/android-12-brings-pinch-to-resize-and-stashing-for-picture-in-picture-windows/)一样，有新的画中画手势。开发人员现在可以轻松地将模糊效果应用到背景中，此外还改进了通知可见性，以获得更好的隐私。但除了官方宣布的变化，Android 12 开发者预览版 2 中还有许多新功能存在或隐藏。这是我们发现的所有隐藏功能的总结。

## 浏览这篇文章:

目前，在 Pixel Launcher 主屏幕底部或应用程序列表顶部看到的搜索小工具由谷歌应用程序提供支持。谷歌应用相当臃肿，因为它包含了谷歌搜索、谷歌助手、谷歌镜头、谷歌播客等服务。因此，当前的搜索工具打开起来会很慢，但谢天谢地，谷歌有解决这个问题的办法。该公司正在开发一个不依赖于谷歌应用的新搜索工具提供商。实际上，我们在 Android 12 DP1 中已经看到了这个特性，但是 DP2 对这个特性进行了一些改进。

在下面嵌入的截图库中，你可以看到谷歌正在测试应用列表中的新搜索界面。这个搜索界面打开得非常快，可以让你在手机中搜索应用程序、联系人、设置等等。然而，它在 Android 12 DP2 中无法正常工作，所以我们只能搜索设备上安装的应用程序。

## 大屏幕设备的任务栏

Pixel Launcher 中隐藏的另一个功能是任务栏。该任务栏出现在屏幕底部，并在所有应用程序中保持不变。它会显示您最常用的应用程序以及一些您最近使用的应用程序。不过，它只会出现在大屏幕设备上。像三星的 Galaxy Tab S7 这样的平板电脑可能符合条件，但我们不知道这一功能是否会进入 AOSP 的 Launcher3 代码库。

[video width = " 1314 " height = " 638 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/03/Pixel-Launcher-taskbar . MP4 "]

Android 现在已经为几个版本提供了隐藏的桌面模式界面，所以这可能是让桌面模式更有用的第一步。

## 基于人脸的自动旋转

在第一个 Android 12 开发者预览版发布之前，我们得知谷歌正在开发一个更智能的自动旋转系统。具体来说，我们了解到谷歌正在准备一个基于面部的自动旋转系统，该系统将使用你的前置摄像头来检测你何时在看屏幕，以防止用户界面旋转。在 Android 12 DP2 中，增加了该功能的代码。一旦这个功能被启用，你会看到“基于面部”被添加到“自动旋转屏幕”设置的潜台词中。

 <picture>![Android 12 DP2 face-based autorotate](img/53685d713cf1b63d13601d13c2b2882a.png)</picture> 

Credits: Mishaal Rahman

这个功能的一个字符串提到它可以帮助你躺着阅读内容。对我来说，当我在床上使用手机时，我总是禁用自动旋转(我知道这是个坏习惯)。基于面部的自动旋转将确保每当我在床上浏览 Reddit 时，UI 不会旋转。

## 游戏仪表板

我们上个月首次报道了谷歌正在 Android 12 中开发浮动游戏工具栏。这个工具栏在屏幕上覆盖了两个图标，其中一个可以让你开始屏幕录像。然而，这还不是全部。我们还谈到了一个游戏仪表板类，我们怀疑它将包含更多的功能。在 Android 12 DP2 中，我们发现了游戏仪表板上的工作，尽管它还远远没有准备好。

目前，隐藏的游戏仪表板有一个小部件，可以通过 YouTube Live 启动直播流。它还有一些设置切换，如截图，开始屏幕录制，切换 FPS 计数器，以及切换勿扰模式。目前还有一个小部件是空的，但在不久的将来，它可能会包含一些其他有用的快捷方式。

上个月，XDA 知名开发者 Quinny899 让我们第一次看到了 Android 12 的对话小工具。我们第一次知道这个特性是在我们获得一份概述主要新平台特性的文件的时候。现在，我们可以提前看看这个小部件的开发中的小部件选择器 UI。

这在很大程度上仍然是一项正在进行的工作，所以最终的结果可能会看起来更加精细。目前，对话小部件的默认大小是 3x2，考虑到实际内容，这个大小太大了。此外，我们看不到为联系人显示重要事件的选项，如生日或纪念日。作为参考，我们发布的文档显示了一个通知用户联系人生日的小部件。不过，快速浏览一下 SystemUIGoogle 的字符串可以发现，Google 仍在致力于此。

## 改进的大头针视图

在我们对 Android 12 DP2 中发现的所有[新功能的报道中，我们提到锁屏 PIN 视图已经接受了轻微的 UI 更改。我们注意到“紧急呼叫”按钮现在用与系统强调色匹配的背景色填充。现在，我们还为大头针视图启用了一个全新的 UI。这个新的用户界面的特点是数字和 delete 和 enter 键有大气泡。然而，数字和 delete/enter 键的背景颜色是不同的，这使得它们更容易区分。](https://www.xda-developers.com/android-12-dp2-new-features/)

PIN 视图的新用户界面可能是谷歌对锁屏进行更广泛调整的一部分，这是我们上个月首次报道的。

## 增强型 Monet 主题系统

上个月，开发者向我们展示了谷歌新的基于壁纸的主题系统，代号为“莫奈”当“莫奈”被启用时，用户的壁纸决定了整个设置和 SystemUI 的背景色和强调色。然而，在 DP1 中，“莫奈”只是部分重新着色设置。现在在 Android 12 DP2 中，每个设置页面都使用了基于你的壁纸的主题进行了彻底的改造。

此外，“monet”的范围已经扩展到主题化锁屏 PIN/图案视图、Pixel Launcher 中的对话框和 Pixel Launcher 中的应用程序列表。

在幕后，“莫奈”正在使用一种更复杂的方法来确定任何给定壁纸的最佳颜色。根据 kdrag0n 的说法:“基于壁纸的主题系统 Monet 现在使用 CAM16 感知颜色模型进行更准确的颜色提取。DP1 使用简单的 HSL(色调-饱和度-亮度)转换，这可能会产生奇怪的颜色，因为它没有模拟人眼看到的东西。

## 新的 Toast 消息用户界面

接下来，谷歌也在致力于调整吐司信息用户界面。Toast 消息包含无法操作的简单消息，但并不总是清楚是什么应用程序生成了它们。在 Android 12 DP2 中，谷歌正在测试一个新的 toast 消息 UI，该 UI 显示生成消息的应用程序的图标。在下面的截图中，生成 toast 消息的应用程序是 Android 12 的 SystemUI。

 <picture>![Android 12 toast message](img/a67a546312801cc41f05088af52ccaf8.png)</picture> 

Credits: kdrag0n

## 新锁屏打开/关闭动画

Android 12 DP2 中隐藏的另一个变化是一个显示/隐藏锁屏的新动画。下面是一段屏幕录音，由 Telegram 用户 kampotik 提供(via kdrag0n)。

[video width = " 540 " height = " 1140 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/03/Android-12-DP2-New-lock screen-animation . MP4 "]

如果你很好奇，这个屏幕记录是在谷歌 Pixel 4 上制作的。[在后续视频](https://twitter.com/MishaalRahman/status/1372646681133584389)中，我们的线人展示了在实际设备上播放的新锁屏转换动画。如您所见，动画在实际电源按钮附近开始和结束。根据 kdrag0n 的说法，动画是从你解锁的点开始的，也就是说向上滑动从底部开始动画，按下电源键从侧面开始动画。

再次感谢开发者 kdrag0n，我们现在可以展示即将到来的 Android 12 版本中的另一个 UI 变化。这一次，我们可以确认谷歌正在测试当你试图滚动页面顶部或底部时播放的过度滚动动画。此外，还有一个新的涟漪效应，当你点击任何项目时都会播放。根据[官方 Android 文档](https://developer.android.com/reference/android/graphics/drawable/RippleDrawable#STYLE_PATTERNED)，这种效果可以被描述为“一种具有图案化、嘈杂内部的圆形形状从热点扩展到边界的风格。”

[video width = " 576 " height = " 1216 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/03/Android-12-DP2-Ripple-Effect-and-over scroll . MP4 "]

## 摄像头和麦克风的隐私指示器

在我们早期泄露的 Android 12 中，我们发现谷歌正在努力在应用程序使用摄像头或麦克风时显示状态栏指示器。我们还了解到，点击这些指示器会显示一个弹出窗口，告诉您哪些应用程序当前正在使用这些传感器。在深入研究 Android 12 DP2 的代码时，我们确认这些功能正在开发中。多亏了 [kdrag0n](https://mobile.twitter.com/kdrag0n/status/1372783638803214338) ，我们现在可以向您展示这些特性在当前版本中的样子。

## 其他变化

以下是我们发现的其他一些较小的变化:

*   继续致力于使 Android 12 [更加单手友好](https://www.xda-developers.com/android-12-better-one-handed-use/)。添加了应用信息页面和系统仪表板的新 V2 布局。
*   显示[设备控制菜单](https://www.xda-developers.com/android-11-power-menu-device-controls-smart-home-dream/)的快速设置磁贴正在制作中。
*   在 Android Auto 的 APK 存根中发现了三个像素代号:barbet、raven 和 oriole。

* * *

Android 12 开发者预览版 2 中肯定会有我们尚未启用的其他功能。一旦我们让它们工作起来(或者放弃尝试)，我们会用我们了解到的任何细节更新这篇文章。如果你有兴趣了解我在 Android 12 DP2 中发现的所有其他变化，[请查看我的 Twitter](https://twitter.com/MishaalRahman/status/1372231611488559110) ，我们在 Twitter 上发布了我发现的所有内容。否则，请参考[我们的 Android 12](https://www.xda-developers.com/android-12/) 英雄页面，深入了解谷歌新操作系统。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*