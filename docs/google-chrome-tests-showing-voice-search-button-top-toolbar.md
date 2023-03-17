# 谷歌 Chrome 测试显示顶部工具栏有一个语音搜索按钮

> 原文：<https://www.xda-developers.com/google-chrome-tests-showing-voice-search-button-top-toolbar/>

# 谷歌 Chrome 测试显示顶部工具栏有一个语音搜索按钮

最新的谷歌 Chrome UI 测试引入了一个新的标志，在浏览器的顶部工具栏添加了一个语音搜索按钮。

今年 1 月早些时候，我们了解到谷歌正在努力用谷歌助手取代 Chrome 地址栏中的旧语音搜索界面。当时，我们在 Chromium Gerrit 中发现了两个新的提交，突出了一个名为“Omnibox Assistant Voice Search”的新标志，该标志将允许使用 Google Assistant 进行 Omnibox 语音查询。谷歌 Chrome 现在已经开始测试相关的 UI 变化，将在顶部工具栏添加语音搜索按钮。

与变更相关的代码提交只是将[合并到 Chromium Gerrit](https://chromium-review.googlesource.com/c/chromium/src/+/2496031) 中，它添加了一个名为“顶部工具栏中的语音按钮”的新标志，描述为“允许在顶部工具栏中显示语音搜索按钮”当此标志被启用，并且顶部工具栏中的[分享按钮的标志被禁用时，浏览器顶部工具栏中会显示一个语音搜索按钮(见所附截图)。](https://www.xda-developers.com/chrome-test-adds-share-button-toolbar/)

提交的描述进一步指出，如果启用了 omni box-Assistant-voice-search-flag，那么新按钮将启动助手搜索 UI。如果该标志被禁用，该功能将退回到旧的语音搜索用户界面。同样值得注意的是，共享按钮标志将优先于语音按钮标志，所以如果你都启用了，你只会在顶部工具栏看到共享按钮。

这是 Google Chrome 的又一个用户界面测试，不能保证它会渗透到运行稳定版的用户，并默认启用。谷歌一直在进行这类测试，看看用户最喜欢什么。如果这项新功能获得足够的参与，它可能会在未来的版本中添加到稳定频道的谷歌 Chrome 中。