# Android 12 开发者预览版 2.1 已经发布，修复了 WebView 崩溃问题

> 原文：<https://www.xda-developers.com/android-12-developer-preview-2-1/>

# Android 12 开发者预览版 2.1 已经发布，修复了 WebView 崩溃问题

谷歌发布了支持 Pixel 手机的 Android 12 开发者预览版 2.1，修复了令人讨厌的 WebView 崩溃问题。

谷歌在两周前发布了 Android 12 的[第二次开发者预览版，新增了权限、视觉变化和重要的 bug 修复。然而，它引入了一个新的错误，导致一些应用程序不断崩溃，现在已经修复。谷歌今天早些时候发布了 Android 12 开发者预览版 2.1，声称修复了](https://www.xda-developers.com/android-12-developer-preview-2/) [WebView 崩溃问题](https://www.xda-developers.com/google-confirms-webview-issue-crashing-android-apps/)。

有数不清的 [报道](https://www.reddit.com/r/android_beta/comments/mchq7u/google_app_issues/)谷歌、Gmail 和其他依赖 WebView(在原生 Android 应用中显示网页内容的系统组件)的应用无法在 Android 12 开发者预览版上正常工作，尽管[一些人声称](https://www.reddit.com/r/android_beta/comments/md2uqy/gmail_and_google_app_force_closing_constantly/gs72pez/)最近通过 Play Store 对 WebView 的更新修复了漏洞。

Android 12 开发者预览版 2.1 更新还修复了其他几个经常被报道的问题，包括背部手势不起作用，时钟小工具损坏，以及通过 Google Pay 进行 NFC 支付的问题。下面是来自谷歌的完整[发布说明](https://developer.android.com/about/versions/12/release-notes.html)。

### Android 12 开发者预览版 2.1 发行说明

### 开发者报告的问题

*   修正了在某些情况下返回手势不起作用的问题。([问题编号 180932529](https://issuetracker.google.com/issues/180932529) )
*   修复了用户通过 Google Pay 使用非接触式支付时遇到的问题。([问题编号 180725322](https://issuetracker.google.com/issues/180725322)
*   修复了在某些应用程序顶部渲染时导致通知抽屉中的文本难以阅读的问题。([问题#180647015](https://issuetracker.google.com/issues/180647015)
*   修复了导致`java.lang.Deprecated`被标记为已弃用的问题。([第 180705308 期](https://issuetracker.google.com/issues/180705308)
*   修复了一个问题，阻止了针对 Android 12 的应用程序使用版本 2.7.0-alpha01 的[工作管理器](https://developer.android.com/topic/libraries/architecture/workmanager)。该修复包含在版本 [2.7.0-alpha02](https://developer.android.com/jetpack/androidx/releases/work#2.7.0-alpha02) 中。([第 180884673 期](https://issuetracker.google.com/issues/180884673))

### 其他已解决的问题

*   修复了 WebView 的一个问题，该问题阻止开发者在 Android 12 上启用或测试有计划的同站点更改。
*   修复了从生产版本升级到 Android 12 而不擦除数据可能会丢失以前配对的蓝牙设备的 HID 控制的问题。
*   修复了从相机应用程序共享的视频可能使用错误的编码发送的问题。
*   修复了一个问题，该问题可能会导致主屏幕上的时钟小工具的文本在某些设备上被切断。
*   修正了主屏幕上的空白页面有时不会被删除的问题。
*   修正了有时会阻止用户访问通知阴影的问题。

如果你想尝试新的 Android 12 开发者预览 2.1 版本，而你还没有使用 Android 12，你需要从 Android 开发者网站的[手动下载并刷新最新版本。那些已经在开发者预览版 1 或 2 上的人应该通过空中下载(OTA)获得新版本。兼容设备的列表保持不变，您需要一个 Pixel 3/3 XL、Pixel 3a/3a XL、Pixel 4/4 XL、Pixel 4a/4a 5G 或 Pixel 5。](https://developer.android.com/about/versions/12/download.html)