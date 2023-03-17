# Android 12 可能会使用机器学习来修复背部手势问题

> 原文：<https://www.xda-developers.com/android-12-machine-learning-improve-back-gesture-problem/>

谷歌前几天发布了 Android 12 的第一个开发者预览版[，我们一直在挖掘代码，寻找所有新的东西。我们发现的最令人兴奋的变化之一是对 Android 检测向后滑动手势的方式进行了彻底改革。如果实现，Android 12 将使用机器学习模型来*预测*用户何时打算使用背部手势。](https://www.xda-developers.com/android-12/)

随着 Android 10 的推出，谷歌[推出了其全屏手势导航系统](https://www.xda-developers.com/everything-new-android-q-beta-3/)。Android 的手势导航系统在屏幕底部放置了一个药丸，你可以与之互动，在应用程序之间切换，打开最近的应用程序界面，或进入主屏幕。与此同时，后退按钮被一个向内滑动的手势取代，可以从屏幕的左侧或右侧触发。关于 Android 的背部手势的问题[已经说了很多，但值得称赞的是，他们](https://www.xda-developers.com/google-android-q-gesture-mess/)[已经使整个生态系统的体验保持一致](https://www.xda-developers.com/google-gesture-navigation-android-10/)，并且[为开发者提供 API](https://developer.android.com/training/gestures/gesturenav#conflicting-gestures)以确保与手势的兼容性。虽然许多应用程序已经不再使用[导航抽屉](https://developer.android.com/guide/navigation/navigation-ui)，但仍有许多应用程序的后退手势可能会与应用内 UI 冲突。为了解决这个问题，谷歌正在测试一种新的基于机器学习的方法，用于 Android 12 中的背部手势检测。

Android 的 back 手势目前的工作原理如下。一个看不见的触发区域几乎一直存在于屏幕的两边。根据用户定义的背面灵敏度设置，该触发区域从屏幕两侧延伸 18dp-40dp 的宽度。用户只需将手指放在插图中的任意位置，然后将手指向内移动一个最小距离，就可以触发后退手势。谷歌在设计背部手势插图时使用了手机屏幕热图，[他们选定了用户认为符合人体工程学和单手友好的](https://android-developers.googleblog.com/2019/08/gesture-navigation-backstory.html)识别区域。

Android 10+中的手势导航。来源:谷歌。

正如谷歌自己承认的那样，这种方法的问题是，一些用户仍然需要滑动才能打开导航抽屉，这与后退手势相冲突。每个应用程序的设计都不一样，但背部手势触发区域仍然是一样的。因此，这种一刀切的背部手势方法并不能很好地适应一些应用程序的设计，这就是为什么谷歌正在尝试用机器学习来取代当前的模型。

在调查谷歌对 Android 12 中双击后退手势所做的改变时，XDA 认识到开发者 [Quinny899](https://forum.xda-developers.com/m/quinny899.3563640/) 发现了一种新的 TensorFlow Lite 模型和名为“back gesture”的 vocab 文件的存在后者包含 43，000 个包名，既有流行的，也有不知名的安卓应用，包括 2 个 Quinny899 自己的应用。我们相信这个列表包含了谷歌训练其机器学习模型所针对的应用程序——ie。他们逐个应用程序地确定了背部手势最常见的起点和终点。深入挖掘，我们发现在 Android 12 的 SystemUI 中更新的 EdgeBackGestureHandler 类中引用了机器学习模型。如果启用了功能标志，那么 Android 12 似乎将使用 ML 模型来预测用户是否打算执行后退手势，或者他们是否只是想在应用程序中导航。馈送到 ML 模型进行推理的数据包括手势的起点和终点、应用程序是否在列表中，以及以像素为单位的显示宽度。或者，如果功能标志被禁用，那么 Android 12 简单地恢复到标准的背扫检测方法(即 insets)。

目前，Android 12 开发者预览版 1 中默认禁用基于 ML 的背部手势预测。如果这种方式最终并不优于现有的嵌入式模式，谷歌可能会放弃这种方式。然而，在几个月后谷歌发布 Android 12 测试版之前，我们无法确定，因为那时谷歌通常会透露其对 Android 的更大变化。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*