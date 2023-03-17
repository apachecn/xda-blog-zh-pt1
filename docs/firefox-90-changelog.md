# 桌面版和安卓版的 Mozilla Firefox 90 有什么新功能

> 原文：<https://www.xda-developers.com/firefox-90-changelog/>

# Firefox 90 在桌面和安卓系统上都有大量的改进

Firefox 90 现在正在 Windows、macOS、Linux 和 Android 上推出，具有令人印象深刻的性能提升和更好的自动填充功能。

Firefox 是少数几个拥有自己渲染引擎的浏览器之一，Opera、Brave、Edge 和其他浏览器现在都使用谷歌的 Chromium 引擎。这意味着 Mozilla 可以尝试谷歌可能不感兴趣的新改进和渲染变化，随着浏览器的更多部分用 Rust 编程语言重写，Firefox 变得越来越快。Mozilla 现在正在桌面和安卓平台上推出 90 版 Firefox 浏览器，并做了一些有益的改进。

桌面上的 Firefox 90 增加了保存、管理和自动填写信用卡信息的功能，这是多年来在 Chrome 和 T4 Safari 上已经有的功能。此次更新还推出了 WebRender(也称为 [Quantum Render](https://wiki.mozilla.org/Platform/GFX/Quantum_Render) )，这是一种用 Rust 编写的速度更快的页面合成器，适用于大多数电脑。除了 Chromebooks 和芯片组使用 PowerVR 和 Adreno 4(骁龙 808，骁龙 415 等)的手机/平板电脑，所有 Android 设备上都已经可以使用 WebRender。)图形。今年早些时候 Chrome中也移除了 Firefox 90 中的 FTP 支持。

### Firefox 90 桌面变更日志

*   在 Windows 上，当 Firefox 没有运行时，[更新现在可以在后台](https://support.mozilla.org/kb/enable-background-updates-firefox-windows)应用。
*   Firefox for Windows 现在提供了一个新的页面[关于:第三方](https://support.mozilla.org/kb/identify-problems-third-party-modules-firefox-windows)来帮助识别由第三方应用程序引起的兼容性问题
*   [仅 HTTPS 模式的例外情况](https://support.mozilla.org/kb/https-only-prefs)可在“关于:首选项#隐私”中管理
*   打印到 PDF 现在产生工作超链接
*   “在新标签中打开图像”上下文菜单项现在默认在背景标签中打开图像和媒体
*   大多数没有硬件加速 WebRender 的用户现在将使用软件 WebRender。
*   改进的软件 web 渲染性能
*   FTP 支持已被移除
*   Firefox 的 SmartBlock 功能第二版进一步改善了隐私浏览。第三方脸书脚本被屏蔽，以防止你被跟踪，但现在，如果你决定在任何网站上“用脸书登录”，它们会“及时”自动加载。
*   DevTools 中提供了对私有字段的支持( [TC39 提案](https://github.com/tc39/proposal-class-fields#private-fields)，阶段 3)。支持包括:对象检查、自动完成、表达式求值、变量工具提示和漂亮的打印( [bug](https://bugzilla.mozilla.org/show_bug.cgi?id=1650188) )
*   支持[获取元数据请求头](https://blog.mozilla.org/security/2021/07/12/firefox-90-supports-fetch-metadata-request-headers/)，这允许 web 应用程序更好地保护自己和用户免受各种跨来源的威胁。
*   添加了使用存储在硬件令牌或操作系统存储中的客户端身份验证证书的功能。
*   网络面板在响应标签中显示了对字体的 HTTP 请求的预览( [bug](https://bugzilla.mozilla.org/show_bug.cgi?id=872078) )
*   各种[安全修复](https://www.mozilla.org/security/advisories/mfsa2021-28/)

### 火狐 90 安卓变更日志

*   Firefox 现在可以[为你保存、管理和自动填写信用卡信息](https://support.mozilla.org/kb/automatically-fill-credit-card-information-firefox)，让在 Firefox 上购物更加方便。
*   现在，使用卸载事件侦听器的网页启用了后退/前进缓存(也称为 BFCache ),使得这些页面上的后退和前进导航速度更快。
*   需要导入用户 Android 证书的用户可以通过[秘密设置](https://github.com/mozilla-mobile/fenix/wiki/%22Secret-settings%22-debug-menu-instructions)进行导入
*   各种稳定性和[安全性修复](https://www.mozilla.org/security/advisories/mfsa2021-28/)

与此同时， [Android 版 Firefox](https://www.mozilla.org/en-US/firefox/android/90.0/releasenotes/) 也获得了同样的信用卡自动充值支持。Mozilla 还为一些页面推出了后退/前进缓存(BFCache)，这是[去年在 Android 版 Chrome 中出现的](https://www.xda-developers.com/back-forward-google-chrome-faster-bfcache/)(谷歌[仍在桌面浏览器上测试它](https://www.xda-developers.com/google-chrome-desktop-back-forward-cache/))。不幸的是，Firefox 90 for Android 不包括期待已久的通用扩展支持[的回归——你仍然必须从应用程序设置中的少数可用选项中进行选择。](https://www.androidpolice.com/2020/09/03/firefox-update-faces-backlash-due-to-missing-features-and-few-supported-extensions/)

可以从[浏览器官网](https://www.mozilla.org/en-US/firefox/new)下载桌面平台的 Firefox。安卓版本在谷歌 Play 商店的[有售。](https://play.google.com/store/apps/details?id=org.mozilla.firefox)