# Firefox 88 取消了对 FTP 链接的支持，将于 6 月全面取消

> 原文：<https://www.xda-developers.com/firefox-88-disables-ftp-support/>

# Mozilla Firefox 88 不再支持 FTP，完全删除 Firefox 90

Mozilla 将从 4 月 19 日开始推出 Firefox 88，不再支持 FTP(文件传输协议)链接。请继续阅读！

随着 Firefox 88 的发布，Mozilla 停止了对 FTP(文件传输协议)链接的支持。开发者去年宣布了从浏览器中移除内置 FTP 实现的计划。然而，由于冠状病毒疫情，该计划被推迟。在[的一篇新博客文章](https://blog.mozilla.org/addons/2021/04/15/built-in-ftp-implementation-to-be-removed-in-firefox-90/)中，Mozilla 现在确认该实现目前在 Firefox Nightly 和 Beta 预发布渠道中被禁用，并将在 4 月 19 日 Firefox 88 发布时对所有用户禁用。一旦实现被禁用，Firefox 将把 ftp://链接传递给外部应用程序。

此外，有计划在 Firefox 90 中完全删除 FTP 实现，预计 Firefox 90 将于 6 月发布。新的变化预计也会影响安卓版本的浏览器。值得注意的是，谷歌 Chrome 早在 2021 年 1 月就已经取消了对 FTP 网址的支持。

"*扩展可以通过‘FTP’的大多数地方，例如代理或 webRequest 的过滤器，应该不会导致错误，但是 API 将不再处理这些类型的请求。为了帮助弥补这种删除，ftp 已被添加到浏览器扩展支持的 protocol_handlers 列表中。这意味着扩展将能够提示用户启动一个 FTP 应用程序来处理某些链接。*

据*安卓警察*T3[报道，火狐 88 安卓版显然已经提前几天发布。在](https://www.androidpolice.com/2021/04/14/you-can-now-download-firefox-88-for-android/) [Firefox 88 beta](https://www.mozilla.org/en-US/firefox/88.0beta/releasenotes/) 发布期间，发布说明提到新的更新将修复全屏或画中画模式下的视频播放在使用桌面视窗的网站上无法正确显示的问题，特别是在 Android 的 Firefox 上。Firefox 88 也有望将 URL 栏的页面操作菜单中的截屏功能移动到一个常规图标中，用户可以从自定义菜单中将其添加到工具栏中。