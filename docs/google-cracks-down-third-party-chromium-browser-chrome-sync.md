# 谷歌打击使用 Chrome Sync 的第三方 Chrome 浏览器

> 原文：<https://www.xda-developers.com/google-cracks-down-third-party-chromium-browser-chrome-sync/>

# 谷歌打击使用 Chrome Sync 的第三方 Chrome 浏览器

谷歌宣布将限制对其私有 Chrome APIs 的访问，包括第三方 Chrome 浏览器使用的 Chrome Sync API。

如果你使用的是第三方 Chrome 浏览器和 Chrome Sync，那么你会失望地得知谷歌正在打击这种做法。

在 Chromium 博客上发布的一篇简短博文[中，谷歌宣布将从 2021 年 3 月 15 日开始限制对其私有 Chrome APIs 的访问。谷歌官方 Chrome 浏览器使用这些 API 来支持 Chrome Sync 和 Click to Call 等专有功能。前者允许用户在登录同一谷歌账户的浏览器之间同步书签、浏览器历史、打开的标签等，而后者允许用户通过点击有效的电话号码从任何网页快速拨打电话。这两个功能都是由谷歌开发的，并不是开源 Chromium 项目的一部分，而谷歌 Chrome 和其他基于 Chromium 的浏览器——如微软 Edge——都是基于开源 Chromium 项目的。](https://blog.chromium.org/2021/01/limiting-private-api-availability-in.html)

通过限制对私有 Chrome APIs 的访问，谷歌并不打算惩罚第三方 Chrome 浏览器的用户。谷歌不会删除任何已经从这些第三方浏览器同步的数据，但他们也不会在 3 月 15 日之后同步任何新数据。如果您使用第三方 Chromium 浏览器在本地存储了任何数据，Google 鼓励您前往 My Google Activity 页面查看和管理您的数据，或者前往 Google Takeout 下载您的数据。

今天的举动并不令人意外。Chrome Sync 从来都不是基于 Chrome 的浏览器的标准特性，许多第三方 chrome 浏览器会明确警告你这一点。谷歌在过去限制了对其他私有 API 的访问，特别是在 Android 方面，所以任何在项目中启用 Chrome Sync 的开发者都知道这可能会发生。这很遗憾，但这是谷歌让人们使用 Chrome 而不是另一个基于 Chrome 的浏览器的最好方法之一。