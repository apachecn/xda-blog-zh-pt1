# 不只是你:脸书、Messenger、Instagram 和 Whatsapp 都瘫痪了

> 原文：<https://www.xda-developers.com/facebook-messenger-instagram-whatsapp-outage/>

**更新 4(10/04/2021 @ 06:56PM ET):**WhatsApp 也终于上线了。[点击这里了解更多信息。今天早些时候发表的这篇文章保留在下面。](#update4)

### 以前的更新

**更新 3(10/04/2021 @ 06:06PM ET):**insta gram 和 Facebook Messenger 又开始工作了，尽管 WhatsApp 似乎仍然存在问题。[点击这里了解更多信息。](#update3)

更新 2 (10/04/2021 @ 05:45 PM ET): 脸书正慢慢开始显示出生机，尽管并非所有服务都已完全恢复。[点击这里了解更多信息。](#update2)

**更新 1 (10/04/2021 @ 1:47 PM ET):** 脸书已经承认它的所有服务都关闭了，一份报告揭示了为什么它们似乎离线。[点击这里了解更多信息。](#update1)

今天早上，美洲、欧洲和亚洲的脸书服务被中断，导致脸书本身、Facebook Messenger 及其姐妹服务 Instagram 和 WhatsApp 的用户在试图访问任何操作系统上的任何网站和服务时，都会抛出错误信息。该问题可能与 DNS 有关，因为没有一个域返回 IP。断电也影响了提供脸书登录的服务，比如 Pokemon Go。

脸书尚未公开评论影响其所有服务的持续中断。就连[脸书职场服务状态](https://www.workplace.com/status)此时也无法访问。随着我们了解更多，我们一定会更新这个故事。

[Down Detector](https://downdetector.com/) 显示，在美国东部时间今天 11:30 左右，所有四个服务的报告都出现了巨大的峰值。

在撰写本文时，脸书还没有承认在其任何社交媒体页面上存在该问题，因此，我们没有关于预期持续时间原因的信息。

我们将密切关注此次脸书停电事件，并在有进一步消息时通知您。

* * *

## 更新 1:脸书、WhatsApp 和 Instagram 承认宕机，新信息说明原因

[脸书](https://twitter.com/facebookapp/status/1445060225468297216?s=19)、 [WhatsApp](https://twitter.com/whatsapp/status/1445060216161116168?s=21) 和 [Instagram](https://twitter.com/InstagramComms/status/1445062531932835841) 的官方推特账号已经承认他们的服务已经被黑了。据记者 Brian Krebs 称，所有这些服务关闭的原因是，告诉系统如何导航到这些服务的 DNS 记录已经从全球路由表中删除。为什么会这样还不知道，因为脸书应该控制自己的 DNS 记录。

* * *

## 更新 2:脸书显示生命迹象

脸书的部分地区正在慢慢恢复供电。该公司的[新闻编辑室恢复了](https://about.fb.com/news/)，我们能够看到 [XDA 脸书的页面](https://www.facebook.com/xda.developers/)。然而，目前事情进展非常缓慢，Instagram 和 WhatsApp 等其他服务似乎仍处于关闭状态。我们将继续关注这一情况，并会在服务恢复后尽快更新这篇文章。

* * *

## 更新 3: Instagram 和 Messenger 重新上线

几个小时后，脸书恢复了更多的核心服务。主网站看起来对许多人来说还在运行，T2 的 Instagram 和 Messenger 也恢复了。然而，WhatsApp 似乎仍然存在问题，尽管我们已经看到一些用户断断续续地回来了。

对于那些想知道发生了什么的人来说，[这篇来自 Cloudflare](https://blog.cloudflare.com/october-2021-facebook-outage/) 的博客文章很好地解释了脸书是如何从互联网上消失的。要找出导致这种情况的确切原因，我们必须等待公司自己对这一问题的内部调查。然而，网络安全记者布莱恩·克雷布斯(Brian Krebs)报道称，该问题源于“一次例行的 BGP 更新出错”，因为该更新“阻止了远程用户恢复更改”，而具有物理访问权限的人“没有网络/逻辑访问权限”来恢复它。

* * *

## 更新 4: WhatsApp 重新上线

世界各地的许多用户都报告说 WhatsApp 重新上线了，消息也终于传了出去。我们可以确认 XDA 门户网站的一些员工已经恢复了服务，但是该公司还没有宣布其服务已经完全正常。您所在地区的服务可能需要几分钟才能恢复，所以请继续检查！