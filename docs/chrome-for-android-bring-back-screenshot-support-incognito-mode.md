# Android 上的 Chrome Canary 支持匿名模式下的屏幕截图

> 原文：<https://www.xda-developers.com/chrome-for-android-bring-back-screenshot-support-incognito-mode/>

# Android 版 Chrome 可能很快会恢复匿名模式下的屏幕截图支持

谷歌在加那利分公司的安卓 Chrome 上添加了一个新的标志，允许在匿名模式下截图。看看吧！

早在 2018 年，谷歌就取消了 Android 上 Chrome v65 在隐名模式下截图的功能。这项功能是作为保护用户隐私的措施而受到限制的。然而，这种情况似乎很快就会改变，该功能可能会重新推出。虽然手头有一些复杂性，但 Chrome 团队已经在 Chrome 89 Canary 上添加了一个标志，允许用户在匿名页面上截屏。

截至目前，如果你正在 Android 设备上使用 Chrome，并试图对一个在匿名选项卡中打开的网页进行截图，你应该会看到一条消息，称“此处无法截图”。禁用截图背后的想法是，当[用户不想将历史留在](https://www.xda-developers.com/google-is-being-sued-for-tracking-users-in-incognito-mode/)之后时，通常会选择匿名浏览，而截图不过是同样情况的证明。正如 [*Techdows*](https://techdows.com/2020/11/chrome-canary-lets-you-take-screenshots-in-incognito-on-android.html) 所指出的，官方 [Chromium Bug 报告页面](https://bugs.chromium.org/p/chromium/issues/detail?id=985245)上的一个帖子提到，有一些复杂性使得很难添加一个设置来实现这一点。首先，隐姓埋名没有任何现有的设置，这使得添加一个“新的”隐名设置非常重要。在 Android 如何分割屏幕模糊和屏幕截图功能方面做出所要求的改变之前，该设置不会是开或关的选择，而是:“屏幕截图启用”或“隐藏屏幕”。

值得注意的是，其他基于 Chromium 的 Android 网络浏览器，如 Firefox，包括一个“允许在私人浏览中截图”的选项，而 Kiwi browser 提供了“保护匿名窗口”隐私设置，让你隐藏内容，并防止在匿名模式下截图。

目前，开发人员已经在 Chrome v89 Canary 上添加了一个新标志，允许你在匿名模式下截图。这可以通过以下步骤完成:

*   打开 Chrome 金丝雀
*   访问 chrome://flags
*   搜索“隐姓埋名截图”
*   单击下拉箭头并启用设置
*   重启浏览器

我们还没有得到谷歌的确认，这一功能是否真的会在未来向所有用户推出。