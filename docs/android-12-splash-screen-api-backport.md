# 新的 Jetpack 库支持 Android 12 的闪屏 API

> 原文：<https://www.xda-developers.com/android-12-splash-screen-api-backport/>

# 新的 Jetpack 库为 Android 12 的闪屏 API 增加了向后兼容性

已经发布了一个新的 Jetpack 库，它将 Android 12 中新的闪屏 API 一路反向移植到 API level 23/Android 6.0。

随着 [Android 12](https://www.xda-developers.com/android-12/) 的[第三次开发者预览版](https://www.xda-developers.com/android-12-dp3-features/#android12dp3splashscreens)的发布，谷歌为应用添加了新的平台 API，以定制他们应用的闪屏。虽然 Android 12 [会自动生成一个闪屏](https://www.xda-developers.com/android-12-dp3-features/#android12dp3splashscreens)，在浅色或深色的背景上显示应用程序的图标，但开发者可以用自定义图标或动画来定制闪屏，以保持他们独特的品牌。例如，Android 12 上的 Google Drive 应用程序有一个带有动画图标的自定义闪屏，正如 Reddit 上的[用户上周发现的](https://www.reddit.com/r/Android/comments/o930va/animated_splash_screen_for_google_drive/)。

为了让开发者更容易制作自定义闪屏，Google 今天发布了[Core splash screen 1 . 0 . 0 版本](https://developer.android.com/jetpack/androidx/releases/core#core-splashscreen-1.0.0-alpha01)。这是一个新的 [Jetpack](https://www.xda-developers.com/android-jetpack-components-kotlin-android-studio-3-2/) 支持库，允许开发人员向他们的应用程序添加闪屏，不仅与 Android 12 中新的[闪屏 API](https://developer.android.com/about/versions/12/features/splash-screen)兼容，还向后兼容到 API 级别 23，或 Android 6.0 棉花糖。

今天发布的 Jetpack 库的另一个值得注意的更新是核心 Google 快捷方式的 1.0.0 版本。这个模块允许使用[ShortcutManagerCompat](https://developer.android.com/reference/androidx/core/content/pm/ShortcutManagerCompat)API 保存的快捷方式也被“捐赠给谷歌”这将“为用户解锁那些快捷方式的附加功能，例如将它们显示为建议或允许谷歌助手通过语音查询来实现它们。”

在谷歌 I/O 2021 上，谷歌宣布了 Android 12 中快捷方式的[新 API，这使得找到应用程序支持的所有助理查询变得更容易。开发人员建立了一个 Android 快捷方式，可以让它们自动出现在助手快捷方式库中，不久，这些](https://www.xda-developers.com/android-12-will-help-google-assistant-find-and-use-app-shortcuts/)[快捷方式将在助手面板的建议芯片中显示](https://www.xda-developers.com/google-assistant-one-tap-shortcuts-third-party-apps/)，或者作为搜索界面的建议。