# Android 13“提拉米苏”增加了对另一个私有 DNS 标准的支持

> 原文：<https://www.xda-developers.com/android-13-tiramisu-support-dns-over-https/>

从表面上看，浏览网页对普通用户来说是一个非常简单的过程；你只需要在地址栏里输入一个网址，回车，浏览器就会加载相应的网站。但是，幕后发生的事情，显然牵扯更多。按 enter 键后，您的设备会向域名服务器(DNS)发送查询，将 URL 转换为机器可读的 IP 地址。一旦您的设备收到相应的 IP 地址，它就会打开网站。您的计算机和 DNS 之间的这种通信是通过用户数据协议(UDP)或传输控制协议(TCP)以明文形式完成的，任何可以看到您的连接的人都可以看到它。如果您不希望任何人访问这些数据，您需要使用支持私有 DNS 标准的 DNS，如 TLS 上的 DNS(DoT)或 HTTPS 上的 DNS(DoH)。

许多流行的 DNS 服务器，如 Google Public DNS、NextDNS 和 Cloudflare，都支持 DoT 和 DoH 标准。但是，Android 目前只原生支持 DoT。谷歌在 Android 9 Pie 中增加了对 DoT 的原生支持，恰如其分地命名为 Private DNS，你可以在手机的网络和互联网设置的高级部分找到它。您可以按照本指南中的[步骤进行配置。但是，如果你想配置这些设置，通过 HTTPS 使用 DNS，你必须等到谷歌明年推出 Android 13“提拉米苏”。](https://developers.google.com/speed/public-dns/docs/using#android)

Android 开源项目(AOSP)最近合并的[代码变更](https://android-review.googlesource.com/c/platform/packages/modules/DnsResolver/+/1833144)表明谷歌将在 Android 13 中添加 DoH 支持。它的描述是:*“默认启用 T 中的 DoH 功能”。*由于谷歌内部[将 Android 13 称为 T 或“提拉米苏”，](https://www.xda-developers.com/google-android-13-t-tiramisu-dessert-name/)我们预计该公司明年将在 Android 的“私人 DNS”菜单中添加原生 DoH 支持。

虽然 DoT 和 DoH 本质上做的是相同的事情，但 DoT 使用 TLS(也称为 SSL)来加密 DNS 流量，这与 HTTPS 网站用于加密和验证通信的协议相同。另一方面，DoH 使用 HTTP 或 HTTP/2 协议来发送查询和响应，而不是直接通过 UDP。这两种标准也使用不同的端口，从隐私角度来看，这使 DoH 略有优势。

正如这篇 [*Cloudflare* 帖子](https://www.cloudflare.com/en-gb/learning/dns/dns-over-tls/)所指出的，DoT 为 DNS 流量使用了一个专用端口，任何具有网络可见性的人都可以看到流量，即使请求和响应本身是加密的。然而，DoH 使用端口 443 —所有其他 HTTP 流量使用的端口。这意味着所有 DNS 流量都与其他 HTTPS 流量混合在一起。这使得监控和阻止 DoH 查询变得更加复杂，网络管理员无法在不阻止其他 HTTPS 流量的情况下阻止 DoH 流量。

谷歌可能会在 Android 的网络和互联网设置中为私有 DNS 选项添加 DoH 支持。目前，我们没有关于该功能的任何进一步的细节。我们会尽快更新这篇文章。

*感谢 XDA 公认的开发者 [luca020400](https://forum.xda-developers.com/m/luca020400.5778309/) 的提示！*