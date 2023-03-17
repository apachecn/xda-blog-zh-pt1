# 这是我们第一次看到 Android 12 基于壁纸的主题系统

> 原文：<https://www.xda-developers.com/android-12-wallpaper-theming-system-leak/>

在本周早些时候发布 Android 12 开发者预览版之前，我们了解到谷歌正在开发一个[新的主题系统](https://www.xda-developers.com/android-12-theming-system/)，它可以对支持的第三方应用重新着色。这个增强的主题系统采用了以前版本的 Android 中引入的 RRO 和 OMS API 的基础，并将它们与 Android 的调色板和壁纸颜色 API 相结合，以便创建与当前壁纸匹配的自定义主题。虽然这一功能在公开的开发者预览版中并不工作，但以其为 Pixel 设备制作 ProtonAOSP ROM 和 ProtonKernel 而闻名的开发者 [kdrag0n](https://forum.xda-developers.com/m/kdrag0n.7291478/) 设法让它工作，让我们首次看到了 Android 12 新的基于壁纸的主题化系统。

这是开发者分享的一个相册，展示了设置壁纸并让 Android 12 为快速设置磁贴选择通知背景色和强调色的感觉:

Android 12 中壁纸及其对应主题的图库。演职员表:[kdrag0n](https://twitter.com/kdrag0n)

这是另一个相册，展示了一个主题如何重新着色部分设置(启用了[隐藏的“Silky Home”标志](https://www.xda-developers.com/android-12-better-one-handed-use/)):

*演职员表:[kdrag0n](https://twitter.com/kdrag0n)*

最后，这里有一组图片展示了 Android 12 的[新开发的锁屏和通知 UI 启用时的主题化系统](https://www.xda-developers.com/android-12-new-lockscreen-notifications-design-leak/):

*演职员表:[kdrag0n](https://twitter.com/kdrag0n)*

虽然我们自己没有成功启用“monet ”,但在深入研究 Android 12 的 SystemUI 后，我们基本上理解了它是如何工作的。在与开发者 kdrag0n 交谈后，他透露了一些他是如何让它工作的。他是这样说的:“我在设置了一个系统属性后启用了该功能。但是，它没有影响，因为 DP1 不包含任何系统调色板。它的工作原理是基于颜色相似性动态应用 RRO 覆盖，所以我对 SystemUI 进行了逆向工程，以找出应该如何创建覆盖。之后，我写了一个脚本，根据谷歌官方的材质设计调色板生成叠加图。调色板一装好，莫奈就开始工作了。”

上周，我们[收到了 Android 12](https://www.xda-developers.com/android-12-first-look-screenshots/) 的设计模型，展示了新的通知面板 UI。有趣的是，通知面板的背景是浅米色，我们认为这是米色墙纸的结果。我们认为，谷歌是在展示 Android 的新主题化系统，它展示了根据用户选择的壁纸的突出颜色来改变背景和强调颜色的感觉。本周早些时候，我们透露谷歌正在开发这种新的基于壁纸的主题系统[，代号为“莫奈”](https://www.xda-developers.com/android-12-ui-changes-material-next/)，昨晚晚些时候，我们发布了 Android 12 的[开发中锁屏和通知 UI](https://www.xda-developers.com/android-12-new-lockscreen-notifications-design-leak/) 的第一张图片，部分匹配泄露的设计模型。通过第一次看“莫奈”，我们现在对 Android 12 的最终设计有了更清晰的了解，包括从[到单手可达性](https://www.xda-developers.com/android-12-better-one-handed-use/)的变化。

如何看待 Android 12 新的主题化系统和 UI？