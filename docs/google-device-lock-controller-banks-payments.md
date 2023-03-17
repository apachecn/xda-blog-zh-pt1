# 如果你拖欠还款，这个应用程序可以让银行锁定你的手机

> 原文：<https://www.xda-developers.com/google-device-lock-controller-banks-payments/>

**更新 1(美国东部时间 11/06/2020 @ 06:05PM):**谷歌已经发布了关于设备锁定控制器应用程序的更多细节。[点击这里了解更多信息。](#update1)今天早些时候发表的原文保留在下面。

旗舰智能手机在过去几年里变得越来越贵，因此许多原始设备制造商和运营商提供支付计划，让消费者可以选择在 24 个月或更长时间内每月支付一小部分价格。但是，如果发生了意想不到的事情，你一两个月都无法付款，你该怎么办？

嗯，当你拖欠设备付款计划时会发生什么取决于向你发放贷款的公司。例如，在美国的威瑞森，[让你有机会](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU30536/https://www.verizon.com/support/promise-to-pay-faqs/)在去收款并关闭网络接入之前设置支付安排，而三星印度[则根据债务尚未偿还的时间限制设备功能](https://images.samsung.com/is/content/samsung/p5/in/microsite/finance-plus/online/samsung-finance-plus-faqs.pdf?q=12)。看起来，谷歌希望让银行或其他信贷提供商更容易实施后一种收债方法。

今天早些时候，我们在谷歌 Play 商店上发现了一款名为“设备锁定控制器”(h/t @ [JasonBayton](https://twitter.com/JasonBayton) )的应用。以下是该应用在 Google Play 上的描述:

> #### 设备锁定控制器支持信用提供者的设备管理。如果您不付款，提供商可以远程限制对您设备的访问。如果您的设备受到限制，基本功能(如紧急呼叫和访问设置)仍将可用。

这款应用利用了安卓的

[DeviceAdminService API](https://developer.android.com/reference/android/app/admin/DeviceAdminService)

远程控制设备功能。企业使用这个 API 来控制员工可以用他们的工作电话做什么。向员工分发手机的公司通常会预装使用这种 API 的应用程序，因此没有办法禁用它们。据推测，银行或其他金融机构等信贷提供商可以在将设备借给客户之前预装谷歌的设备锁定控制器应用程序，如果客户无法付款，他们可以远程锁定他们的手机。

当你搜索 Google Play 或在 Play Store 登录页面[中查找所有由 Google](https://play.google.com/store/apps/collection/cluster?clp=igM4ChkKEzU3MDAzMTM2MTg3ODYxNzc3MDUQCBgDEhkKEzU3MDAzMTM2MTg3ODYxNzc3MDUQCBgDGAA%3D:S:ANO1ljLC8CY&gsr=CjuKAzgKGQoTNTcwMDMxMzYxODc4NjE3NzcwNRAIGAMSGQoTNTcwMDMxMzYxODc4NjE3NzcwNRAIGAMYAA%3D%3D:S:ANO1ljKF24s) 制作的应用时，设备锁控制器应用并未出现。然而，这个应用程序的开发者显然是谷歌，所以我们联系了该公司进行评论，但在这篇文章发表之前还没有得到回复。

我对这个应用的感觉是复杂的，但大多数是负面的。我理解债权人在提供贷款时承担了风险，但我认为禁用大多数功能会适得其反。智能手机是数百万人的主要计算设备，尤其是对于那些买不起个人电脑和家庭互联网的人。当然，设备锁定控制器应用程序仍然可以让你拨打和接听电话，但如今很多业务都是通过互联网进行的，保持联系真的很重要。

## 更新 1:来自谷歌的澄清

谷歌的一位发言人出面澄清了关于设备锁定控制器应用程序的一些细节。首先，谷歌表示，他们与一家名为 [Safaricom](https://www.safaricom.co.ke/) 的肯尼亚运营商合作推出了这款应用。在一篇日期为 2020 年 7 月 28 日的博客文章中，题为“[越来越多的可负担得起的智能手机](https://africa.googleblog.com/2020/07/growing-access-and-inclusion-with-more.html?m=1)”的文章中，谷歌谈到了 Safaricom 新推出的“Lipa Mdogo Mdogo”(“逐位支付”)融资计划，该计划允许肯尼亚人以可负担的分期付款方式购买新的 Android Go 版智能手机。在 [Safaricom 关于这项融资计划的 FAQ 页面](https://www.safaricom.co.ke/faqs/faq/750)上，运营商表示，在 4 天不付款后，他们将“锁定设备”。

但是这款应用在谷歌 Play 商店上安静的出现又如何呢？显然，那只是个错误。谷歌已经确认，设备锁定控制器应用程序不应在美国谷歌 Play 商店上市，他们将努力撤销上市。我们已经联系了谷歌，以澄清该公司是否有计划在未来与更多的运营商或金融机构合作，如果我们得到回复，我们将更新这篇文章。