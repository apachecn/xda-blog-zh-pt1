# 谷歌在 Pixel 5 和 Pixel 4a 5G 中启用了 DSDS 支持

> 原文：<https://www.xda-developers.com/google-will-enable-dsds-support-with-5g-in-a-future-update-for-the-pixel-5-and-pixel-4a-5g/>

**更新 1(03/03/2021 @ 08:39PM ET):**2021 年 3 月的更新在 Pixel 4a 5G 和 Pixel 5 上启用了双 SIM、双待机支持。[点击这里了解更多信息。](#update1)下面保留了 2020 年 11 月 10 日发表的文章。

Pixel 5 和 Pixel 4a 5G 的一个更被低估的功能是支持双卡双待(DSDS)。该功能允许用户使用两个 SIM(一个物理 sim 和一个 eSIM)通过一个运营商打电话和发短信，而在另一个运营商只使用数据。不幸的是，当两个 sim 卡都启用时，这些设备仅限于 4G 网络，但这显然即将改变。

谷歌自己的[支持页面](https://support.google.com/pixelphone/answer/9449293?hl=en)解释说，Pixel 4a 5G 和 Pixel 5 只有在两种 sim 都提供的情况下才支持 4G 连接。

> 重要提示:使用两个 sim 卡的 Pixel 5 和 Pixel 4a (5G)手机将退回到 4G 网络。要连接到 5G 网络，请暂时关闭未设置为使用数据的 SIM 卡。

然而，Android 开源项目(AOSP)发布的代码变更[表明谷歌正在配置这两款设备以支持 DSDS 和 5G 网络。AOSP 是开源的，允许所有开发者的贡献，但变化来自谷歌自己的团队，并已被合并。](https://android-review.googlesource.com/c/device/google/redbull/+/1493217)

提交描述具体指的是更改“Bramble”的设备配置，这是 Pixel 4a 5G 的代号。然而，正在更改的代码位于“Redbull”的设备树下，这是 Pixel 5(代号“Redfin”)和 Pixel 4a 5G 的共享设备树的代号。因此，很可能这两款设备都将支持 DSDS 和 5G 网络，只要这种变化最终出现在公共版本中。

这个提交是刚刚合并的，所以我们不知道具体什么时候会在 Pixel 5 和 Pixel 4a 5G 上启用。但当谷歌在 12 月推出安全更新时，这种情况可能会发生。

**[谷歌 Pixel 4a 5G 论坛](https://forum.xda-developers.com/pixel-4a-5g)**| |**|[谷歌 Pixel 5 论坛](https://forum.xda-developers.com/pixel-5)**

自 Pixel 3a 以来，谷歌设备一直支持 DSDS 功能。但同时支持 DSDS 和 5G 网络将是该公司的新领域。

*感谢 XDA 公认的开发者 [luca020400](https://forum.xda-developers.com/member.php?u=5778309) 的提示！*

* * *

## 2021 年 3 月更新 1: 5G DSDS 支持像素功能下降

周一，谷歌推出了对其支持的 Pixel 手机的更新，带来了 2021 年 3 月的安全补丁级别和 T2 最新的 Pixel 功能。他们没有告诉任何人的是，当其中一个提供的 SIM 卡连接到 5G 网络时，更新还支持双 SIM 卡，双待机(DSDS)(H/T Reddit 用户 [rinsf](https://www.reddit.com/r/GooglePixel/comments/lwfchk/as_of_march_feature_drop_5g_works_with_dsds/) )。这意味着你最终可以使用一个 SIM 卡连接到 5G 网络，而不必禁用另一个 SIM 卡。我们一直在等待这一变化的发生，当我们在 10 月份发现该功能的提交时，它终于在最近的更新中出现了。