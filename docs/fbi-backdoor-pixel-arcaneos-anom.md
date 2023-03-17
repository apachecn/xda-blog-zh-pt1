# 一名 XDA 成员不知情地购买了一部带有 FBI 后门的 Pixel 手机

> 原文：<https://www.xda-developers.com/fbi-backdoor-pixel-arcaneos-anom/>

XDA 论坛经常有手机有问题的新用户，但是一个不幸的用户最终遇到了一个没人知道如何解决的问题。事实证明，这位用户购买了一部二手 Pixel 手机，这部手机最初不是由谷歌或官方零售商出售的，而是由美国联邦调查局(FBI)出售的。这部手机带有一个名为 ArcaneOS 的定制 ROM，并预装了名为“ANOM”的消息软件，这是由联邦调查局秘密制作的，用于捕捉罪犯讨论他们的犯罪活动。

五月底，一名 XDA 成员[在我们的 Pixel 4a 论坛](https://forum.xda-developers.com/t/is-it-bricked-cannot-flash-stock-android-to-remove-arcaneos.4285827/)上发帖，寻求他人帮助移除 ArcaneOS 软件并安装谷歌官方 Android 版本。德国 Android 论坛 [*上的另一名用户 Android-Hilfe*](https://www.android-hilfe.de/forum/google-pixel-3-pixel-3-xl-pixel-3a-pixel-3a-xl.3409/google-pixel-3a-auf-standard-rom-zurueck-flashen.973774-page-2.html) 也在 3 月份用他们的 Pixel 手机遇到了类似的问题，但他们用的是 Pixel 3a，而不是 XDA 用户用的 Pixel 4a。

当两个用户都在网上发帖的时候，ArcaneOS 和 ANOM 的存在还没有被公开，所以没有人知道这两个用户的手机实际上在运行什么。ArcaneOS 缺乏谷歌移动服务(因此没有 Play Store ),并隐藏了打开开发者选项的能力，因此用户很难解锁引导加载程序来刷新股票固件。手机的引导加载程序被锁定，尽管他们没有运行股票固件，这是可能的，因为 Pixel 手机支持在锁定的引导加载程序上运行替代操作系统，只要有人将自己的签名密钥添加到 Android 验证启动(AVB)过程中。这就是 Pixel 手机上的引导加载程序在闪存了 CalyxOS 或 GrapheneOS 等安全加固的定制 ROM 后可以被锁定的方式，这很可能是 FBI 也是如何将 ArcaneOS 加载到他们卖给犯罪分子的 Pixel 手机上的。

在弄清楚 XDA 的用户实际上手上拿着一个镇纸之后，他们当然[扔掉了它](https://forum.xda-developers.com/t/is-it-bricked-cannot-flash-stock-android-to-remove-arcaneos.4285827/page-2#post-85210151)。他们没有说它最终去了哪里，但很可能这就是最近 *[副](https://www.vice.com/amp/en/article/n7b4gg/anom-phone-arcaneos-fbi-backdoor)* 拿到的同一部手机。Vice 的团队发现了手机软件背后的真相:这是一部 FBI 卖给罪犯的手机，这样他们就可以记录他们的通信，作为犯罪活动的证据。

 <picture>![Anom app on a Pixel 4a.](img/b14f1ebc8a1f06d74d83376e0747ba06.png)</picture> 

Anom app on a Pixel 4a. Credits: Vice.

使用普通 PIN 码解锁手机会显示一些普通应用，如 Tinder、网飞和脸书，但当你点击它们的图标时，没有一个应用会真正打开。然而，用不同的 PIN 码解锁 Pixel 手机会显示时钟应用程序、计算器应用程序和设备设置的图标。然而，点击计算器图标实际上并不会打开计算器应用程序。相反，它打开了 ANOM 服务的登录界面，这是一种由联邦调查局秘密运营的“加密”信息服务。在 [ANOM 的存在被披露](https://www.europol.europa.eu/newsroom/news/800-criminals-arrested-in-biggest-ever-law-enforcement-operation-against-encrypted-communication)后，犯罪分子迅速寻求处理掉他们的设备，这很可能就是这位不幸的 XDA 用户以如此便宜的价格得到 Pixel 4a 的原因。

关于联邦调查局蜜罐行动和 ANOM 服务的更多细节，我推荐阅读 *Vice* 的[关于这个话题的精彩报道](https://www.vice.com/en/article/m7e733/anom-fbi-andrew-young-encryption-honeypot)。