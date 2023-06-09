# Chrome 准备让你在 Android 12 上截图

> 原文：<https://www.xda-developers.com/google-chrome-full-page-screenshots-android-12/>

谷歌正在 [Android 12](https://www.xda-developers.com/android-12/) 中添加许多被高度要求的功能，其中之一就是滚动截图。在 Android 12 Beta 3 中首次引入了[，滚动截图功能可以让你捕捉整个页面的截图，这意味着你不再需要手动捕捉然后将多个截图拼接在一起。谷歌实现这一功能的方式与大多数原始设备制造商不同，因此，它目前并不适用于所有应用程序。谷歌 Chrome 是最著名的不能滚动截图的应用之一，但这种情况很快就会改变。](https://www.xda-developers.com/android-12-beta-3-changes/#:~:text=and%20scrollable%20screenshots.-,Scrolling%20screenshots,-With%C2%A0scrolling%20screenshots)

当谷歌设计滚动截图功能时，他们不想遵循许多原始设备制造商采取的相同方法。大多数 OEM 实现都包括自动向下滚动，同时捕捉单个屏幕截图，以便在到达页面末尾时进行组合，但这可能会导致图像拼接不佳。相反，Android 12 的版本直接作用于[视图](https://developer.android.com/reference/android/view/View)，这是 Android 应用程序中用户界面组件的基本构建模块。这使得 Android 12 的方法更快、更可靠，但通用性也较差。谷歌表示，对于大多数使用基于标准视图的用户界面的应用程序来说，滚动屏幕截图是现成的，但网页并不包含在这种视图中。对于那些应用程序不使用基于视图的用户界面或使用高度定制的用户界面的开发人员，谷歌建议实现 Android 12 的新 [ScrollCapture API](https://developer.android.com/reference/android/view/ScrollCaptureCallback) ，以提供关于要捕捉的视图的滚动捕捉系统信息。

这正是 Chrome 的开发者计划在 Android 12 上添加对捕获整页截图的支持的方式。在提交给 Chromium Gerrit 的一份承诺中，Chrome 工程师准备增加对 Android 12 的 ScrollCapture API 的支持。

该代码实现了 ScrollCaptureManager 类，以提供活动选项卡的渲染快照，用于长屏幕截图。Chrome 提供使用[画图预览](https://chromium.googlesource.com/chromium/src/+/refs/heads/main/components/paint_preview)的标签快照，这本质上是代表网页视觉内容的快照。绘画预览是 [Chrome 的冻干标签功能](https://www.xda-developers.com/google-chrome-89-freeze-dried-tabs/)的关键，该功能显示标签的交互式预览，而实际标签在后台加载。

然而，你不可能获得每个网页的全页截图。该功能目前显然不适用于 [AMP](https://amp.dev/) ，开发者[也认为](https://chromium-review.googlesource.com/c/chromium/src/+/3089805/comment/348bf92a_e52244ab/)不适用于具有多个可滚动区域的页面。然而，这些问题可能会在谷歌 Chrome 上线之前得到解决。

一旦提交被合并，滚动捕获支持将被锁定在“滚动捕获”特征标志之后。即便如此，该特性最初也只对运行 Canary 构建的用户可用。然后，大约需要[4 周](https://www.xda-developers.com/chrome-updates-will-now-be-released-every-4-weeks/)功能标志才能在稳定渠道中对用户可用，甚至可能需要更长时间来默认启用该标志。谷歌[此前表示](https://www.xda-developers.com/android-12-beta-3-changes/)他们正在努力使他们的滚动屏幕截图实现在 WebViews 中工作，这可能需要更长的等待，因为 [Android 系统 WebView](https://play.google.com/store/apps/details?id=com.google.android.webview) 应用的更新[独立于 Chrome](https://www.xda-developers.com/google-chrome-no-longer-webview-provider-android-10/) 。

谷歌 Chrome 增加支持的另一个 Android 12 功能是动态主题化。该功能目前正在运行，但是被隐藏在一个功能标志后面，所以我们不用等很久就可以得到它。