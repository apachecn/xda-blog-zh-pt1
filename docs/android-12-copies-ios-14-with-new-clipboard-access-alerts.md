# Android 12 复制 iOS 14，新增剪贴板访问提醒

> 原文：<https://www.xda-developers.com/android-12-copies-ios-14-with-new-clipboard-access-alerts/>

谷歌几年来一直在打击 Android 中的剪贴板访问。随着 Android 10 的发布，该公司[阻止后台应用程序读取剪贴板数据](https://www.xda-developers.com/android-q-blocks-background-clipboard-access/)，现在在 Android 12 中，谷歌引入了一个设置，每次应用程序访问你的剪贴板时都会显示一个弹出窗口——即使它在前台。

[我们在 4 月份](https://www.xda-developers.com/android-12-beta-features-leak/#android12leakclipboardprompt)报道了谷歌正在 Android 12 中开发剪贴板访问弹出窗口，可以从系统隐私设置中访问。启用后，该功能会在每次应用程序访问剪贴板中的文本、图像或其他内容时显示一条 toast 消息。谷歌在今天的“Android 新功能”演讲中证实了这一功能，并表示将在 Android 12 Beta 2 中试用。

该功能在大多数情况下可能没有用，因为剪贴板访问已经被限制在前台应用程序，但它将在调查应用程序行为时派上用场。这种效果可能类似于 Android 10 引入的后台位置访问通知，它突出了 Instagram 和其他应用程序秘密获取位置数据的频率。

苹果在 iOS 14 中引入了类似的功能，当应用程序读取你的剪贴板数据时，会显示通知。该功能揭示了 Twitter、Zilow、抖音和其他应用程序[悄悄访问剪贴板](https://www.macrumors.com/2020/06/25/tiktok-clipboard-access-ios-14-caught/)的频率。目前还不清楚谷歌是否会像苹果在 iOS 14 中一样，在 Android 12 中默认启用提醒。