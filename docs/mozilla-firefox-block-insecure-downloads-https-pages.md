# Mozilla Firefox 还将阻止 HTTPS 页面上不安全的下载

> 原文：<https://www.xda-developers.com/mozilla-firefox-block-insecure-downloads-https-pages/>

# Mozilla Firefox 还将阻止 HTTPS 页面上不安全的下载

Mozilla 正准备在 Firefox 92 中阻止 HTTPS 网页上的不安全下载。这是继 2020 年谷歌 Chrome 添加的类似功能之后。

Mozilla 正准备在下一个主要版本中阻止从火狐 HTTPS 页面开始的不安全下载。一个类似的功能[于去年在谷歌 Chrome](https://www.xda-developers.com/google-chrome-block-insecure-downloads-https-pages/) 上推出，通常被称为混合内容下载阻止。

该功能旨在确保用户知道他们从哪些网站下载文件。当您访问 HTTPS 页面时，您希望您与网站共享的任何信息在传输过程中受到保护。但是，使用 HTTPS 的网站可以链接到常规的 HTTP 网站，包括文件下载。用户可能会不知不觉地连接到更容易受到第三方攻击的网站。

通过阻止从 HTTPS 页面开始的不安全的 HTTP 下载，Firefox 可以让用户知道他们何时试图下载一个可能在下载过程中被篡改的文件。这可能会导致下载不同的文件，而不是预期的文件。但是，如果用户信任有问题的网站，他们可以选择继续下载。您可以在下图中看到警告。

然而，该特性的目标并不是阻止所有的 HTTP 下载。如果你访问的是一个 HTTP 页面，下载还是一样的。此外，地址栏中粘贴的文件下载的直接链接也可以。如上所述，我们的目标是确保用户在使用 HTTPS 时可以信任网站和下载的文件。

根据 Mozilla 的 [bug 追踪器](https://bugzilla.mozilla.org/show_bug.cgi?id=1722286)中的参考，该特性计划在 Firefox 92 中普遍提供。这是火狐的下一个重大更新，目前[计划在 9 月 7 日发布](https://wiki.mozilla.org/Release_Management/Calendar)。虽然它已经在 Firefox 的实验版本中可用，但是你也可以通过一个标志在稳定版本中启用它。只需进入 *about:config* ，搜索*DOM . block _ download _ unsecure*。将该值设置为 t*true*将启用混合内容下载阻止。