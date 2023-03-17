# Mozilla 在 Firefox 83 中增加了缩放支持和仅 HTTPS 模式

> 原文：<https://www.xda-developers.com/mozilla-firefox-83-pinch-to-zoom-https-only-mode/>

Mozilla 已经宣布发布 Firefox 83，这是一个引入了对纯 HTTPS 模式支持的更新。等着瞧吧:缩放。

仅 HTTPS 模式将尝试与您正在访问的网站建立安全连接。这意味着如果你点击一个 HTTP 链接或者手动输入一个 HTTP 地址，Firefox 83 将尝试使用 HTTPS 访问该网站。如果无法建立安全连接，Firefox 会在连接到网站之前征求您的许可。

Firefox [指出](https://www.mozilla.org/en-US/firefox/83.0/releasenotes/)如今大多数主流网站都支持 HTTPS 协议，该协议在你的浏览器和你访问的网站之间提供了更好的加密。但是有一些网站仍然在使用 HTTP 协议。还有数百万个传统 HTTP 链接，因此 Firefox 83 中的 HTTPS 专用模式旨在为用户提供更安全的连接。

Firefox 表示，也可能存在一种罕见的情况，即一个网站在 HTTPS 可以访问，但其中包含的资源在 HTTPS 无法访问。因此，一些网站可能看起来不正确或会完全失灵。如果发生这种情况，用户可以通过单击地址栏中的锁图标轻松禁用仅 HTTPS 模式。

Firefox 83 还包括 Windows 和 Mac 上的缩放支持。如果你使用的是带触摸屏的 Windows 设备，你可以轻松地缩放你想要的网站。Mac 设备上的触摸板也是如此。这是一个在竞争浏览器中已经存在多年的功能，但迟做总比不做好。

Firefox 83 还包括其他几个功能，包括画中画模式的键盘快捷键，支持 AcroForm，支持[苹果新的 M1 芯片](https://www.xda-developers.com/apple-macbook-air-macbook-pro-13-mac-mini-m1-arm-soc/)。Firefox 83 也推出了 Android 设备，支持几个新的插件，包括 FoxyProxy，Bitwarden，AdGuard AdBlocker，Tomato Clock，LeechBlock NG，Web Archives 和 Ghostery。

如果你想要更安全的浏览体验，并且你是火狐用户，那么你应该现在下载最新的更新。您可以在下面查看完整的 Firefox 83 桌面版变更日志。

## Firefox 83 变更日志:

### 新的

*   由于我们的 JavaScript 引擎 SpiderMonkey 的重大更新，Firefox 变得越来越快，您现在将体验到页面加载性能提高了 15%，页面响应速度提高了 12%，内存使用减少了 8%。我们已经替换了 JavaScript 引擎的一部分，帮助您编译和显示网站，同时提高了引擎的安全性和可维护性。
*   火狐推出 HTTPS 独有模式。启用后，这种新模式可以确保 Firefox 与网络的每个连接都是安全的，并在安全连接不可用时提醒您。[你可以在火狐的偏好设置中启用它。](https://support.mozilla.org/kb/https-only-prefs#w_enable-https-only-mode)
*   对于使用 Windows 触摸屏设备和 Mac 设备触摸板的用户，现在将支持捏合缩放。Firefox 用户现在可以在支持触摸的设备上使用 pinch 来放大和缩小网页。
*   画中画现在支持快进和快退视频的键盘快捷键:使用箭头键向前和向后移动 15 秒，以及音量控制。有关支持的命令列表，请参见[支持 Mozilla](https://support.mozilla.org/kb/about-picture-picture-firefox#w_keyboard-shortcuts)
*   当您在 Firefox 的视频会议上展示您的屏幕时，您将看到我们改进的用户界面，它使哪些设备或显示器正在被共享变得更加清晰。
*   我们改进了许多 Firefox 搜索功能的功能和设计:
    *   现在，在搜索面板底部选择一个搜索引擎会进入该引擎的搜索模式，允许您查看搜索词的建议(如果有的话)。旧的行为(立即执行搜索)可通过按住 shift 键单击来实现。
    *   当 Firefox 自动完成某个搜索引擎的 URL 时，您现在可以通过选择地址栏结果中的快捷方式，直接在地址栏中搜索该引擎。
    *   我们在搜索面板的底部添加了按钮，允许您搜索书签、打开标签和历史记录。
*   Firefox 支持 AcroForm，这将允许您[填写、打印和保存支持的 PDF 表单](https://support.mozilla.org/kb/view-pdf-files-firefox-or-choose-another-viewer)，PDF 查看器也有了新的外观。
*   我们在印度的火狐英文版用户现在可以在他们的新标签中看到口袋推荐，里面有一些网络上最好的故事。如果你没有看到它们，你可以通过[按照这些步骤](https://support.mozilla.org/kb/hide-or-display-content-new-tab)在你的新标签页中打开口袋文章。
*   对于最近发布的使用苹果硅 CPU 构建的苹果设备，您可以使用 Firefox 83 和未来版本，无需任何更改。这个版本(83)将支持苹果公司的 Rosetta 2 下的仿真。我们正致力于在未来的版本中为这些 CPU 原生编译 Firefox。
*   这是 WebRender 的一个重要版本，因为我们在 Windows 7 和 8 以及 macOS 10.12 到 10.15 上向更多的 Firefox 用户推出了。

### 固定的；不变的

*   此版本还包括许多辅助功能修复:
    *   屏幕阅读器的报告段落功能现在可以正确地报告段落，而不是谷歌文档中的行
    *   当使用屏幕阅读器逐字阅读时，当附近有标点符号时，单词现在会被正确报告
    *   在画中画窗口中使用 tab 键后，箭头键现在可以正常工作
*   对于在 macOS 上使用最小化窗口恢复会话的用户来说，Firefox 现在使用更少的电量，你应该会看到更长的电池寿命。
*   各种[安全修复](https://www.mozilla.org/security/advisories/mfsa2020-50/)

### 网络平台

*   这个版本在 CSS 中增加了对[圆锥渐变的支持，帮助颜色在围绕中心旋转时平滑过渡，而不是从中心向外前进。](https://developer.mozilla.org/docs/Web/CSS/conic-gradient)