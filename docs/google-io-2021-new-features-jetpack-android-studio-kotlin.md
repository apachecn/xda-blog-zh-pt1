# 谷歌为 Jetpack、Android Studio 和 Kotlin 推出新功能

> 原文：<https://www.xda-developers.com/google-io-2021-new-features-jetpack-android-studio-kotlin/>

我们现在已经进入了谷歌 I/O 2021 开发者大会，因此我们看到了一堆关于谷歌所有开发产品的以开发者为中心的新闻。除了对 [Flutter](https://www.xda-developers.com/flutter-2-2-google-io-2021) 和 [Firebase](http://xda-developers.com/firebase-news-google-io-2021) 的改变，我们还为原生 Android 开发提供了一些新功能，包括关于 Android Jetpack、Android Studio 甚至 Kotlin 的声明。

## Jetpack 复合

Jetpack Compose 是一个基于 Kotlin 的声明式设计框架，适用于 Android、桌面甚至 web(尽管后两者由 JetBrains 而非 Google 管理)。

今天，谷歌宣布了 Jetpack Compose 稳定发布的日期，以及一些正在开发的新功能。Jetpack Compose 1.0 将于 7 月的某个时候发布到 stable。它将带来更多的组件，对大屏幕的更好支持，以及一些更普遍的生活质量变化。

## 安卓工作室

Android 工作室北极狐已经在金丝雀[呆了一段时间了](https://www.xda-developers.com/android-studio-emulator-rollable-phones/)。今天，金丝雀成为测试版，因为谷歌正在向测试版频道发布北极狐的最新版本。

除了更换频道之外，这里没有太多新的东西，但这里有一个金丝雀中发现的一些功能的快速纲要。IDE 具有内置的 Jetpack 合成支持，具有布局预览、代码完成等功能。有一些新的调试工具，包括可访问性扫描器和内存分析器。此外，谷歌已经将 Android Gradle 插件更新到 7.0，版本现在与 Gradle 本身一致。

## 我的锅

Kotlin 今天也获得了一些改进，包括新注释处理器 API 的稳定发布:Kotlin 符号处理。谷歌表示，这种 API 应该比以前的选项快两倍，而且通常更高效。

## 喷气背包

最后，我们对谷歌的支持库套件 Android Jetpack 进行了一些更改。

谷歌已经发布了处于 alpha 状态的 Jetpack Macrobenchmark，以帮助开发者分析应用程序中的启动和动画延迟，并查明相关问题。Kotlin DataStore 是 SharedPreferences 的 Kotlin-first 替代品，现已进入测试阶段。