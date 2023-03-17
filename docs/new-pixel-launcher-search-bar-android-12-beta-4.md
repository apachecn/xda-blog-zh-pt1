# Android 12 Beta 4 首次展示了 Pixel Launcher 更快的搜索栏

> 原文：<https://www.xda-developers.com/new-pixel-launcher-search-bar-android-12-beta-4/>

随着昨天[第四个测试版](https://www.xda-developers.com/android-12-beta-4/)的发布，Android 12 达到了平台稳定性。Android 12 Beta 4 代表着一个重要的里程碑，因为我们离公开发布越来越近了。虽然最新的测试版没有带来任何新功能或值得注意的面向用户的变化，但它确实让我们首次看到了已经开发了一段时间的 Pixel Launcher 的更快的搜索栏。

我们首先在 Android 12 开发者预览版 2 上看到了 Pixel Launcher 的新搜索栏，我们终于让它在 Android 12 Beta 4 上工作了。但是，您需要 root 访问权限才能启用它。这个新的搜索栏取代了 Pixel Launcher 的应用抽屉中现有的谷歌应用支持的搜索小工具。不过，主屏幕上的搜索栏仍然使用谷歌应用程序的搜索工具。

正如你在下面的截图中看到的，新的搜索栏可以让你快速找到应用程序、快捷方式、小工具、设置、联系人、对话、提示等等。

您可以选择弹出什么样的结果，也可以切换是否希望键盘在搜索栏显示时自动打开。旧的搜索栏只是简单地打开了谷歌应用程序，一些人抱怨它又慢又笨重。

新的搜索栏让你可以直接从应用抽屉中直接跳到应用的特定部分。例如，如果你输入“相机”，搜索栏会显示“拍摄视频”、“自拍”、打开相机应用程序、录制视频、跳转到画廊等选项。

这个新的解决方案非常快速和有用。查看下面的演示视频，看看它的实际效果。

Pixel Launcher 的新搜索栏利用了名为 AppSearch 的新 API，该 API 与 [Android 12 Beta 3](https://www.xda-developers.com/android-12-beta-3-changes/) 一起发布。 [AppSearch](https://android-developers.googleblog.com/2021/06/sophisticated-search-with-appsearch-in-jetpack.html) 是一个完全离线的设备上搜索库，开发者可以将其集成到他们的应用程序中，以提供功能丰富的全文搜索功能。

我们设法让新的搜索在 Pixel Launcher 中工作，这要归功于 Android 系统智能应用程序中新添加的服务，名为 *AiAiSearchUiService* 。该服务被设置为 Pixel 手机上的系统默认搜索 UI 服务，由框架配置值 config_defaultSearchUiService 定义。这项服务在之前版本的 Android 系统智能/设备个性化服务应用中不可用，这就是为什么这项功能在之前的 Android 12 版本中不起作用。