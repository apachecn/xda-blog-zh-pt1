# 2023 年安卓设备最佳应用

> 原文：<https://www.xda-developers.com/android-augmentation-and-electronics-mod-101-hacking-a-relay-into-a-circuit-xda-developer-tv/>

Android 最大的优点之一就是它的可定制性。这种定制可以从简单的事情开始，比如[安装一个新的启动器](https://www.xda-developers.com/best-android-launchers/)，甚至到[让你的智能手机](https://www.xda-developers.com/root/)root 以便解锁真正的超级用户权限。你想走多远实际上取决于你，但如果你想完全控制你的设备，并添加工厂安装的操作系统中不总是可用的功能，你最终会选择一些利用 root 访问潜力的应用程序。

有很多应用程序，但很少能达到长期保持领先地位所需的受欢迎程度。由于成功率下降，缺乏支持，功能冗余，或者人们对它们感到厌倦，一些非常成功的根应用程序很容易从基座上掉下来，只会成为 Android 修改场景历史上的一个污点。如果你是新手，你可能会在几个选择中犹豫不决，包括那些被否决的选择。不过不要担心，我们是来帮忙的。

这篇文章将让你仔细看看你可以在你的 Android 设备上安装的一些最好的根应用，并解释每一个能为你做什么。

* * *

## 自动化

### 大型机器人

MacroDroid 提供了一套先进的自动化功能，但主要侧重于简单易用的用户界面和逻辑逐步过程的可用性。这款应用还附带了一个插件商店，你可以在那里找到与 MacroDroid 兼容的其他应用，这样你就可以进一步扩展功能。

**MacroDroid: [XDA 讨论线程](https://forum.xda-developers.com/t/1694335/)**

### 包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包包

Tasker 可能是 Android 最受欢迎的自动化应用，这是有充分理由的。该应用程序允许您创建基于特定条件自动触发的配置文件来执行任务。Tasker 还提供了各种各样的插件。有了 root 访问权限，您可以自动化几乎任何您能想到的事情。

**[XDA Tasker 提示&招数论坛](https://forum.xda-developers.com/f/tasker-tips-tricks.5015/)**

* * *

## 备份和恢复

在 Android 上备份和恢复数据可能是一项痛苦的工作。多亏了这些应用程序，有了 root 用户，事情就简单多了。

### 移动

就像其他备份应用程序一样，Migrate 会备份你的应用程序数据、APK 文件、权限、通话记录、消息等。它的独特之处在于，在 ROM 安装过程中，它可以毫无痛苦地将它们还原为 TWRP 备份。

**迁移: [GitHub 回购](https://github.com/BaltiApps/Migrate-OSS) || [XDA 讨论线程](https://forum.xda-developers.com/t/3862763/)**

### Neo 备份

Neo Backup(以前的 OAndBackupX)是一款用于 Android 的开源备份应用程序，允许您备份单个应用程序及其数据。支持单独和批量备份/恢复。您也可以选择加密备份。

**Neo 备份: [GitHub 回购](https://github.com/NeoApplications/Neo-Backup) || [XDA 讨论线程](https://forum.xda-developers.com/t/4167179/)**

https://f-droid.org/en/packages/com.machiav3lli.backup/

### 分区备份和恢复

有经验的修改者通常需要创建或恢复低级分区备份。如果你不想使用 CLI 工具如`dd`来做这样的操作，你可以选择分区备份&恢复应用。

**分区备份&恢复: [XDA 讨论线程](https://forum.xda-developers.com/t/3003599/)**

### 快速备份

Swift Backup 可以备份你的 apk，你的短信，你的通话记录，应用壁纸，无需 root。然而，通过 root 访问，它可以备份和恢复特殊的应用程序数据，如权限、电池优化、Magisk 隐藏应用程序状态等。滴也可以访问一些只支持 root 用户的功能。

* * *

## 用户化

### 达尔克

DarQ 为 Android 10 及以上版本提供了每个应用程序可选的强制黑暗选项。它还提供了一个选项，只在日落之后和日出之前应用系统黑暗主题(以及可选的强制黑暗)。

**DarQ: [GitHub 回购](https://github.com/KieronQuinn/DarQ) || [XDA 讨论线程](https://forum.xda-developers.com/t/3944356/)**

### live boot(live boot)

LiveBoot 是一个独特的启动动画应用程序，在设备启动时向您显示 logcat 和 dmesg 的输出。修改者不仅认为它是比 OEM 徽标更好的启动动画，而且它也很有用，因为它可以在错误发生时向您显示这些日志中的错误。

**live boot:t1】github rest| |[xd da 讨论线程](https://forum.xda-developers.com/t/2976189/)**

* * *

## 生产力

### 阿达韦

AdAway 是一款免费开源的[广告拦截器](https://www.xda-developers.com/block-ads-on-android/)，它使用 hosts 文件来拦截提供广告服务的主机名。它本质上做的是保存一个广告服务网络的更新列表，并将它们重定向到本地主机(即您自己的电话)，因此这些请求不会到达任何地方，也不会提供任何广告。该应用程序也有非 root 模式，但它与 root 配合使用效果最好。

**AdAway: [GitHub 回购](https://github.com/AdAway/AdAway) || [XDA 讨论线程](https://forum.xda-developers.com/t/2190753/)**

https://f-droid.org/en/packages/org.adaway/

### AFWall+

AFWall+是“Android Firewall Plus”的缩写，是一个用于`iptables` Linux 防火墙的图形前端。它提供了对允许哪些 Android 应用程序访问网络的细粒度控制。您还可以使用此应用程序控制局域网内或通过 VPN 连接时的流量。

**AFWall+: [GitHub 回购](https://github.com/ukanth/afwall) || [XDA 讨论线程](https://forum.xda-developers.com/t/1957231/)**

https://f-droid.org/en/packages/dev.ukanth.ufirewall/

### Aurora Store

Aurora Store 是谷歌 Play 商店的一个流行的开源客户端，允许用户在任何设备上搜索、下载和更新 Android 应用程序和游戏，而不依赖于任何类型的 [GApps](https://www.xda-developers.com/download-google-apps-gapps/) 、MicroG 或谷歌服务。有了 root 权限，它可以在应用程序下载后立即在后台自动安装和更新。

**极光商店: [GitLab 回购](https://gitlab.com/AuroraOSS/AuroraStore) || [XDA 讨论线程](https://forum.xda-developers.com/t/3739733/)**

https://f-droid.org/en/packages/com.aurora.store/

### BetterBatteryStats

如果你曾经觉得一些应用程序通过不断在后台运行或从深度睡眠状态中唤醒你的设备来滥用你的电池，那么你需要尝试更好的电池状态。你可以配置这个应用程序来跟踪这些唤醒锁，并关注一切。

**BetterBatteryStats: [XDA 下载与讨论线程](https://forum.xda-developers.com/t/1179809/)**

### 滴

滴是一个漂亮的工具，使普通应用程序能够直接调用具有 ADB/root 权限的系统 API。它也可以在非根环境中使用，但是与不同的 OEM 皮肤有许多不兼容性，因此根模式是更好的。

**滴: [GitHub 回购](https://github.com/RikkaApps/Shizuku)**

### 存储隔离

Storage Isolation 是一款应用程序，其工作原理与 Android 的[范围存储](https://developer.android.com/training/data-storage#scoped-storage)功能相同，并允许您管理应用程序如何使用您的存储。顾名思义，您可以选择要隔离哪些应用程序，以及要授予哪些应用程序对共享存储的完全访问权限。

### 泰尔穆克

Termux 是一个功能丰富的终端仿真软件，适用于您的 Android 设备，同时也是一个 GNU/Linux 环境。它附带了一个多功能的 Linux 应用程序包集合，其中一些是为根用户量身定制的。请记住，[Termux 的 Google Play 版本早就被弃用了](https://www.xda-developers.com/termux-terminal-linux-google-play-updates-stopped/)，所以请始终从其 GitHub repo 或 F-Droid 获取最新版本。

**术语:[github rest](https://github.com/termux)**

https://f-droid.org/en/packages/com.termux/

* * *

## 多方面的

### 文件管理应用程序

当我们谈论 Android 上的文件管理器时，有相当多的选项是[我们推荐的](https://www.xda-developers.com/best-file-manager-android/)。对于高级用户来说，拥有 root 权限的文件管理器非常方便。你可以访问 Android 的所有文件系统，并根据需要进行修改。

### 内核管理器应用

如果你曾经关心过在你的 Android 设备上使用定制内核的话，那么你可能听说过内核管理器应用，比如 EX Kernel Manager，Franco Kernel Manager 等等。用户可以利用这些应用来调整 CPU 控制器、改变时钟速度和电压值、调整调度程序等等。

### 日志阅读器应用程序

在记录你的 Android 设备正在做什么的时候，有很多选项可供选择。无论是出于调试或报告问题的目的，还是想通过 PC 或直接从设备获取日志，[您都有无数的选择](https://www.xda-developers.com/how-to-take-logs-android/)。使用 root 访问权限，日志阅读器应用程序可以轻松地连接到许多其他方式无法读取的源。

### 神奇的模块

在 Android 设备上释放超级用户权限的许多不同方法中，Magisk 无疑是最好的。由于其无系统界面和对附加模块的[支持，您可以调整、增强和添加设备功能。](https://www.xda-developers.com/best-magisk-modules/)

### 暴露模块

由 Xposed 框架提供支持的, [Xposed 模块](https://www.xda-developers.com/best-xposed-modules/)是直接插入到您的操作系统中的小应用程序，让您完全控制您的 Android 设备的功能。

* * *

## 荣誉奖

### 钛备份

作为最古老的根应用程序之一，Titanium Backup 允许用户跨多个 rom 备份和恢复所有已安装的应用程序及其用户数据，包括所有系统应用程序和受保护的应用程序。更重要的是，它是为数不多的仍能兼容安卓 1.5 版本的应用之一。

### ViPER4Android FX

对于许多人来说，Viper4Android FX 是他们首选的音频增强解决方案，实际上对一些人来说仍然如此。该项目包括一个驱动程序和一个图形均衡器接口。随着 Android 新更新的推出，该项目面临着一些不兼容的问题。

**ViPER4Android FX: [XDA 下载与讨论线程](https://forum.xda-developers.com/t/3774651/)**

* * *

植根于你的 Android 智能手机打开了一个定制的世界。如果你能想象一个定制或调整，可能有一个工具或模块通过 root 访问来实现它。如果你喜欢这个列表，或者有一些你认为我们可能错过的好选择，请在下面的评论中告诉我们。