# 微软宣布 Edge 92 将获得自动 HTTPS

> 原文：<https://www.xda-developers.com/microsoft-edge-automatic-https/>

微软宣布将在 92 版 Edge 浏览器中引入自动 HTTPS。它目前可以通过 Dev 和 Canary 频道预览。

它是这样工作的。当你键入一个网址时，你显然不是以“http”或“https”开头。浏览器现在做的是默认为 HTTP，然后重定向到 HTTPS，如果网站支持的话。现在，它将默认使用 HTTPS。

但微软 Edge 只有在认为网站“极有可能”支持更安全的协议(至少在默认情况下)时，才会使用自动 HTTPS。它有一个网站列表，显然包括成千上万的域名。

不过，你实际上可以把这个功能提高一个档次。你可以在 *edge://settings/privacy* 中找到一个功能，你可以改变它，这样*所有的*网站都会从 HTTP 切换到 HTTPS。它还指出，如果您选择这一点，可能会有更多的连接错误。

使用 HTTPS 网站很重要，因为它更安全，或者更确切地说，因为常规的旧 HTTP 非常不安全。正如微软所说，有了 HTTP，坏人可以在你的网络流量传输过程中查看或改变它。简而言之，互联网流量可以被拦截，如果不安全，它可以被操纵。

如果你在 Dev 或者 Canary 频道，还没有的话，可以在*edge://flags/# edge-automatic-https*下启用一个标志。之后，您应该会在设置中看到该功能。

虽然它现在在 Dev 和 Canary 频道，但一旦 Edge 92 发布到该频道，它可能会进入测试版。这计划在 6 月 8 日的那个星期发生，所以不会等很久。当然，如果微软愿意，它可以选择推迟 Edge 93 的发布。

另一方面，谷歌 Chrome 从 Chrome 90 开始[就有这个功能了。由于这是一个安全功能，人们可能会认为，当 Edge 92 在 7 月 22 日这一周向稳定渠道发布时，微软将努力赶上并让每个人都拥有它。](https://www.xda-developers.com/google-chrome-90-stable-rollout/)