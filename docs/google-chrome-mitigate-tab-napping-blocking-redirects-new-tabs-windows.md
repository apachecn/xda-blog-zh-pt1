# 谷歌 Chrome 通过阻止新标签或窗口中的重定向来减少“标签劫持”

> 原文：<https://www.xda-developers.com/google-chrome-mitigate-tab-napping-blocking-redirects-new-tabs-windows/>

您可能已经观察到在任何网站上点击链接时的两种行为之一——链接要么在同一个选项卡中打开，要么在一个新的选项卡/窗口中打开。网站作者可以通过向他们希望在新标签中打开的 URL 添加 [target="_blank"](https://www.xda-developers.com/chrome-crakc-down-page-redirects/) 属性来控制这种行为。此属性指示浏览器在单击时在新选项卡中打开链接。但是这个属性有一个[已知的安全问题](https://www.xda-developers.com/chrome-crakc-down-page-redirects/)，它让新打开的页面利用 JavaScript 将你重定向到一个不同的 URL。这造成了严重的威胁，因为重定向的 URL 可能是一个恶意软件网站或钓鱼页面。为了解决这个问题，谷歌 Chrome 采取了新的安全措施。

正如最近一份来自[*bleeding computer*](https://www.bleepingcomputer.com/news/security/google-chrome-to-block-javascript-redirects-on-web-page-url-clicks/)的报告所解释的，网站作者已经可以通过使用 **rel="noopener"** HTML 链接属性来阻止新标签使用 JavaScript 重定向到不同的 URL。但是，他们必须手动将属性添加到每个具有 target="_blank "属性的链接中。早在 2018 年，苹果[在 Safari 中做了一个改变](https://webkit.org/blog/8475/release-notes-for-safari-technology-preview-68/)，在利用 target="_blank "的 HTML 链接上自动暗示了 noopener 属性。得益于此，即使作者没有使用 rel="noopener "属性，浏览器也会自动保护新标签。上周，微软 Edge 开发者 Eric Lawrence [在 Chromium 中实现了同样的功能](https://bugs.chromium.org/p/chromium/issues/detail?id=898942#c28)。这意味着它也将被引入所有基于 Chromium 的浏览器，如微软 Edge、谷歌 Chrome、Brave 等等。

在对安全措施的评论中，劳伦斯指出:

为了减轻“标签劫持”攻击，其中由受害者上下文打开的新标签/窗口可以导航该打开者上下文，HTML 标准被改变以指定 target_blank 的锚应该表现得好像|rel="noopener"|被设置。希望退出此行为的页面可以设置|rel="opener"|，"

新的安全措施目前在 Chrome Canary 频道启用，预计明年 1 月将在 Chrome 88 上稳定推出。如前所述，该特性实质上意味着 HTML 链接上的“noopener”属性，该属性利用 target="_blank "并阻止页面使用 JavaScript 重定向到新页面，除非另有说明。

这项新的安全措施是在谷歌修补了 Chrome 的两个零日漏洞几天后出台的。你可以通过点击[此链接](https://www.xda-developers.com/google-fixes-two-zero-day-chrome-flaws-exploited/)了解更多关于这些漏洞的信息。