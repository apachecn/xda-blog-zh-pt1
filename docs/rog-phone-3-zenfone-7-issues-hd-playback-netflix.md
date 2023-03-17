# 华硕修复了 ROG Phone 3 和 ZenFone 7 上网飞高清播放的错误

> 原文：<https://www.xda-developers.com/rog-phone-3-zenfone-7-issues-hd-playback-netflix/>

**更新 2 (01/26/2021 @美国东部时间下午 1:40):**ROG Phone 3 现在也正在接收软件更新，以恢复网飞的高清播放。[点击这里了解更多信息。](#update2)

**更新 1 (01/22/2021 @ 04:00 PM ET):** 华硕推出了 ZenFone 7 系列的更新，据称解决了 Widevine 降级问题。[点击这里了解更多信息。](#update1)下面保留 2020 年 12 月 30 日发表的文章。

华硕 ROG Phone 3 和 ZenFone 7/7 Pro 的一些用户发现，他们的设备已经失去了 Widevine L1 的地位。因此，他们无法播放高清的网飞内容。

用户已经在华硕的论坛上表达了他们的不满。似乎这个问题已经持续了几个星期，没有消失的迹象。

Widevine 是一种 DRM 技术，被网飞和亚马逊 Prime Video 等许多流媒体服务使用，以确保这些服务被具有未经修改的安全固件的设备使用。没有 Widevine L1 状态，用户无法从网飞以 540p 以上的质量播放视频。不幸的是，由于 [ROG 手机 3 和 ZenFone 7](https://www.xda-developers.com/asus-zenfone-7-pro-rog-phone-3-update-security-patches-bug-fixes/) (两者都由高通骁龙 865 驱动)的 SoC 固件中的一个错误，Widevine DRM 级别对于少数用户来说从 L1 降级到 L3。根据华硕的说法，解决这个问题的唯一方法是受影响的用户将他们的设备运往华硕，以便他们可以重新供应。

华硕就此问题发表了一份声明:“华硕意识到这个问题影响了一小部分用户，是由我们的 SOC 供应商高通的一个错误引起的，”华硕说。"如果这种情况已经发生，我们敦促您联系华硕客户服务在您的地区."

一些用户在论坛上表示，在他们的手机修好后，这个问题又出现了。用户 yashpandya295 在华硕论坛上说:“在服务中心解决了我的问题后，我又遇到了这个问题，但今天这个问题又发生了。”。"所以我不得不再次拜访服务中心."

值得的是，我们检查了我们的 ROG Phone 3 和 ZenFone 7 审查单位，我们的 Widevine 级别没有被降级。要检查您自己的 Widevine DRM 级别，[下载 DRM 信息应用程序](https://play.google.com/store/apps/details?id=com.androidfung.drminfo)。

**[ROG 手机 3 论坛](https://forum.xda-developers.com/c/asus-rog-phone-3.11025/)**| |**|[华硕 ZenFone 7 论坛](https://forum.xda-developers.com/c/asus-zenfone-7-7-pro.11393/)**

* * *

## 更新 1:华硕 ZenFone 7 的潜在修复

在告知我们解决 Widevine 降级问题的唯一方法是将您的设备运送到服务中心后，华硕现在正在推出 ZenFone 7 系列的更新，据称该更新可以修复该问题。29.14.53.23 软件版本将在全球推出，发布说明如下:

1.  Android 安全补丁更新至 2021 年 1 月 5 日
2.  改进的触摸稳定性
3.  在 Telia 上启用 Volte(LT)
4.  修复了 Widevine 降级到 L3 的问题

由于我们自己的单位没有面临这个问题，我们不能确认更新是否解决了受影响单位的问题。然而，由于这个问题据称是由高通固件中的一个错误引起的，因此认为它可以通过软件更新来修复是合理的。我们还没有发现 ROG Phone 3 有类似的更新，但是一旦有了，我们会让你知道的。如果你的 ZenFone 7 的 Widevine 级别降级到 L3，而这次更新又为你把它升级到 L1，请在下面的评论中告诉我们！

* * *

## 更新 2:修复 ROG 电话 3

华硕[宣布](https://zentalk.asus.com/en/discussion/43949/210125-rog-phone-3-zs661ks-ww-17-0823-2012-131)ROG 手机 3 的软件更新版本 17.0823.2012.131。此更新将随着以下发行说明在全球范围内推出:

1.  改进了耳机模式下通话时听不到声音的问题
2.  修正了网飞高清电影不能播放的问题

似乎华硕设法恢复了 Widevine keybox，它通常用工厂提供的设备特有的密钥加密。这是一个好消息，因为这意味着网飞高清播放可以恢复，而无需将设备送回华硕。如果更新为您解决了问题，请告诉我们！