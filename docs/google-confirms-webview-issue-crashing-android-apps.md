# [更新:已修复更新]谷歌证实 WebView 的一个问题导致许多 Android 应用程序崩溃

> 原文：<https://www.xda-developers.com/google-confirms-webview-issue-crashing-android-apps/>

在过去的几个小时里，许多 Android 应用突然开始崩溃，当用户试图打开它们时，应用会抛出可怕的“继续关闭”警告信息。Twitter 和 Reddit 论坛[充斥着应用崩溃的报告](https://www.reddit.com/r/GMail/comments/may197/gmail_app_crashing/)。DownDetector 还显示 Gmail 和亚马逊的宕机报告大幅增加。桌面 Gmail Web 界面和 Google Workspace 服务不受影响。

许多用户很快发现，这个问题源于 Android WebView 最近的一次更新。Android WebView 是一个系统组件，允许开发人员在其应用程序中显示网页。它预装在每个现代 Android 设备上，并通过 Play Store 定期更新最新的安全增强和修复。似乎是一个错误的更新破坏了 WebView 组件。简单地卸载 Android WebView 更新就可以解决崩溃问题(通过[*【Engadget】*](https://www.engadget.com/android-gmail-stop-running-webview-234125352.html))，正如它对绝大多数受影响用户所做的那样:

如果您受到该问题的影响，请打开 Play Store，搜索 Android WebView，然后卸载更新。或者，你也可以从你的设备设置中进入“应用”或“应用”，在系统应用中找到 Android WebView 应用，并卸载其最新更新。

谷歌发言人证实，该公司已意识到这一问题，并正在努力解决:

> 我们意识到 WebView 的一个问题导致 Android 上的一些应用程序崩溃。我们目前正在全面验证范围，修复工作正在进行中。

根据[谷歌工作区状态面板](https://www.google.com/appsstatus#hl=en&v=issue&sid=1&iid=aa75515d184a2423be444d676b7ebf45)上发布的最新更新，谷歌仍在调查这个问题。

在撰写本文时，谷歌还没有分享任何关于修复的更新。Android 用户有责任通过卸载最近的 Android WebView 更新来解决这个问题。

* * *

## 更新:新的 WebView 更新修复了崩溃问题

谷歌分享了关于应用崩溃问题的更新:

我们已经解决了 WebView 导致 Android 上的某些应用程序对某些用户崩溃的问题。通过 Google Play 更新 Android 系统 WebView 和 Google Chrome 现在应该可以解决这个问题。

建议用户更新到最新的 [Android 系统 WebView](https://play.google.com/store/apps/details?id=com.google.android.webview) 和[谷歌 Chrome](https://play.google.com/store/apps/details?id=com.android.chrome) 版本。