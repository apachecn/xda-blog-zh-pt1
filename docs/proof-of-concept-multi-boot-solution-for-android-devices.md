# 开发人员为 Android 设备制作了一个多启动解决方案的概念验证

> 原文：<https://www.xda-developers.com/proof-of-concept-multi-boot-solution-for-android-devices/>

Android 设备上的多重引导总是有点棘手。在普通的 x86 PCs 和 MAC 上，很容易启动另一个操作系统。然而，在智能手机上，情况就不同了。幸运的是，优秀的售后开发者社区以及个人改装者经常想出不同的方法来让你的 Android 设备同时运行两个 ROMs 甚至多个不同的操作系统。

当提到 Android 上的多重引导时，由 XDA 知名开发者 [Tasssadar](https://forum.xda-developers.com/m/tasssadar.3418703/) 开发的 **MultiROM** 是首先想到的项目之一。我们也有**安全带**和**双靴修补器**，前者[仍然保留了几个忠实的追随者](https://www.xda-developers.com/samsung-galaxy-s9-galaxy-note-9-snapdragon-root/)。最近，TWRP 本身已经成为另一个创建多重引导解决方案的优秀平台。现在，XDA 知名开发者 phhusson 已经开始展示他的 AOSP GSI 和三星 Galaxy A71 上的 stock One UI ROM 之间的双启动解决方案。

Pierre-Hugues 休松，即“phhusson”别名背后的人，可能最出名的是他的项目高音 GSI，但他也研究了许多不同的工具和项目，从非常有用到非常有趣的 T2。前面提到的多重引导项目就是这样一个例子。它被称为“引导分流器”，当前的实施需要最终用户按下音量摇杆来选择他们想要引导的操作系统。

据开发商称，装载机“...位于 boot.img 和 system 之间，可以引导未修改的股票和 GSI。这使得它比谷歌的 DSU 装载机更加通用。辅助操作系统可以存储在 SD 卡上，这在便携性方面也是一大优势。截至目前，它还不能在启动时切换内核，但该解决方案的 SoC 不可知结构允许它在基于 Exynos、高通和联发科芯片组的设备上工作，而不依赖于平台特定的代码。

如果 Android 是关于开放性的，那么多重引导为这个想法增加了一个全新的维度。对于闪存爱好者来说，启动多个操作系统的能力提供了一个机会，可以安全地试用新的 rom 或测试某些 mod，而不会危及日常驱动程序的完整性。本着这种精神，如果你想看看 phhusson 的 boot-diverter 项目，你可以在这里找到它的 GitHub 库。请记住，现成的二进制文件尚未发布，因此您需要自己调整代码并编译。