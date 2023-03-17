# Android 12 可能会在谷歌 Pixel 手机上添加自定义锁屏时钟

> 原文：<https://www.xda-developers.com/android-12-custom-lock-screen-clock-google-pixel/>

虽然 AOSP 多年来一直有一个强大的主题系统，但直到 Android 10 发布后，谷歌才最终利用它在 Pixel 手机上进行主题化。在 Android 10 中，谷歌推出了可从 Pixel Launcher 中的“Styles & wallpapers”快捷方式访问的 [Pixel 主题应用](https://www.xda-developers.com/google-pixel-themes-customize-android-10/)。除了定制图标形状、强调颜色和字体，Pixel Themes 应用程序还可以让你改变 Pixel Launcher 的网格大小。然而，我们多年前就知道谷歌也在[致力于增加新的锁屏时钟](https://www.xda-developers.com/android-q-lock-screen-clock-customization/)。基于新的证据，我们认为谷歌很可能最终会在 Android 12 中引入新的锁屏时钟[作为像素专属功能。](https://www.xda-developers.com/android-12/)

回到 2019 年，我们了解到谷歌正在研究 3 种不同的锁屏时钟预设，包括文本时钟、气泡时钟和拉伸模拟时钟。谷歌从稳定版中移除了这些锁屏时钟，直到今天，它们也不再出现在 SystemUI 应用中。

在被移除之前，Android 10 有 3 个不同的隐藏时钟选项。

然而，在第一个 Android 12 开发者预览版发布之前，[我们透露了](https://www.xda-developers.com/android-12-ui-changes-material-next/)谷歌一直在幕后改进这一功能。在 DP1 退出后，我们也让你先看看[Android 12 中锁屏的新 UI](https://www.xda-developers.com/android-12-new-lockscreen-notifications-design-leak/) 可能是什么。我们推测，新的布局和扩大的时钟是为了方便将默认的数字时钟替换为其他时钟选项。

*Android 12 正在开发的新锁屏界面*

经过一番挖掘，我们得知谷歌在 Android 12 中更新了 WallpaperPicker 应用程序，添加了与自定义锁屏时钟相关的新代码。通过检查代码，我们了解到，如果没有安装软件包名称与“clocks_stub_package”值匹配的应用程序，Pixel Themes 应用程序不会在底部显示“clock”选项卡。“clocks_stub_package”的值目前与“com.google.pixelcustomclocks”匹配，这表明 google 正在开发一个包含自定义锁屏时钟的单独的包。鉴于“com.google”命名空间和软件包名称中“pixel”的存在，这款应用可能会专门预装在运行 Android 12 的 Pixel 手机上。不幸的是，这个包目前没有出现在 Android 12 开发者预览版 1 中，所以我们不知道哪些锁屏时钟选项将可用。

我们将密切关注该应用程序在未来开发者预览版和测试版中的出现，但不能保证它会在稳定版发布前添加。无论如何，我们终于知道这个功能还没有被放弃，可能会出现在 Android 12 的许多其他 UI [变化中。如果你没有 Pixel 手机，那么你会很高兴知道有这个功能的开源版本](https://www.xda-developers.com/android-12/)，但是你的 OEM 厂商可能必须开发他们自己的钟面。