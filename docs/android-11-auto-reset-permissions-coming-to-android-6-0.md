# Android 11 的自动重置权限功能将在旧版本的操作系统中实现

> 原文：<https://www.xda-developers.com/android-11-auto-reset-permissions-coming-to-android-6-0/>

在 Android 11 中，谷歌[引入了自动撤销权限](https://www.xda-developers.com/android-11-features-developers-new-apis/)，禁止未使用的应用访问用户授予的敏感权限。虽然这一隐私功能目前仍为 Android 11 及以上版本的设备所独有，但它很快就会渗透到旧版本的 Android 中——一直追溯到 Android 6.0。

今天，谷歌宣布将把 [Android 11 的权限自动重置功能](https://developer.android.com/about/versions/11/privacy/permissions)带到所有运行 Android 6.0 及以上版本的设备上。该功能将于今年晚些时候开始在安装了 Google Play 服务的设备上推广。谷歌表示，针对 Android 11 (API 级别 30)或更高版本的应用程序将默认启用该功能。对于 API 级别为 23 到 29 的应用程序，用户必须从设置中手动启用它。

首先，权限自动重置功能会自动撤销授予用户几个月没有访问的应用程序的敏感权限。例如，如果您允许某个应用程序访问您的位置，但由于某种原因，您很长时间没有打开该应用程序，则该功能会自动撤销该应用程序的位置权限，当您打开该应用程序时，它必须再次请求位置权限。

权限自动重置功能不适用于设备管理员应用；同样，由企业策略固定的权限也不会被撤销。该功能还兼容 [Android 12](https://www.xda-developers.com/android-12/) 中的 [app 休眠](https://www.xda-developers.com/app-hibernation-android-12-beta/)。如果需要，应用程序开发人员还可以要求用户禁用自动重置权限功能。如果你的应用目标是 API 级别 30 或更高，你希望要求用户禁用权限自动重置，那么你需要使用新的跨平台 API，它是 [Jetpack 核心](https://developer.android.com/jetpack/androidx/releases/core)库— `androidx.core.content.PackageManagerCompat.getUnusedAppRestrictionsStatus()`和`androidx.core.content.IntentCompat.createManageUnusedAppRestrictionsIntent()`的一部分。这样做有助于主要在后台运行的应用程序，如智能手表的配套应用程序。

许可自动撤销功能进入旧的 Android 手机表面上看起来可能无关紧要，但考虑到许多旧手机的软件支持很久以前就停止了，因此被恶意应用程序利用的风险更高，很高兴看到谷歌将这一隐私功能扩展到旧的 Android 版本。

权限自动重置功能将从 2021 年 12 月开始通过安装了 Google Play 服务的 Android 10 设备逐步推广到 Android 6.0。谷歌表示，该功能将在 2022 年 Q1 奥运会前覆盖所有符合条件的设备。与此同时，跨平台自动重置 API 今天与 Jetpack Core 1.7.0 一起推出测试版，但将在 2021 年 10 月作为稳定 API 推出。