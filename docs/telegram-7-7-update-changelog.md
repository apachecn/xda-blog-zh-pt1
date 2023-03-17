# Telegram 扩展了支付支持，增加了预定的语音聊天等等

> 原文：<https://www.xda-developers.com/telegram-7-7-update-changelog/>

Telegram 是一个受欢迎的移动通讯平台，在脸书宣布将对其 WhatsApp messenger 做出[改变后，该应用的用户数量最近出现激增。Telegram 通常每隔几个月就会收到新功能，现在另一项更新正在推出，对支付和语音聊天进行了更改。](https://www.xda-developers.com/whatsapp-updates-terms-privacy-policy-mandate-data-sharing-facebook/)

首先，Telegram 正在推出对其支付系统的改进，允许机器人在不离开应用程序的情况下接受支付。例如，你可以和一个电报机器人交谈来订购一个比萨饼。“从今天开始，”Telegram 在一篇博客文章中说，“依靠 Stripe 等 8 个集成的第三方支付提供商，商家可以在任何聊天中天然接受信用卡支付。”该应用程序声称它不存储支付信息，也不从购买中抽取佣金。

Telegram 的新[开发者文档](https://core.telegram.org/bots/payments)列出了所有支持的支付提供商: [Stripe](https://stripe.com) ， [Yandex。Money](https://money.yandex.ru/new) ， [Sberbank](https://www.sberbank.ru) ， [Tranzzo](https://tranzzo.com) ， [Payme](https://payme.uz/) ， [CLICK](http://click.uz/) ， [LiqPay](https://www.liqpay.ua/uk/) ，以及 [ECOMMPAY](https://ecommpay.com/) 。Telegram 还支持 Apple Pay 和 Google Pay，具体取决于应用运行的平台。主要的问题是，机器人不允许接受 iOS 用户的数字商品和服务的支付，因为苹果公司硬性要求所有数字购买都使用其自己的支付平台(从卖家那里收取 15-30%)。谷歌*在技术上*对来自 Play Store 的应用程序也有同样的规定，但该公司直到今年 9 月才会开始严格执行这一要求。

支付文档还列出了所有支持的货币，包括美元(USD)、英镑(GPB)、日元(JPY)、俄罗斯卢布(RUB)和许多其他货币。没有受支持的加密货币——这是一个有趣的举动，因为许多其他 [应用](https://www.xda-developers.com/signal-testing-privacy-focused-payments-feature/)都在双倍押注比特币和其他完全数字化的货币。不过，考虑到比特币开采带来的[能源需求上升对环境的危害，Telegram 的这一举措并不坏。](https://www.bbc.com/news/technology-56012952)

Telegram 的更新还增加了为未来安排语音聊天的功能，类似于在微软团队和 Slack 等服务中安排会议。安排聊天时会显示倒计时钟，聊天开始时，群组中的任何人都可以收到推送通知。Telegram 还推出了两个实验性的网络应用，一个是捏放照片，一个是改进的视频播放器。