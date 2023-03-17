# Android 版 Chrome 可以让你在锁屏后锁定匿名标签

> 原文：<https://www.xda-developers.com/chrome-for-android-biometric-authentication-for-incognito-tabs/>

上个月，谷歌在 Android 和桌面平台的稳定渠道上推出了 Chrome 92。新版本带来了改进的网站安全控制，支持新的 Chrome 操作，更好的钓鱼检测和网站隔离，等等。与往常一样，最新版本也适用于 iOS，增加了支持整页截图、改进标签切换器以及在发现、设置、历史和书签页面上进行小的 UI 调整等功能。除了这些改进，Chrome 92 for iOS 还增加了一个漂亮的功能:可以在锁屏后锁定匿名标签。目前，这项功能仍然是 iOS 独有的，但看起来谷歌可能很快就会将其引入 Android。

Android 版 Chrome 正准备为匿名标签添加生物认证功能。一个新的提交被[合并](https://chromium-review.googlesource.com/c/chromium/src/+/3081943)到 Chromium Gerrit 中，为一个叫做“匿名重新认证”的特性添加了一个标志。标志描述为:*“启用后，设置>隐私和安全中会出现一项设置，允许重新验证您现有的匿名选项卡。”*

启用后，当有人试图访问任何已打开的隐名标签时，该功能可能会使用[生物计量提示 API](https://developer.android.com/reference/androidx/biometric/BiometricPrompt) 来显示系统提供的认证提示。

该功能的标志已经添加到 Canary 分支中，您可以通过在地址栏中粘贴以下 URL 来访问它:*chrome://flags # incognito-re authentication-for-Android。*然而，该功能似乎仍在开发中，因为启用标志还没有出现在设置中。一旦该功能上线，将可以在*设置>隐私和安全*下访问。

如上所述，Chrome 还没有锁定匿名标签的功能。在推出稳定版之前，它很可能会首先推出 Chrome Canary 分支。如果你想成为第一个尝试它的人，你可以从下面的链接下载 Canary 的最新版本。

* * *

精选图像图标由 [*扁平图标*](https://www.flaticon.com/free-icon/mobile-security_5248740?term=authentication&page=1&position=95&page=1&position=95&related_id=5248740&origin=tag) 组成