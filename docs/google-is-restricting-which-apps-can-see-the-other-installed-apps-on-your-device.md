# 谷歌正在限制哪些应用程序可以看到你的设备上安装的其他应用程序

> 原文：<https://www.xda-developers.com/google-is-restricting-which-apps-can-see-the-other-installed-apps-on-your-device/>

谷歌正在对开发者计划政策进行一些新的修改，这将使应用程序更难看到你的 Android 设备上安装了哪些其他应用程序。谷歌表示，它将用户设备上安装的应用程序的完整列表视为个人和敏感信息，因此将限制哪些应用程序可以访问这些信息。具体来说，谷歌将限制哪些应用程序可以请求 QUERY_ALL_PACKAGES 权限，目前针对 API 级别 30 (Android 11)及以上的应用程序需要该权限，才能查询运行 Android 11 或更高版本的用户设备上已安装应用程序的列表。

接下来，只有当应用程序的核心功能依赖于查询已安装的应用程序时，才允许使用 [QUERY_ALL_PACKAGES 权限](https://support.google.com/googleplay/android-developer/answer/10158779#zippy=%2Cinvalid-uses%2Cpermitted-uses-of-the-query-all-packages-permission)。开发人员必须“充分证明为什么一种侵入性较低的应用可见性方法不能充分支持你的应用的符合政策的面向用户的核心功能。”

Google 将 QUERY_ALL_PACKAGES 权限的允许使用概述如下:

> 许可使用涉及必须发现设备上安装的任何和所有应用的应用，出于认知或互操作性目的，可能具有许可资格。许可用途包括:设备搜索、防病毒应用、文件管理器和浏览器。

如果一个应用程序不符合上述要求，开发人员必须从应用程序的清单中删除权限，以符合播放政策。即使应用程序满足使用 QUERY_ALL_PACKAGES 权限的要求，开发人员仍需要在 Play 控制台中签署声明表单。谷歌警告称，未能提交声明表或不符合政策要求可能会导致你的应用程序被从谷歌 Play 商店移除。这一新变化将于 2021 年 5 月 5 日开始生效。值得注意的是，从 2021 年 11 月开始，所有提交到 Google Play 的新应用和应用更新都将被要求针对 Android 11 或更高版本，加强了这一新政策的执行力度。

这是一个受欢迎的变化，将使应用程序更难窥探你在设备上使用的应用程序。了解您的设备上安装了哪些应用程序可能会被用作定向广告的一部分或用于恶意目的。

值得注意的是，谷歌已经要求请求短信或通话记录权限的[应用签署一份声明表](https://www.xda-developers.com/google-play-developer-policy-call-log-sms/)，然后才能在 Google Play 上发布。对应用程序包可见性的限制只是谷歌限制权限访问以保护用户隐私的下一步。

*感谢 XDA 公认的开发者 [M66B](https://forum.xda-developers.com/m/m66b.2799345/) 的提示！*