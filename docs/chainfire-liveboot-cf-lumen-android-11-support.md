# Chainfire 的 LiveBoot 应用程序现在已经开源，可以在 Android 11 上运行

> 原文：<https://www.xda-developers.com/chainfire-liveboot-cf-lumen-android-11-support/>

# Chainfire 的 LiveBoot 应用程序现在已经开源，可以在 Android 11 上运行

Chainfire 已经更新了他的 LiveBoot 和 CF.lumen 应用程序，支持 Android 11。而且，LiveBoot 现在已经完全开源了。

我们已经在过去的中讨论过 LiveBoot，以及它如何通过添加 logcat 和 dmesg 日志来调整 Android 设备的默认启动动画(带来了老式的 Matrix digital rain vibe)。不是别人，正是 XDA 传奇人物 [Chainfire](https://forum.xda-developers.com/m/chainfire.631273/) 、 [SuperSU](https://forum.xda-developers.com/f/supersu.3522/) 的创造者，这个令人难以置信的创新应用在短暂中断后，现在获得了新的更新。此次更新将应用版本提升至 1.84，并最终兼容 Android 11。

除了增加对 Android 11 的支持，Chainfire 还将 LiveBoot 完全开源，包括它使用的名为 [libCFSurface](https://github.com/Chainfire/libcfsurface) 的低级库。该库允许以 root 用户身份直接访问 SurfaceFlinger，当 Android 本身没有完全加载时，这对于获取屏幕上的任何内容可能是有用的。

如果您有兴趣在您的设备上试用该应用程序，您可以从谷歌 Play 商店下载更新版本，或者从下面链接的应用程序线程中抓取 APK 进行手动侧装。如果你想看看代码库并玩玩它，你可以访问这个项目的 GitHub 库。

**[LiveBoot XDA Thread](https://forum.xda-developers.com/t/app-5-0-root-2020-12-21-liveboot-logcat-dmesg-boot-animation-v1-84.2976189/)**

[appbox googleplay "我. chaifire . live boot "]

Chainfire 的另一个受欢迎的应用程序叫做 [CF.lumen](https://www.xda-developers.com/cf-lumen-resurrected-as-new-app-brings-kitkat-support/) ，它也刚刚获得了版本号为 3.74 的新更新，以增加对 Android 11 的支持。对于那些不熟悉 CF.lumen 的人来说，它可以根据太阳的位置或根据您的自定义配置来调整您的 Android 设备上的颜色。然而，根据开发者的说法，目前只有 CF.lumen 的兼容模式驱动程序可以在 Android 11 下工作，只有 root-only 模式也是如此。

以下是 CF.lumen v3.74 的官方变更日志:

*   2020 年
*   删除对 G+的引用
*   Android 11 支持
*   Android 10+:显示通知选项不起作用的警告
*   Android 10+:禁用无根模式
*   Android 10+:禁用高级/注入/防闪烁/性能驱动程序(需要进一步调查才能工作)
*   添加前台服务权限
*   为 API 29 建造
*   修复垃圾通知问题
*   修复地图崩溃

**[CF.lumen XDA 线程](https://forum.xda-developers.com/t/app-5-0-2020-12-22-cf-lumen-v3-74.2711912/)**【app box Google play " eu . chain fire . lumen "】