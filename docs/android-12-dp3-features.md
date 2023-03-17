# Android 12 DP3 Changelog:我们发现的所有新功能！

> 原文：<https://www.xda-developers.com/android-12-dp3-features/>

今天早些时候，谷歌发布了 Android 12 的第三个开发者预览版。官方上，这次发布再次面向开发者，为触觉、相机等带来了[新的 API](https://www.xda-developers.com/google-android-12-developer-preview-3-features/)。像往常一样，我们通过快速实践发现了一些面向用户的新功能。如果你有兴趣了解 Android 12 开发者预览版 3 中有哪些新功能，请继续阅读！

我们在 DP3 中发现的许多面向用户的变化也在 Android 12 的泄露版本中发现，我们上周独家详细介绍了该版本。

* * *

## 浏览这篇文章

* * *

## Android 12 DP3 中面向用户的新功能

### 默认情况下启用单手用户界面

Android 12 最大的变化之一是改进的设置用户界面，更加单手友好。在开发者预览版 1 中首次发现，新的单手 UI 现在在开发者预览版 3 中对每个人都可用——不需要标志。

在开发者预览版 2 中，谷歌正在测试一种新的滚动动画，当你试图滚动页面的顶部或底部时，它就会播放。在 Android 12 DP3 中，这种过度滚动动画现在在整个框架中默认启用。任何可以滚动的地方，你都可以超滚。这包括延伸超过快速设置面板的左边缘或右边缘，延伸超过对话框的末端，或者只是向上或向下滚动超过任何标准列表视图的边界。

默认情况下，点击任何项目时看到的[涟漪效果](https://www.xda-developers.com/android-12-beta-features-leak/#android12leakrippleoverscroll)是不启用的，但我们可以确认该功能仍然被隐藏起来。

### 每个应用程序的闪屏

谷歌在 Android 12 DP3 的博客文章中提到的一个功能是为每个应用程序引入自动生成的闪屏。新的应用程序启动动画包括一个闪屏，显示应用程序图标和应用程序本身的过渡。开发人员可以自定义闪屏的背景颜色，用自定义图标或动画替换静态启动器图标，控制显示应用程序的时间，设置亮或暗模式，以及自定义退出动画。

[video width = " 652 " height = " 1344 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/04/Android-12-Splash-screens . MP4 "]

由于开发者预览版 3 刚刚发布，我们使用过的应用程序都没有利用这个 API，所以如果一个应用程序已经实现了自己的闪屏，那么闪屏看起来会有点普通或多余。

### 一切(甚至更)圆

默认情况下，UI 中有圆角的部分甚至有更多的圆角。虽然圆角在过去的版本中更加微妙，但 Android 12 DP3 正在全力以赴地采用圆角。圆角甚至延伸到您添加到主屏幕的小部件！

### 新的，更活泼的音量面板用户界面

我们[在泄露的 Android 12 build](https://www.xda-developers.com/android-12-beta-features-leak/#android12leaknewvolumeui) 中首次发现的设计变化现在在 DP3 中为每个人直播。薄体积面板已被更大、更圆的面板取代。

### 像素发射器有一个新的应用程序抽屉动画

我们在泄露的 Android 12 版本中发现的另一个变化是显示应用抽屉的新动画。DP3 中的应用抽屉动画比我们在泄露的版本中看到的版本慢了一点，但物理特性非常相似。

[video width = " 320 " height = " 656 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/04/5-Pixel-Launcher-App-Drawer-animation . MP4 "]

你安装了很多应用程序吗？那些应用程序有大量的插件吗？如果是这样，您可能很难找到合适的 widget 添加到主屏幕。这就是为什么在 Android 12 DP3 中，谷歌在 widget picker 中增加了搜索栏。除此之外，Pixel Launcher 还在顶部展示了一些推荐的小部件。小部件推荐功能[在我们之前发布的泄露版本](https://www.xda-developers.com/android-12-beta-features-leak/#android12leakwidgetsearchbar)中并不存在，但这很可能是因为我们运行的是 Pixel Launcher 的开源版本。

### 电池电量估计现在有一个进度条

在“设置”>“电池”中，随着电池充电而填满的巨大电池图标已经被一个更简约的进度条所取代。

### 标记图像编辑器现在允许您更改字体

Markup 是一款谷歌应用，用于快速编辑截图。在 Android 12 的早期版本中，谷歌增加了一个文本工具，让你可以在图像上写文本。在 DP3 中，您现在可以更改该文本的字体。

在开发者预览版 1 发布之前，我们先来看一下 Android 12 ,谷歌计划增加一个“对话”小工具。经过一点努力，我们能够让小部件[在 DP1](https://www.xda-developers.com/android-12-conversation-widget-first-look/) 中部分工作。这个小部件现在在开发者预览版 3 中向一些用户显示，看起来它实际上是从最近的消息中提取文本。对话窗口小部件的选择器也进行了改进，与我们上周发现的一致。

不过，这个小工具的设计显然还不完整，因为应用程序的图标和/或更大的对话预览可能会占用大量空间。此外，点击小工具会打开一个选择器，它实际上并不包含正确的对话快捷方式(在这种情况下，我在 Telegram 应用程序中与 XDA 的 Zachary Wander 的对话)。很明显还有很多工作要做，但是我们只开发了 DP3，比谷歌的内部消息晚了一个月。

### 您最终可以微调通知访问

通知监听器服务可以读取和拦截*你设备上发布的所有*通知，但在 Android 12 中似乎不会这样。[正如我们在](https://www.xda-developers.com/android-12-beta-features-leak/#android12leakenhancednotifpermission)之前解释的，谷歌正在为通知访问进行“增强设置”，允许你微调通知监听器服务对你的通知的访问级别。这是一个整洁的隐私功能，我希望谷歌很快会谈论更多。

### 杂项变更

为了保持这篇文章的长度，下面是我们在 Android 12 开发者预览版 3 中发现的一些较小的面向用户的变化。

*   Pixel Launcher 的上下文菜单中的项目现在是分开的
*   辅助功能菜单现在可以通过一个浮动按钮打开(取消了双指向下滑动手势)
*   新的 bouncier 通知下拉动画[video width = " 320 " height = " 656 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/04/20-Bouncy-Notification-Pull-down . MP4 "]
*   “降低亮度”现在被称为“超暗”
*   WiFi、蓝牙和旋转等更多快速设置磁贴都有开/关标签
*   2.4GHz WiFi 热点切换现在称为“最大化兼容性”
*   “添加链接”按钮，手动添加应用程序可以打开的支持链接
*   “NFC 要求设备解锁”设置，因此只有在手机解锁时才能进行非接触式支付
*   “帐户”已更改为“密码和帐户”，而“自动填充服务”已从“系统>语言和输入”转移到此处

* * *

这就是我们到目前为止从挖掘 Android 12 开发者预览版 3 中发现的所有面向用户的功能。如果我发现更多细节，我会在这个 Twitter 帖子中分享它们，或者在门户网站上写一篇新文章。