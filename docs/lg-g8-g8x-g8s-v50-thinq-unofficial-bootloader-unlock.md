# 为 LG G8、G8S、G8X 和 V50 ThinQ 找到了通用引导加载程序解锁方法

> 原文：<https://www.xda-developers.com/lg-g8-g8x-g8s-v50-thinq-unofficial-bootloader-unlock/>

解锁一个引导加载程序，给一个设备找根，刷新定制的 rom 是 XDA 流行的爱好。许多用户对这种能力推崇备至，如果手机不能解锁，他们几乎不会对手机感兴趣。然而，LG 在 bootloader 解锁方面有着传奇的历史——即，韩国 OEM 更喜欢允许最终用户解锁少数型号(可能是由于运营商的要求)。修改社区对 LG 的立场不满意，现在看来我们不耐烦的用户找到了一种非官方的引导加载程序解锁方法，可以应用于 LG G8 ThinQ、LG G8S ThinQ、LG G8X ThinQ 和 LG V50 ThinQ 的几乎所有版本。

**XDA 论坛:[LG G8 ThinQ](https://forum.xda-developers.com/c/lg-g8.8515/)| |[LG G8X ThinQ](https://forum.xda-developers.com/c/lg-g8x-thinq.9263/)| |[LG V50 ThinQ](https://forum.xda-developers.com/c/lg-v50-thinq.8623/)**

根据 XDA 资深会员 [cloud1250000](https://forum.xda-developers.com/m/cloud1250000.4160343/) 的意见，XDA 会员 [Seasee606](https://forum.xda-developers.com/m/seasee606.9954733/) 提出了一个真正创新的过程来解锁 LG G8/G8S/G8X 或 LG V50 ThinQ 的引导加载程序。然而，非官方的方法并不像你想象的那么简单。它利用了一个泄露的工程引导程序，需要你强制目标设备引导到高通 SoC 的紧急下载模式( [EDL](https://www.xda-developers.com/exploit-qualcomm-edl-xiaomi-oneplus-nokia/) )并执行几个低级的刷新工作。

这种方法的基本概念非常类似于用于 [Sprint LG G8 ThinQ bootloader 解锁](https://www.xda-developers.com/bootloader-unlocking-method-has-been-found-for-the-sprint-lg-g8-thinq/)过程的概念，只是最初的部分需要[利用漏洞](https://www.xda-developers.com/lg-v50-thinq-root-locked-bootloader-exploit/)获得临时 root 访问权限。简而言之，新方法不需要特定的固件，它甚至与 LG G8 的威瑞森版本兼容。工程引导加载程序本质上是将设备置于一种状态，在这种状态下，它们能够接受常规的`fastboot oem unlock`命令，而无需 LG 官方解锁服务器生成的令牌。

**[解锁 LG G8、G8X、G8S、V50 ThinQ-XDA 线程](https://forum.xda-developers.com/t/guide-lg-g8-g8x-v50-bootloader-unlock-and-magisk-root-using-firehose.4221793/)** 的 bootloader

由于这个过程有点棘手，需要通过 EDL 模式闪光，可以肯定地说，它不适合初学者，而且肯定会使保修无效。如果你想继续，一定要非常仔细地阅读帖子和开篇文章，并尽可能精确地执行步骤。