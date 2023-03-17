# 火狐 92 推出 HTTPS 改进和 Android 上的网络认证

> 原文：<https://www.xda-developers.com/firefox-92/>

Mozilla 发布了适用于所有主要平台的最新版本的 Firefox 浏览器。作为少数几个仍然使用自己的渲染引擎的浏览器之一，Firefox 仍然拥有大量的追随者，92 版包括一些显著的改进。与此同时，iOS 用户也可以获得火狐 37 自带的新闻。

对于桌面用户来说，Firefox 92 对 HTTPS 进行了改进。浏览器现在可以使用 HTTPS RR 作为 Alt-Svc 头，这可以将一些网站连接升级到 HTTPS。这是 Firefox 版本 91 的后续版本，它尽可能将 HTTPS 作为默认连接类型，只有在必要时才回退到 HTTP。还有一些针对 macOS 用户的升级，比如可以从 Firefox 的文件菜单访问系统的共享选项。您可以在下面找到 desktop 的新功能、更改和修复的完整列表:

### Firefox 92 桌面版变更日志

### 新功能

*   更安全的连接:火狐现在可以使用 HTTPS RR 作为 Alt-Svc 头自动升级到 HTTPS。
*   现在，许多系统都支持视频回放的全范围色阶。
*   Mac 用户现在可以从 Firefox 的文件菜单中访问 macOS 共享选项。
*   macOS 上启用了对包含 ICC v4 配置文件的图像的支持。

### 变化

*   macOS 上的书签工具栏菜单现在遵循 Firefox 的视觉风格。
*   证书错误页面已经过重新设计，以提供更好的用户体验。
*   继续努力重组 Firefox 的 JavaScript 内存管理，以提高性能和使用更少的内存。

### 修理

*   如果在 Firefox 之后安装或更新 Mozilla Thunderbird，Firefox 的屏幕阅读器和其他辅助工具的性能不再会严重下降。
*   macOS VoiceOver 现在可以正确报告使用 aria-expanded 属性标记为“扩展”的按钮和链接。
*   选项卡中打开的警报不再会导致使用相同流程的其他选项卡出现性能问题。
*   各种[安全修复](https://www.mozilla.org/security/advisories/mfsa2021-38/)

对于 Android 用户来说，Firefox 92 最大的新闻是支持 Web 认证 API，或 WebAuthn。这允许用户使用 USB 令牌或安全密钥登录网站。以下是完整的变更日志:

### Android 版 Firefox 92 变更日志

### 新功能

*   增加了对 Web 身份验证 API 的支持，允许 USB 令牌(如使用 USB 或蓝牙安全密钥)进行网站身份验证。

### 修理

*   尝试从 Mozilla 帐户断开连接时崩溃。
*   禁用病历报告后导航回设置菜单时崩溃。
*   各种[安全修复](https://www.mozilla.org/security/advisories/mfsa2021-38/)

最后，正如我们在开始时提到的，iOS 用户正在同时获得 Firefox 37。由于苹果的要求，iOS 版火狐使用 WebKit 而不是 Mozilla 的 Gecko 引擎。不管怎样，这里有一些值得注意的新增功能，比如手动添加新账户到 Firefox 的密码管理器。除其他新增功能外，还对增强跟踪保护(ETP)进行了改进。以下是完整的变化列表:

### Firefox 37 for iOS changelog

*   您现在可以手动向密码管理器添加新帐户。
*   干净启动:如果浏览器关闭超过 4 小时，Firefox 将在你的主页上打开。
*   快速主页访问:你现在可以在工具栏上找到主页按钮。
*   我们对增强跟踪保护(ETP)菜单(见锁图标)进行了改进，为您提供有关您所访问网站安全性的更多信息。

如果你想下载火狐 92 版，你可以在 Mozilla 的网站上找到桌面版。如果你在手机上，你可以在谷歌 Play 商店上找到安卓版的[火狐，在应用商店](https://play.google.com/store/apps/details?id=org.mozilla.firefox)上找到 iOS 版的[火狐。](https://apps.apple.com/us/app/firefox-private-safe-browser/id989804926)