# 以下是如何在 Android 版 Snapchat 上启用未发布的黑暗模式

> 原文：<https://www.xda-developers.com/enable-dark-mode-snapchat-android/>

虽然在过去几年中，大多数流行的应用程序都获得了原生的黑暗主题，但仍有相当多的应用程序没有提供这一功能。例如，Snapchat 仍然不支持黑暗模式。但这种情况很快就会改变。这个社交媒体平台最近开始在 iOS 上推出黑暗模式，其 Android 应用程序也将很快获得类似的功能。但是如果你不想等待，你可以在一个有根的 Android 手机上使用一个简单的变通方法来立即在 Snapchat 上获得黑暗模式。

早在 5 月份，Snapchat 就在应用程序设置中推出了一个新的“应用程序外观”部分。该部分包括三个选项——匹配系统、总是亮和总是暗——让你自动将应用程序主题与 iOS 系统主题匹配，默认情况下保持亮模式，或者选择新的暗模式作为默认选项。虽然这一设置并没有在 Android 版本的应用程序上运行，但 XDA 承认开发者 [Quinny899](https://forum.xda-developers.com/m/quinny899.3563640/) 报告称，可以使用首选项管理器应用程序启用开发中的黑暗主题。

***注意:**偏好设置管理器应用需要 root 权限，所以在执行下面提到的步骤之前，请确保你的手机是 root 的。如果你还没有 root 你的手机，你可以查看我们的[详细指南](https://www.xda-developers.com/root/)开始使用。*

以下是如何在 Android 版 Snapchat 中启用开发中的黑暗主题:

1.  从 [Play Store](https://play.google.com/store/apps/details?id=fr.simon.marquis.preferencesmanager) 下载偏好设置管理器应用。
2.  在应用主页选择 Snapchat，打开 APP_START_EXPERIMENT_PREFS.xml 文件。
3.  在文件中，找到“DARK_MODE”标志，将其设置为“ENABLED”，然后就可以开始了。

正如您在所附截图中看到的，该变通办法允许您访问 Snapchat for Android 上的开发中黑暗模式。请注意，黑暗模式仍然是一个正在进行的工作，所以你可能会注意到一些不一致。例如，几个屏幕在黑色背景上有灰色文本，还有几个部分还没有主题化(见下面的截图)。

还值得注意的是，偏好设置管理器应用程序需要 root 访问权限，因此该变通办法仅适用于根设备。你可以按照[这篇文章](https://www.xda-developers.com/root/)中给出的步骤给你的手机 root。如果这看起来太复杂，那么我们建议避开，等待 Snapchat 在 Android 上正式推出新的黑暗模式。由于该功能已经为几个 iOS 用户所用，不久之后它也会在 Android 上推出。