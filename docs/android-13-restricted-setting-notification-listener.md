# Android 13 的限制设置功能将阻止恶意应用访问你的通知

> 原文：<https://www.xda-developers.com/android-13-restricted-setting-notification-listener/>

# Android 13 的限制设置功能将阻止恶意应用访问你的通知

从 app store 之外侧装的应用将无法访问 Android 13 上的通知监听器。请继续阅读，了解更多信息。

谷歌在 Android 13 中引入了一个变化，这将[阻止侧装应用滥用可访问 API](https://www.xda-developers.com/android-13-google-malware-crackdown-accessibility-api/)。受限设置功能将阻止用户为恶意应用程序启用辅助功能服务。识别此类应用程序后，该应用程序的辅助功能设置将变得不可访问，用户将看到一个“受限设置”对话框，说明该设置当前不可用。但这并不是新功能的全部。

根据米沙·拉赫曼的说法，受限设置功能还会阻止用户启用应用程序的通知监听器。不知情的是，Android 的 NotificationListenerService API 允许应用程序代表用户拦截所有通知并与之交互。如果恶意应用程序获得 API 的访问权限，它可以读取所有传入的通知并获得敏感信息的访问权限。Android 13 的限制设置功能防止所有应用程序使用非基于会话的软件包安装程序进行侧装。

由于大多数 app store 使用基于会话的软件包安装程序，因此该限制不适用于从 app store 下载的应用程序。它只会屏蔽用户从应用商店之外下载的应用，比如通过浏览器或消息应用。但是，有一个解决方法可以防止该功能阻止侧载应用程序的访问。

拉赫曼指出，可以*“确认受限设置对话框，然后重新启用对辅助功能设置的访问”*。你可以在[这篇博文](https://blog.esper.io/android-13-sideloading-restriction-harder-malware-abuse-accessibility-apis/)中了解更多关于变通办法的信息。

* * *

特色图片来源:米沙·拉赫曼