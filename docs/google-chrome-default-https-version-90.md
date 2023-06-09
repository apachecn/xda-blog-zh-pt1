# 谷歌 Chrome 在输入 90 版本的网址时会默认使用 HTTPS

> 原文：<https://www.xda-developers.com/google-chrome-default-https-version-90/>

谷歌[今年早些时候开始测试 Chrome 的一项变化](https://www.xda-developers.com/google-chrome-to-default-to-https-when-typing-in-urls/),以改善加密网站的页面加载时间。这一改变修改了浏览器中的 Omnibox 和自动完成代码，以自动加载 HTTPS 版本的网站，而不是先进入未加密的版本。谷歌现在宣布，这一变化将随着桌面和安卓系统的 Chrome 90 更新推出。

本月早些时候，chrome 90 for desktop and Android[在测试频道](https://www.xda-developers.com/google-chrome-desktop-shipping-av1-encoder-improve-video-conferencing/)上推出，带有 AV1 编码器，以改善视频会议。根据最近来自该公司的[博客帖子](https://blog.chromium.org/2021/03/a-safer-default-for-navigation-https.html?m=1)，更新也将包括上面提到的变化，这将改变地址栏的行为，默认使用 *https://* 。这不仅能提高隐私保护，还能确保支持 HTTPS 的网站有更快的加载速度。

正如谷歌解释的那样，*“通过手动键入网址导航到网站的 Chrome 用户通常不会包括“http://”或“https://”。例如，用户经常在地址栏中键入“example.com”而不是“https://example.com”。在这种情况下，如果是用户第一次访问网站，Chrome 之前会选择 http://作为默认协议。这在过去是一个实际的默认，当时很多网站都不支持 HTTPS。”*

从 Chrome 90 开始，对于大多数没有指定协议的输入导航，浏览器将默认为 HTTPS。谷歌声称这不仅是安全和隐私的改善，还将提高支持 HTTPS 的网站的初始加载速度，因为 Chrome 将直接连接到 HTTPS 端点，而无需从 *http://重定向到 https://。*

在网站不支持 HTTPS 的情况下，HTTPS 的尝试失败后，Chrome 将回退到 HTTP。这包括存在证书错误(如名称不匹配或不受信任的自签名证书)或连接错误(如 DNS 解析失败)的情况。

如前所述，这一变化将推广到 Chrome 桌面和 Chrome for Android 版本。它将在未来几周推出 iOS 版 Chrome。