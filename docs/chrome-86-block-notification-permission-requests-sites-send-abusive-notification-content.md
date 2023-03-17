# Chrome 86 将阻止发送滥用通知内容的网站的通知权限请求

> 原文：<https://www.xda-developers.com/chrome-86-block-notification-permission-requests-sites-send-abusive-notification-content/>

# Chrome 86 将阻止发送滥用通知内容的网站的通知权限请求

Chrome 86 将阻止发送误导用户的辱骂通知内容的网站的通知权限请求。

谷歌[本月早些时候开始在稳定频道推出](https://www.xda-developers.com/google-chrome-86-rolls-out-with-flags-for-menu-icons-back-forward-cache-and-more/) Chrome 86。此次更新引入了安全改进，可在用户保存的密码遭到破坏时提醒用户，新的菜单图标可帮助用户轻松导航大菜单，原生文件系统 API，增强的 Android 安全浏览，以及几项面向开发者的技术更改。根据 Chromium 博客上[最近的一篇帖子，Chrome 86 还包括通知权限请求的更改，以防止网站发送辱骂性的通知内容。](https://blog.chromium.org/2020/10/reducing-abusive-notification-content.html)

对于不知情的人，谷歌[在 Chrome 80 中引入了安静通知权限 UI](https://www.xda-developers.com/google-chrome-80-rolling-android-desktop/) 。随着 Chrome 84 的更新，该公司发布了[自动注册安静通知 UI](https://www.xda-developers.com/google-chome-84-abusive-notifications-permissions-requests/) ，用于使用欺骗性模式请求通知访问的网站。现在，随着 Chrome 86 的推出，该公司已经开始阻止推送辱骂通知内容的网站的通知权限请求。

更新后的用户界面现在主动阻止用户向使用 web 通知发送恶意软件或模仿系统消息来获取用户凭据的网站授予通知访问权限。为了有效地检测沉迷于此类行为的网站，如果请求推送通知权限，Google 的自动 web 爬行服务将偶尔订阅网站推送通知。发送到自动化 Chrome 实例的通知将被评估滥用内容，如果问题未解决，发送滥用通知的网站将被标记为强制执行。

如果 crawler 发现某个网站存在任何类型的通知滥用，搜索控制台将在新用户界面实施前至少 30 天，在该网站的搜索控制台中提醒注册的网站所有者和用户。在此期间，违规网站可以解决问题，并要求再次审查。为了进一步减少 Chrome 中的通知权限滥用，谷歌现在正在开发一个功能，可以自动恢复违规网站的通知访问。该功能将在未来的更新中发布。