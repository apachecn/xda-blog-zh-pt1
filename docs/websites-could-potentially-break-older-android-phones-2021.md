# [更新:危机解除]2021 年，许多网站可能会在旧的安卓手机上崩溃

> 原文：<https://www.xda-developers.com/websites-could-potentially-break-older-android-phones-2021/>

虽然在过去几年里, [Project Treble](https://www.xda-developers.com/tag/project-treble/) 在改善最新版本 Android 的发行方面发挥了重要作用，但碎片化[仍然是 Android 生态系统最大的缺点之一](https://www.xda-developers.com/android-version-distribution-statistics-android-studio/)。目前使用的大量 Android 设备运行的是过时版本的操作系统，这可能会导致各种问题。例如，由于根证书过期，许多网站明年可能会在旧的 Android 设备上崩溃。

当几年前首次推出为 TLS 加密提供免费证书的非营利认证机构 Let's Encrypt 时，该组织与 IdenTrust 的 DST 根 X3 证书进行了交叉签名，该证书已使用多年，受到大多数主要软件平台的信任，包括 Windows、iOS、Android、macOS 和许多 Linux 发行版。迄今为止，数以百万计的网络域名受到了 Let's Encrypt 证书的保护，但正如[最近的一篇来自 Let's Encrypt 的博客文章](https://letsencrypt.org/2020/11/06/own-two-feet.html)所指出的，DST 根 X3 根证书将于 2021 年 9 月 1 日到期。

Let's Encrypt 与 IdenTrust 的合作对于现有设备快速信任前者的证书是必要的，但同时，该组织发布了自己的根证书(ISRG 根 X1)，并努力使其受到大多数主要操作系统的信任。然而，一些自 2016 年以来一直没有更新的软件不会信任新的根证书，这包括运行 7.1.1 以下版本的 Android 设备。因此，当 DST 根 X3 根证书明年到期时，许多旧的 Android 设备将不再信任由 Let's Encrypt 颁发的证书，因此在访问其 TLS 加密用 Let's Encrypt 证书签名的网站时会出现证书错误。

根据来自 Android Studio 的[最新 Android 分发统计数据](https://www.xda-developers.com/android-version-distribution-statistics-android-studio/)(如下所示)，截至 2020 年 4 月，流通中的 Android 设备中有 33.8%运行比 7.1 牛轧糖更老的 Android 版本。这相当于拥有加密证书的网站流量的 1-5%。虽然到明年夏令时根 X3 到期时，运行旧版本 Android 操作系统的设备比例无疑会下降，但根据目前的趋势，这一比例的下降可能不会很大。

为了最大限度地减少这一变化对最终用户的影响，Let's Encrypt 提供了两种解决方案。针对网站所有者的第一个解决方案将在明年 1 月引入对 Let's Encrypt API 的更改，以便在默认情况下， *"ACME 客户端将提供通向 ISRG 根 X1 的证书链。* *但是，也有可能为同一证书提供一个备用证书链，该证书链通向 DST 根 X3 并提供更广泛的兼容性。”*

对于拥有运行旧版本 Android 的设备的最终用户，Let's Encrypt 建议安装 Firefox 来规避这个问题。不同于股票浏览器应用程序依赖于操作系统的可信根证书列表，Firefox 自带了自己的可信根证书列表。最新版本的安卓版火狐浏览器包括一个最新的可信认证机构列表，它将允许使用过时版本安卓系统的用户打开拥有加密证书的网站。

## 更新 1:旧 Android 设备兼容性扩展，让我们加密证书

正如今天[在一篇博客文章](https://letsencrypt.org/2020/12/21/extending-android-compatibility.html)中宣布的，运行 7.1.1 之前版本的旧 Android 设备将能够在明年与 IdenTrust 的最初交叉签名合作关系到期后访问使用 Let's Encrypt 证书的网站。事实证明，Android 并没有“强制执行用作信任锚的证书的截止日期。”正因为如此，IdenTrust 为 Let's Encrypt 的 ISRG 根 X1 证书颁发了一份来自其 DST 根 CA X3 的 3 年交叉签名协议，尽管后者将于明年到期。因此，不会对使用旧 Android 手机的用户产生影响，避免了这些设备上许多网站的潜在破坏。