# 谷歌正在为桌面版 Chrome 添加内置截图工具

> 原文：<https://www.xda-developers.com/google-adding-screenshot-tool-chrome-for-desktop/>

谷歌目前正致力于在 Chrome 桌面版中增加一个统一的分享菜单。我们[在今年五月早些时候首次发现了](https://www.xda-developers.com/google-chrome-consolidated-share-menu-soon/)正在开发的共享菜单，并了解到它将为用户提供四个共享选项——复制链接、二维码、页面另存为和 Cast——在 Chrome 的 Omnibox 中。然而，Chromium Gerrit 上的一个新承诺表明，当它在未来的版本中推出时，共享菜单也将提供一个截图工具。

根据最近来自 *Reddit* 上 [u/Leopeva64-2](https://www.reddit.com/r/chrome/comments/ojzhq0/google_is_working_on_a_builtin_tool_to_take/) 的帖子，Chrome 目前在浏览器的开发者工具中隐藏了一个原生截图工具。[的新承诺](https://chromium-review.googlesource.com/c/chromium/src/+/3023004)旨在通过将该工具添加到正在开发的共享菜单中来集中该工具。它的描述是:*“这一变化开始实施“共享”子菜单，这将集中和消除目前分散在各个菜单中的各种共享选项。”*

该更改还将添加一个名为“ShareMenu”的新功能，一个名为“ShareSubmenuModel”的新类，它实现了新的子菜单，并修改了“RenderViewContextMenu”，以便在启用新功能时使用新的 ShareSubmenuModel。此外，提交的描述表明，它还将在共享菜单中添加“复制链接”和“复制链接到文本”项目和截图项目。

*(图片:u/Leopeva64-2)*

正如你在所附的截图中看到的，谷歌 Chrome 桌面版更新后的分享菜单将比我们今年早些时候看到的更多分享选项。除了上面提到的四个选项，它还将提供一个“截图”选项，“发送到您的设备”选项，以及一个“共享链接到”子菜单，其中包含其他共享选项。分享菜单的图标也被更新了，它现在显示的是一架纸飞机，而不是加号。

*(GIF: u/Leopeva64-2)*

值得注意的是，[单独提交](https://chromium-review.googlesource.com/c/chromium/src/+/2993488)表明即将到来的截图工具可能会让用户选择只捕捉屏幕的特定部分。它可能还具有编辑截图的工具。目前，我们还不确定新的截图工具何时会在稳定频道上向用户推出。一旦我们了解到更多情况，我们会尽快通知您。