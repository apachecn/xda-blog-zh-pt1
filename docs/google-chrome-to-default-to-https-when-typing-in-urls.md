# 谷歌浏览器在输入网址时默认使用 HTTPS

> 原文：<https://www.xda-developers.com/google-chrome-to-default-to-https-when-typing-in-urls/>

谷歌 Chrome 正在测试一项改变，Omnibox 将自动默认为页面的加密(HTTPS)版本，而无需先进入未加密版本。这一举措可以从页面加载时间中节省宝贵的几分之一秒，反映了该公司在 2018 年推出的在搜索结果中优先考虑加密网站的政策。

我们的朋友在 *[Windows 最新](https://www.windowslatest.com/2021/01/03/google-chrome-address-bar-is-about-to-become-more-secure-and-faster/)* 发现了一个新的代码 commit，并由 *[9to5Google](https://9to5google.com/2021/01/11/google-chrome-address-bar-may-soon-default-to-https/)* 进行了扩展，显示谷歌 Chrome 开源版本 Chromium 背后的团队正在将下面的列为实验品[:](https://chromium-review.googlesource.com/c/chromium/src/+/2568448)

修改 omnibox 和 autocomplete 代码，使用 HTTPS 作为默认的导航模式。我们称之为“升级的 HTTPS 导航”。

观察升级后的 HTTPS 导航，直到完成，如果 HTTPS 加载失败，则返回到 HTTP 版本的 URL。它通过引入一个名为 TypedNavigationUpgradeThrottle 的新导航节流器来实现这一点。

虽然你可能认为它已经做到了这一点，但只是在最近几年，默认加密页面才成为常态，在谷歌 Chrome 刚刚成为世界上最流行的浏览器平台时，这样做可能会导致不想要的 404 页面。

这是一个最小的实现，还不能用于一般用途。未来的 CLs 将会观察升级后的 HTTPS 导航几秒钟，并在必要时取消加载，而不是无限期地等待 HTTPS 加载成功，”一名谷歌工程师说。

事实上，一些网站可能只加密其主页，使浏览器很难跟踪是否回退，而其他没有适当实施网站加密的网站可能遭受同样的命运。因此，这仍然是一个进行中的工作，没有商业添加它的时间表。然而，当它出现时，包括微软 Edge 和 Opera 在内的其他 Chromium 浏览器很可能也会效仿。

这是一个很好的例子，说明大型技术如何“推动”行为，然后做出改变来接受它。谷歌决定改变其搜索算法，优先搜索加密网站，这首先导致了向加密的转变。现在，它有能力用它来让网络更快一点。