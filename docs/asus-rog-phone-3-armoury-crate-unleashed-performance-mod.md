# 使用此模式自定义 ROG 手机在任何应用程序中的性能

> 原文：<https://www.xda-developers.com/asus-rog-phone-3-armoury-crate-unleashed-performance-mod/>

**更新 1 (04/11/2021 @ 02:56 PM ET):** 军械库板条箱未出租 mod 已经移植到华硕 ROG Phone II。[点击这里了解更多信息。](#update1)文章发表于 2021 年 3 月 21 日，下面保留。

Magisk 模块是一种将系统级 mod 应用到您的设备的简单方法，而无需手动修改系统文件。从最终用户的角度来看，您所要做的就是下载一个模块，通过 [Magisk 应用](https://www.xda-developers.com/magisk-v22-release-samsung-galaxy-s21-support/)启用它，然后重启您的设备以使更改生效。虽然大多数模块侧重于在您的设备上添加一项功能或更改一项内容，但也有一些模块针对特定的设备或固件。XDA 知名开发商 [Freak07](https://forum.xda-developers.com/m/freak07.3428502/) 的《Armoury Crate - Unleashed》就属于后一类，因为它为华硕 ROG 手机 3 上的 Armoury Crate 应用程序引入了过多的调整和修改。

**[华硕 ROG 手机 3 论坛](https://forum.xda-developers.com/c/asus-rog-phone-3.11025/)**

对于那些不熟悉 Armoury Crate 的人来说，华硕[将](https://www.asus.com/us/support/FAQ/1040544/)描述为“所有信息的中心，并通过你的手机控制你的游戏需求。”对于您添加到 Armoury Crate 游戏库中的每个游戏，您可以自定义游戏启动时激活的性能模式。令人惊讶的是，在调整系统变量方面，您可以获得真正的粒度，因为用户可以访问和修改内核公开的几乎每个 CPU 参数。如果你感兴趣的话，我们会在[我们的 ROG 手机 3 评论](https://www.xda-developers.com/asus-rog-phone-3-review/)中进行更详细的介绍。

 <picture>![ROG Phone 3 X-Mode](img/8450e0f00063afc160a1eaa7ec534d32.png)</picture> 

Armoury Crate’s Hardcore Tuning section

虽然也可以在 Armoury Crate 下添加常规应用程序，但不能保证调谐模块能达到您的要求。这是因为 Armoury Crate 下包含了一个应用程序，这使得必须执行双击才能触发后退手势，这实际上与 home 手势相冲突。因此，如果不执行两次这个动作，你就不能触发 home 手势——这在日常使用中很不方便。这正是军械库板条箱释放 Magisk 模块的用武之地。

该模块可以实时修改 ROG Phone 3 固件的各个部分，并允许您将非游戏应用程序添加到 Armoury Crate，而不用担心与导航手势冲突。你也可以添加系统应用程序，比如谷歌地图，尽管在尝试这样做之前，你需要先[无系统地移除工厂安装的副本](https://forum.xda-developers.com/t/module-terminal-debloater-v17-3-2-debloat-systemlessly.3584163/)，并从谷歌 Play 商店重新安装应用程序。国防部还通过利用一系列 [SoC 特有的内核调整](https://forum.xda-developers.com/t/systemless-rom-mod-v2-ww-17-0823-2012-131-armoury-crate-unleashed.4242423/post-84598771)来扩展军械库机箱中的可能设置。

以下是此 Magisk 模块提供的功能分类:

*   当一个应用程序被添加到军械库时，不再需要两次向后滑动手势
*   当一个应用程序被添加到军械库时，不再需要双首页手势
*   一旦一个应用程序被添加到军械库，从屏幕左侧移除游戏精灵触发器(它仍然可以通过通知抽屉中的通知来访问)
*   从军械库板条箱扩展 cpuset 功能
*   为 AirTriggers 提供每秒 10 次点击的功能(从 v4 开始)

值得一提的是，突然限制特定应用程序的 CPU 频率只会导致断断续续，因此在调整参数时，请尝试找到正确的平衡。此外，一些游戏倾向于将 AirTriggers 中的大量快速连续触摸直接标记为作弊。记住这一点，如果你有一部 ROG Phone 3，并且你想体验它的真正力量，你现在可以从下面的链接下载 Armoury Crate Unleashed Magisk 模块。该模块目前处于 v4 版本，仅在 ROG 手机 3 的软件版本 [17.0823.2012.131](https://www.xda-developers.com/rog-phone-3-zenfone-7-issues-hd-playback-netflix/) 上进行了测试。

**[下载军械库机箱为 ROG 手机解锁 Magisk 模块 3](https://forum.xda-developers.com/t/systemless-rom-mod-v2-ww-17-0823-2012-131-armoury-crate-unleashed.4242423/)**

* * *

## 更新 1: ROG 电话 II 支持

《军械库板条箱释放》mod 的开发者 Freak07 已经将他的作品移植到了 ROG Phone II 上。

**[华硕 ROG 手机二代论坛](https://forum.xda-developers.com/c/asus-rog-phone-ii.9056/)**

最初的版本需要运行华硕固件版本 WW-17.0240.2103.75 的 ROG Phone II。当然，您仍然需要拥有 Magisk 的 root 访问权限。

**[下载军械库机箱为 ROG 手机释放 Magisk 模块 II](https://forum.xda-developers.com/t/10-04-2021-systemless-rom-mod-v2-ww-17-0240-2103-75-armoury-crate-unleashed.4260253/)**