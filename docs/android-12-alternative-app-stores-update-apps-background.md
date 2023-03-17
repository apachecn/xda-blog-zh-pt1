# Android 12 将最终让替代应用商店自行更新应用

> 原文：<https://www.xda-developers.com/android-12-alternative-app-stores-update-apps-background/>

# Android 12 将最终让替代应用商店在不打扰用户的情况下更新应用

谷歌兑现了改善安卓第三方应用商店的承诺，允许它们在安卓 12 后台安装应用。

早在去年九月下旬，谷歌[宣布](https://www.xda-developers.com/google-play-store-in-app-billing-clarity-android-12-third-party-app-stores/)将“对 [Android 12](https://www.xda-developers.com/android-12/) 做出改变”...为了让人们更容易在他们的设备上使用其他应用商店，同时小心不要损害 Android 已经到位的安全措施”，以回应来自 Epic Games 和政府监管机构的[越来越大的压力](https://www.xda-developers.com/fortnite-circumvents-google-play-fees-direct-payment-option/)。然而，谷歌没有具体说明*他们将对 Android 做出什么样的改变，他们也没有在[谷歌 I/O 2021](https://www.xda-developers.com/google-io-2021-recap/) 上分享任何关于这一改变的具体信息。然而，在谷歌发布 Android 12 的官方博客文章中，该公司证实其“正在兑现承诺，让第三方应用商店在 Android 12 上更容易使用。”多亏了开发人员的文档，我们终于对正在进行的更改有了一个概念。*

谷歌已经更新了 Android 的 PackageInstaller。SessionParams 类带有一个名为 [setRequireUserAction](https://developer.android.com/reference/android/content/pm/PackageInstaller.SessionParams#setRequireUserAction(boolean)) 的新方法。此方法指示在允许应用程序安装之前是否需要用户操作。对于任何拥有 [REQUEST_INSTALL_PACKAGES](https://developer.android.com/reference/android/Manifest.permission#REQUEST_INSTALL_PACKAGES) 权限的应用程序，它默认为 true，这是任何应用程序在启动安装会话以从 Google Play 或设备上任何预装的应用程序商店下载应用程序之前所必需的。

但是，如果满足以下所有**条件**，则应用安装/更新不需要用户操作*:*

*   安装程序选择新的行为。
*   正在安装的应用程序针对 API 级别 29 (Android 10)或更高。(谷歌指出，目标 API 级别要求将在未来的 Android 版本中提高，这一政策符合关于 API 目标要求的 [Google Play 政策](https://www.xda-developers.com/play-store-updated-requirements-api-level-64-bit/)。)
*   安装程序要么正在更新自身，要么正在安装它首次安装的应用程序的更新。
*   安装程序声明了`[UPDATE_PACKAGES_WITHOUT_USER_ACTION](https://developer.android.com/reference/android/Manifest.permission#UPDATE_PACKAGES_WITHOUT_USER_ACTION)`权限。

因此，当 app store 尝试启动安装会话并使用这个新 API 时，应该可以在用户不必手动接受更新的情况下进行更新。这将使批量更新应用程序更快，并带来更符合谷歌 Play 商店的体验。