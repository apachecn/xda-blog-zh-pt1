# Bitwarden 密码管理器增加了对 Android 11 内嵌自动填充 API 的支持

> 原文：<https://www.xda-developers.com/bitwarden-password-manager-adds-android-11s-inline-autofill-api/>

# Bitwarden 密码管理器增加了对 Android 11 内嵌自动填充 API 的支持

流行的密码管理器 Bitwarden 的最新测试版更新增加了对 Android 11 的内嵌自动填充 API 的支持。

智能键盘建议功能无疑是 Android 11 中最有用的新增功能之一。该功能本质上[通过在键盘应用和密码管理器中集成内嵌自动填充建议，简化了平台的自动填充体验](https://www.xda-developers.com/android-11-seamless-autofill-keyboard-integration/)。这些建议会出现在键盘应用程序的顶部，而不是出现在输入栏的旁边。但要在你最喜欢的键盘应用程序或密码管理器上使用这一功能，开发者首先必须更新他们的应用程序以支持这一功能。1Password 和 Gbaord 是首批更新支持 Android 11 内嵌自动填充 API 的应用程序。现在，流行的开源密码管理器 Bitwarden 在其最新的测试版中获得了对该功能的支持。

根据 Bitwarden 的 GitHub 上的[最新评论](https://github.com/bitwarden/mobile/pull/1145)(通过 Reddit 用户[/u/rodrigoswz](https://www.reddit.com/r/Android/comments/jrzh05/bitwarden_with_android_11_autofill_keyboard/))，密码管理器现在支持 Android 11 在测试版频道上的内嵌自动填充 API。一旦你在 Android 11 设备上安装了测试版更新，该设备带有一个也支持内嵌自动填充 API 的键盘应用程序，你应该开始在键盘顶部看到密码建议(见附件截图)。但如果你没有使用支持内嵌自动填充 API 的键盘应用程序，Bitwarden 将恢复到之前在输入栏旁边弹出的覆盖图。

该评论进一步指出，内嵌自动填充建议将“根据 InlineSuggestionsRequest 中的规则进行着色”，以便它遵循键盘应用程序的当前主题，但该主题不会影响 Bitwarden 的徽标。它还揭示了如果浏览器自己的自动填充功能被启用，该功能可能无法在某些浏览器上正常工作。还值得注意的是，该功能目前在 Firefox (prod 和 beta)中被破坏，因为浏览器不断重新初始化键盘并删除内嵌演示。然而， [Firefox](https://www.xda-developers.com/tag/firefox/) 已经在最新的夜间版本中解决了这个问题，该修复应该很快就会在测试版中推出。

如果你不想使用内嵌自动填充建议，你可以按照本教程来禁用你的设备上的功能。