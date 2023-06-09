# Android 12 的素材 You theming 系统已经被一个开发者重新创建了

> 原文：<https://www.xda-developers.com/android-12-material-you-theming-system-recreated/>

Material You 基于壁纸的主题化系统，代号“monet”，终于在 [Android 12 Beta 2](https://www.xda-developers.com/android-12-beta-2-features/) 上线。主题化系统基于你的壁纸的主要颜色方案创建调色板，并将它们应用于快速设置磁贴、锁屏、设置、弹出窗口和应用程序。然而，在其目前的实现中，它只有[主题部分的系统 UI](https://www.xda-developers.com/android-12-beta-2-features/#android12beta2_dynamictheming) 和[选择系统应用](https://www.xda-developers.com/google-messages-material-you-theming-android-12/)。大多数第三方应用程序不支持这种动态主题，因为谷歌还没有发布关于 Material You 的文档。虽然我们不知道谷歌何时会在 Material You 上发布资源和库，但 ProtonAOSP ROM 的开发者丹尼林(kdrag0n)已经推出了自己的基于“莫奈”的主题引擎。

kdrag0n 的主题引擎的工作方式就像“monet”一样，并向所有运行 Android 12 和一些旧版本 Android 的设备开放像素专属的动态主题。kdrag0n 是第一个让“monet”在早期 Android 12 开发者预览版中工作的开发者。从那以后，他对谷歌的实现进行了逆向工程，甚至向谷歌的 SystemUI 团队成员提供反馈，特别是[詹姆斯·奥利里](https://twitter.com/jpohhhh)(他似乎是谷歌开发“莫奈”团队的一员)。

根据 kdrag0n 的说法，他的实现没有使用任何来自 Google 或 Android 12 的代码或 API，因此他的模型不依赖于运行 Android 12 的设备。kdrag0n 的主题引擎跟随你给目标上色的材质。然后，通过在@bjornornorn 的 Oklab 感知色彩空间中调整色彩和色调，对这些目标进行重新着色。使用 Oklab 空间中的色域交集将生成的颜色色域映射到 sRGB。”用户还可以改变色彩，使其优先于精确的色调。

kdrag0n 的主题引擎在 MIT 许可下是开源的，允许定制 ROM 开发者(甚至 OEM)实现它，如果他们希望这样做的话。事实上，当 Android 12 源代码公布时，开发者自己的 [ProtonAOSP](https://t.co/gVSqB5sv8z?amp=1) ROM 将是首批实现它的之一。如果你是一个定制的 ROM 开发者，你可以挑选[这些提交](https://github.com/kdrag0n/android12-extensions/commits/monet-next)并把它们合并到你的构建中。

开发者还在开发 Jetpack Compose 和 Flutter 库，这将允许甚至为 Android 11 构建的应用程序支持动态颜色。针对旧 Android 版本的应用程序可以[注册一个监听器](https://developer.android.com/reference/android/app/WallpaperManager#addOnColorsChangedListener(android.app.WallpaperManager.OnColorsChangedListener,%20android.os.Handler))在壁纸颜色改变时得到通知——kdrag 0n 的代码更多的是为了基于新的壁纸颜色生成主题。

作为他的模型为针对 Android 11 的应用程序工作的一个例子，这位开发人员与我们分享了一个视频，演示了一个应用程序以 90fps 的速度每帧改变其主题。请注意，该演示只是一个示例，不建议完全按照图中所示重新制作。

这一款对性能和电池有很大影响，尽管开发者的 Pixel 4 可以以 90fps 的速度渲染主题变化，以获得更简单的视图。据开发人员称，Jetpack Compose 尚未针对性能进行太多优化，Flutter 库可能会更好。在任何情况下，他的引擎生成一个主题只需要 0.05 毫秒，但改变每一帧的 UI 主题仍然会对性能造成负担。

* * *

米莎尔·拉赫曼对本文有贡献。