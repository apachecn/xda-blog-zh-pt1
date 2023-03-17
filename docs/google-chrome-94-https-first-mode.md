# 谷歌希望通过 Chrome 的 HTTPS 优先模式推动 HTTPS 的应用

> 原文：<https://www.xda-developers.com/google-chrome-94-https-first-mode/>

HTTPS 是超文本传输协议安全的缩写，它使用传输层安全性(TLS)来保护用户和网站之间传输的数据。多年来，网站管理员一直被建议在他们的网站上采用 HTTPS 来保护用户，由于该协议的广泛采用，大多数网络浏览器都将 HTTPS 作为页面加载的默认选项。仍然有一些坚持者没有采用 HTTPS 进行页面加载，所以谷歌在 Chrome 中引入了一种新模式，这种模式将保护用户不通过 HTTP 连接到网站。

随着 9 月底 Chrome 94 的发布，用户将能够启用新的 HTTPS 优先模式。一旦启用，Chrome 浏览器将尝试将所有页面加载升级到 HTTPS，并在通过 HTTP 加载任何网站之前显示整页警告。这确保了 Chrome 尽可能通过更安全的协议将用户连接到网站。该模式还会在用户试图通过不太安全的 HTTP 连接到某个站点之前警告用户。

*HTTPS——谷歌 Chrome 浏览器的第一模式，正如[之前由](https://www.xda-developers.com/google-chrome-prepares-https-only-mode/)[Chrome Story](https://www.chromestory.com/2021/06/enable-https-only-mode-chrome/)发现的*

谷歌仍在评估 HTTPS 优先是否会被默认启用。自去年年底 Firefox 83 发布[以来，Mozilla 一直在测试一种类似的仅 HTTPS 模式，该公司](https://www.xda-developers.com/mozilla-firefox-83-pinch-to-zoom-https-only-mode/)[称](https://blog.mozilla.org/attack-and-defense/2021/03/10/insights-into-https-only-mode/)该机制成功升级了超过 73%的传统地址的顶级负载。鉴于谷歌 Chrome 的用户数量庞大，我们预计会看到类似的改进，因为许多用户并不知道 HTTP 和 HTTPS 之间的区别。

说到这里，Chrome 正在尝试改变浏览器的锁图标，以减少对 HTTPS 在安全方面实际意义的混淆。谷歌进行的研究表明，用户经常将锁图标与网站的实际可信度联系在一起，而事实上该图标仅表示连接的安全性。为了减少这种混乱，谷歌正在 Chrome 93 中进行一项实验，用一个更中性的下拉箭头取代地址栏中的锁图标，否则会显示相同的页面加载信息。然而，一个[“不安全”指示器](https://www.xda-developers.com/google-chrome-68-http-not-secure/?)仍然会显示在没有 HTTPS 支持的网站上，企业也可以选择完全退出这个实验。

最后，谷歌声明 Chrome 将继续支持传统的 HTTP 连接，但他们[将评估](https://www.chromium.org/Home/chromium-security/deprecating-powerful-features-on-insecure-origins)新的网络平台功能是否会在 HTTP 网页上受到限制。