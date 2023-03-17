# 新的 Android 11 设备可能不支持无缝更新的虚拟 A/B

> 原文：<https://www.xda-developers.com/google-virtual-ab-seamless-updates-android-11/>

**更新 1 (01/25/2021 @美国东部时间下午 2:06):**在 Android 11 发布之前，谷歌似乎在要求启动设备支持虚拟 A/B 方面出了问题。[点击这里了解更多信息。](#update1)下面保留了 2021 年 4 月 7 日发表的文章。

在 Android 7.0 牛轧糖中，谷歌引入了一种旨在加快软件更新速度的分区方案。在 Nougat 中，Google 增加了对复制某些分区的支持，这样非活动分区可以在后台更新，然后通过快速重启切换到活动分区。这种[“A/B 分区”设置允许在受支持的 Android 设备上进行“无缝更新”](https://www.xda-developers.com/how-a-b-partitions-and-seamless-updates-affect-custom-development-on-xda/)，很像谷歌的 Chrome 操作系统。然而，谷歌从未强制要求使用 A/B 分区，所以很多设备都不支持无缝更新。然而，随着 Android 11 的推出，这种情况可能会发生变化，因为谷歌正在强制新推出的设备支持虚拟 A/B 分区。

作为一点背景知识，A/B 分区指的是一组重复的只读分区。复制的分区通常包括系统、供应商、引导和产品分区。当手机下载更新时，更新程序会在后台修补不活动的分区集(一个“插槽”)。一旦更新应用到非活动插槽后，系统会提示用户重启设备。当用户重新启动设备时，非活动插槽与活动插槽交换位置，完成更新过程。如果引导新更新的插槽出现问题，则先前活动的插槽保持不变。当下一次更新开始时，这个过程会重复进行。如果你对更技术性的解释感兴趣，[参考 Google 关于 A/B 分区的开发者文档](https://source.android.com/devices/tech/ota/ab)。

相比之下，没有 A/B 分区的设备，如三星 Galaxy S20、OPPO Find X2 和许多其他设备，在恢复过程中通过专用的更新程序应用更新。这将用户踢出 Android，并使他们在几分钟内无法使用他们的设备，可能会错过重要的通知、电话或短信。谷歌认为，简化更新过程会导致更多的人在更新推出后真正接受更新；事实上，在 2017 年 5 月，[谷歌发现](https://source.android.com/devices/tech/ota/ab/ab_faqs)Pixel 用户运行最新安全更新的比例高于 Nexus 用户。当然，用户可以安排在不使用设备的时候进行更新，但是许多用户甚至在被提示的时候也不更新他们的设备。此外，由于没有 A/B 分区，用户错过了一个固有的好处:保护他们免受拙劣的系统更新。

例如，当小米[首次为 Mi A2 Lite 推出 Android 10 更新](https://www.xda-developers.com/download-xiaomi-mi-a2-lite-official-android-10-update-sideload/)时，许多用户发现他们的设备无法启动。对他们来说幸运的是，Mi A2 Lite 有 A/B 分区用于无缝更新，所以我们论坛上的[用户发现](https://forum.xda-developers.com/showpost.php?p=81973955&postcount=184)他们可以使用 fastboot 命令来设置引导加载程序，以引导未触及的、先前活动的分区集。因此，A/B 分区不仅为用户提供了更快的更新过程，而且它们还充当了拙劣更新的故障保险。没有实现 A/B 分区的 OEM 仍然可以设计他们自己的方法来防止 OTA 故障，尽管当这种保护是 A/B 分区设计的一部分时，为什么要经历这种麻烦呢？为了你的参考，这里有一个部分(当然也是过时的)[支持 A/B 分区](https://www.xda-developers.com/list-android-devices-seamless-updates/)进行无缝更新的设备列表，这里有一个关于[如何检查你自己的设备是否支持功能](https://www.xda-developers.com/how-to-check-android-device-supports-seamless-updates/)的教程。

似乎令人费解的是，为什么像三星这样的原始设备制造商对一部智能手机要价 1400 美元，却不提供如此漂亮的功能。原因通常归结为存储:原始设备制造商不想牺牲几千兆字节的存储空间来支持无缝更新。像三星 Galaxy S20 这样的手机有大量的预装软件，所以复制/system 和/product 这样的分区会导致大量巨大的文件和应用程序被复制。谷歌设法实现了 A/B 分区，而没有牺牲太多的存储空间[,这要归功于一个巧妙的技巧](https://source.android.com/devices/tech/ota/ab/ab_faqs#how-did-you-halve-the-size-of-the-system-partition-without-squashfs)来解决复制海量数据的问题。odex 文件。原始设备制造商可能选择不实现 A/B 分区的另一个原因是成本:跟上谷歌对 Android 分区方案的不断变化需要很多努力，正如 XDA 公认的开发者 [topjohnwu](https://forum.xda-developers.com/member.php?u=4470081) 将告诉你的那样。除非原始设备制造商被迫这样做，否则许多人不会费事去改变已经对他们起作用的东西。

不过，最后，谷歌似乎要在 Android 11 中制定法律。通过在新推出的设备上强制采用虚拟 A/B 分区，他们几乎可以肯定 OEM 将必须支持其 2020 年底和 2021 年设备的无缝更新。正如 XDA 知名开发者 [luca020400](https://forum.xda-developers.com/member.php?u=5778309) 所发现的，谷歌 Treble 项目团队的软件工程师 Yifan Hong 向 Gerrit 提交了一份名为“[在 R 发布](https://android-review.googlesource.com/c/platform/test/vts-testcase/kernel/+/1280636)时要求虚拟 A/B”的承诺该提交更新了供应商测试套件(VTS ),这是一项自动化测试，所有设备都必须通过才能被视为与 Project Treble 兼容。新的测试检查系统属性“`ro.virtual_ab.enabled`”是否设置为 true，以及“`ro.virtual_ab.retrofit`”是否设置为 false(对于出厂 API 级别为 30 或更高的设备)。换句话说，该测试检查使用 Android 11 或更高版本启动的设备是否支持虚拟 A/B 分区。Android 10 引入了“虚拟”A/B 分区和“动态分区”，后者是可动态调整大小的分区。它们与常规 A/B 分区的概念相同，只是它们可以自由调整大小。

如果使用 Android 11 启动的设备不支持虚拟 A/B 分区，那么它将无法通过 VTS。如果设备未能通过 VTS，则不能使用谷歌移动服务。换句话说，Google 已经有效地要求 OEM 支持虚拟 A/B 分区，并通过扩展实现无缝更新。

* * *

## 更新:Android 11 不需要虚拟 A/B

当我们在 4 月份首次报道谷歌要求所有 Android 11 发布设备支持[虚拟 A/B 更新机制](https://source.android.com/devices/tech/ota/virtual_ab)时，人们非常兴奋，因为这将最终使三星手机实现无缝更新。不幸的是，事实证明 Google 决定不将虚拟 A/B 支持作为一项要求。Android 11 的[兼容性定义文档](https://source.android.com/compatibility/android-cdd#11_updatable_software) (CDD)目前写着“设备实现应该支持 A/B 系统更新”而不是“必须”支持。似乎在 Android 11 发布之前的某个时候，谷歌决定收回其要求虚拟 A/B 支持的决定，可能是在几家原始设备制造商的要求下。这种情况经常发生，但从未向公众传达，因为只有 CDD 的最终草案在网上公布。