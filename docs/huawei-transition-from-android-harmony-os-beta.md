# 鸿蒙系统 2.0 现已在华为智能手机的开发者测试版中推出，从 Android 过渡而来

> 原文：<https://www.xda-developers.com/huawei-transition-from-android-harmony-os-beta/>

当我们谈论移动操作系统时，今天只有两种主要的解决方案:Android 和 iOS。苹果对 iOS 的严格控制意味着 Android 是 OEM 厂商构建自己的智能手机的唯一真正的解决方案。尽管 Android 是开源的，但它也非常依赖于谷歌，这要归功于谷歌对 GMS 的掌控以及围绕 GMS 框架的相互依赖的整个生态系统。华为经历了这一艰难的过程，自从美国商务部将其列入实体名单，切断了该公司获得新的 GMS 许可协议的机会以来，形势对其不利。没有谷歌的帮助，这条路是艰难的，但华为带着自己的 HMS 解决方案艰难前行。然而，这家中国科技巨头远未放弃其智能手机业务，它现在开始从无 GMS 的安卓系统向自己的第一方操作系统[鸿蒙系统](https://www.xda-developers.com/harmony-os-huawei-announce/)进行长期过渡。

一年半前，鸿蒙系统正式亮相，该公司展示了作为第一款采用第一方操作系统的设备的 [Honor Vision 智能电视](https://www.xda-developers.com/honor-vision-tv-huawei-harmony-os/)。在整个 2019 年，华为重申了其对 Android 的承诺，计划[将鸿蒙系统扩展到智能手机和平板电脑之外的设备](https://www.xda-developers.com/huaweis-harmony-os-coming-more-devices-next-year-not-smartphones-tablets/)。[在今年早些时候的 HDC 2020](https://www.xda-developers.com/huawei-harmony-os-smartphones-expected-beta-sdk-late-2020/) 上宣布了新的计划，但是今天，该公司已经[开始为第一个移动设备的鸿蒙系统 2.0 测试版招募开发人员](https://developer.huawei.com/consumer/cn/activity/301607581257578636)。

华为表示，鸿蒙系统 2.0 带有“超过 15，000 个 API”，以支持智能手机、可穿戴设备、汽车、更大显示屏和更多用例的开发。要测试新的操作系统，您可以从[鸿蒙系统官方网站](https://www.harmonyos.com/cn/home/)的[华为 deve co Studio IDE(2.0 Beta 3 版)](https://developer.huawei.com/consumer/cn/forum/topic/0201434973761300108?fid=0101303901040230869)中试用模拟器，或者您可以在您支持的华为设备上注册接收 OTA，以迁移到鸿蒙系统 2.0 Beta。一旦您的注册获得批准，您将收到华为的邀请，其中包含如何在您的设备上安装软件的说明。

以下设备有资格安装鸿蒙系统 2.0 开发者测试版:

*   华为 P40 (ANA-AN00)
*   华为 P40 Pro (ELS-AN00)
*   华为 Mate 30 (TAS-AL00)
*   华为 Mate 30 5G (TAS-AN00)
*   华为 Mate 30 Pro (LIO-AL00)
*   华为 Mate 30 Pro 5G (LIO-AN00)
*   华为 MatePad Pro (MRX-AL19)
*   华为 MatePad Pro 5G (MRX-W09)
*   华为 MatePad Pro Wi-Fi (MRX-AN19)

正如开发人员测试版所期望的那样，这是一个不稳定的软件，只供开发人员在平台上开始工作。因此，在升级到新操作系统之前，您绝对应该备份您的数据。有可能回滚到基于 Android 的 EMUI 11 正式版，但是回滚会预期删除所有用户数据。

一些可以访问模拟器的开发者已经在华为开发者社区发布了他们在鸿蒙系统 2.0 上运行的应用的截图样本。

乍一看，这些样本截图显示，鸿蒙系统看起来非常像华为 P40 上基于 Android 的 EMUI 11。开发者文档提到，应用程序是用 Java 编写的，布局是用 XML 文件定义的，类似于 Android。我们猜测，华为希望让 Android 应用开发者尽可能熟悉新操作系统，以便最大限度地减少迁移到新操作系统和配套生态系统的障碍。早期采用者也提到过(翻译)“ *Android 开发思想可以应用到鸿蒙(鸿蒙系统)开发，大大加快鸿蒙*的开发”，这是有道理的，尽管我们还没有挖掘新的 OS 或文档来验证这种说法有多真实。

如果您有兴趣开始使用，这里有一些有用的链接:

目前很多文档都是中文的，源代码还没有发布，所以在这方面还有相当多的探索空间。我们会随时通知你最新进展。