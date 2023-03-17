# Wear 安装程序使再次侧装 Wear 操作系统应用变得容易

> 原文：<https://www.xda-developers.com/wear-installer-sideload-wear-os-apps/>

# Wear 安装程序使再次侧装 Wear 操作系统应用变得容易

一个名为 Wear Installer 的新应用程序可以轻松地使用手机在 Wear OS 智能手表上下载应用程序。继续阅读，了解更多信息！

每天，独立开发者都会在我们的论坛以及其他各种在线平台上发布新的应用或游戏。事实上，每天都有如此多的发布，找到一个真正独特而迷人的应用程序就像大海捞针一样，但这正是我们今天所做的。一位名叫 Malcolm Bryant 的开发人员提出了一个真正创新的解决方案，来解决在 Wear OS 设备上侧装应用程序的问题。这款名为“Wear Installer”的应用程序可以让你保存你的传统 Wear OS 应用程序，并将它们下载到你的手表上，没有任何麻烦。

在我们开始之前，这里有一个关于 Wear OS 应用程序模型的谷歌最新政策的快速回顾:该公司[希望从 3 月 10 日](https://www.xda-developers.com/sideloading-apps-wear-os-complicated/)开始将 Wear OS 应用程序与常规 Android 应用程序分离，这反过来严重限制了应用程序的侧加载能力。Malcolm，又名 Reddit 用户 [*u/malbry*](https://www.reddit.com/user/malbry/) ，first [强调了问题](https://www.reddit.com/r/WearOS/comments/li7nqh/google_removing_the_standard_method_of/)，现在以 Wear Installer 的形式快速修复。虽然仍然可以使用 [Android 调试桥](https://www.xda-developers.com/install-adb-windows-macos-linux/) (ADB)在 Wear OS 设备上[侧加载应用程序，但 Wear Installer 采用了一种略有不同但公认更好的方法来简化安装过程。](https://forum.xda-developers.com/t/how-to-sideload-apks-onto-android-wear-watch.3726276/)

## 如何使用 Wear 安装程序从侧面加载 Wear 操作系统应用

Wear Installer 自带 ADB 实例，而不是依赖外部 PC/Mac 来访问 Android Debug Bridge。此外，该应用程序可以从传统手机应用程序中提取[嵌入式 Wear OS 兼容的 APK 组件](https://developer.android.com/training/wearables/apps/packaging#wear-1x)。因此，你只需要在手机上侧装 Wear Installer APK，这样应用程序就可以通过 ADB 与你的智能手表通信，并远程侧装任何应用程序！它还允许您从手机上的下载目录下载有效的 Wear OS APKs。

了解这款应用的卓越之处的最简单方法是观看一个快速演示:

## 下载磨损安装程序

可以从开发者的网站下载应用[。如果你想给开发者留下一些反馈，一定要查看一下](http://freepoc.org/downloads/) [Reddit 讨论线程](https://www.reddit.com/r/WearOS/comments/lp07ue/new_app_wear_installer_saves_your_legacy_wearos/)。

**[下载穿戴安装程序版本 1.00](http://freepoc.org/wp-content/uploads/2021/02/WearInstaller100.zip)**