# 华硕 ROG 手机 5 bootloader 解锁工具及内核源代码

> 原文：<https://www.xda-developers.com/asus-rog-phone-5-bootloader-unlock-tool-kernel-source/>

华硕 ROG 手机 5 现已正式发售，评论铺天盖地，[包括我们自己的](https://www.xda-developers.com/asus-rog-phone-5-review/)。这款设备具有令人难以置信的魅力，例如 6.78 英寸 FHD+ AMOLED 显示屏和骁龙 888 SoC，高达 18GB 的 LPDDR5 RAM 和 512GB 的 UFS 3.1 存储空间(在“终极”版本上)，双 3000 毫安时电池和 3.5 毫米耳机插孔。华硕对售后市场发展的友好历史往往会导致我们论坛上活动的繁荣。我们希望最新的 ROG 手机也是如此，但只有时间才能证明改装场景是否会在手机上出现。为了方便定制开发，华硕现在已经发布了 ROG 手机 5 的引导加载器解锁工具和内核源代码。

**[华硕 ROG 手机 5 XDA 论坛](https://forum.xda-developers.com/f/asus-rog-phone-5.12119/)**

现在，当然每一个销售 Android 设备的智能手机制造商都有义务发布他们的内核源代码，因为 Linux 内核是根据 GNU 通用公共许可证版本 2 授权的。但是正如我们中的一些人所知道的，许多 OEM 厂商出于各种原因推迟发布他们的内核源代码。然而，华硕的目标是尽快发布它们。ROG 手机 3 [在去年发布的同一周内发布了其内核源代码。很高兴看到该公司在 ROG 手机 5 上也延续了这一趋势。](https://www.xda-developers.com/asus-rog-phone-3-bootloader-unlock-tool-firmware-kernel-sources-release/)

至于 bootloader 解锁，ROG 手机 5 上的 bootloader 可以通过华硕提供的一个应用程序解锁。不过，你需要记住的是，解锁手机上的引导加载程序会使设备保修失效，还会禁用 OTA 更新。此外，请注意，您需要从您的设备本身运行解锁应用程序，解锁引导加载程序会强制恢复出厂设置。

**[华硕 ROG 手机 5: Bootloader 解锁工具&内核来源](https://www.asus.com/supportonly/ROG%20Phone%205%20(ZS673KS)/HelpDesk_Download/)**

我们为华硕及时发布 ROG 手机 5 的引导程序解锁工具和内核源代码而喝彩。如果没有它们，开发定制的基于 AOSP 的 rom(如 LineageOS)将非常困难，如果不是不可能的话。内核源代码对于正确构建可用的 TWRP 也是必要的。既然源代码已经可用，开发论坛在不久的将来应该会有更多的活动，对于那些想要从华硕的 ROG UI 和 ZenUI 皮肤迁移的用户来说，可能会有更好的选择。