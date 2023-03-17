# 谷歌正在努力加快在新的安卓手机上安装重要应用的速度

> 原文：<https://www.xda-developers.com/google-install-hints-speed-up-installing-important-apps-new-android-phone/>

从一部安卓手机迁移到另一部，尤其是当换到一个新品牌的时候，是很困难的...*不太容易*，说白了。这种情况近年来有所改善，越来越多的应用程序和设置支持无缝迁移，但整个过程仍然需要相当多的步骤和相当多的时间，尤其是因为大多数旧应用程序是逐个安装的，然后需要用户干预手动登录。虽然谷歌正在开发[，使新设备上的应用](https://www.xda-developers.com/google-new-block-store-library-easier-sign-in-apps-new-devices-migration/)更容易登录，但他们也在幕后工作，通过新的“安装提示”功能加快批量恢复过程，旨在帮助你在新设备上尽快启动和运行最重要的应用。

正如 XDA 公认的开发者 [*luca020400*](https://forum.xda-developers.com/member.php?u=5778309) 最初发现的那样，谷歌工程师将“[安装提示](https://android-review.googlesource.com/q/topic:%22install-hints%22+(status:open%20OR%20status:merged))功能描述为谷歌 Play 商店等应用商店在批量安装新应用程序时(如在设置或恢复过程中)决定使用哪个编译器过滤器用于 dex2oat 的一种方式。

以下是相关的提交:

这个 CL 向包管理器使用的几个数据结构添加了一个“安装场景”字段。该值将由后续 CL 使用，以根据指定的用例调整 dexopt 的调用。

[Dex2oat](https://source.android.com/devices/tech/dalvik/configure) 是一个编译器，它获取 APK 文件并生成编译工件， [Android Runtime (ART)](https://www.xda-developers.com/google-android-runtime-art-mainline-module-android-12/) 在安装时加载这些工件，帮助加快应用程序加载时间。Dexopt 是一个在安装时优化 dex 文件的程序。

基于这些提交，似乎安装提示将允许在应用安装期间传递四种不同的编译器过滤器:DEFAULT、FAST、BULK_CRITICAL 和 BULK_NON_CRITICAL。我们假设，在手机恢复过程中，应用商店可以向 dex2oat 发送“BULK_CRITICAL”标志，以便以优化为代价更快地安装某些关键应用程序(这可能会在下次更新应用程序时发生)。

根据你的应用安装和使用历史，预装应用商店不难确定你最常用的应用。根据你所拥有的设备，应用程序商店会有一组预先确定的应用程序，它知道这些应用程序对于功能来说是至关重要的，比如 Google Play 服务和其他 OEM 软件服务。因此，这些应用程序可以在批量安装过程中优先考虑，代价是首次运行优化。

你可能会问，作为用户，这种变化会对你产生什么影响？好吧，提交实际上还没有被合并，所以我们的分析是基于我们此刻在提交中看到的信息(当提交最终被合并时，我们的分析可能会改变)。当用户在新手机上安装一系列应用程序时，应用程序商店将能够优先考虑那些它知道你在上次使用的设备上经常使用的应用程序。因此，如果你经常使用 WhatsApp Messenger，例如，app store 会将标志传递给编译器，让它更快地安装，这样你就可以开始登录对你更有用的应用程序。另一方面，对于你不经常使用的应用程序，这些可以正常安装和优化。我们不知道这将为用户节省多少时间——这很可能取决于有多少应用程序被认为是关键的，以及有多少应用程序首先被恢复——但它可能会为下载数百个应用程序的旧手机或较慢的手机节省几分钟。

如前所述，提交还没有合并，所以我们不知道这些更改何时会传到 Android，或者是否会有进一步的代码更改。如果这些提交在未来几个月内合并，那么我们将看到这个功能在 [Android 12](https://www.xda-developers.com/android-12/) 的应用商店中可用。

* * *

*来自[www.flaticon.com](https://www.flaticon.com/ "Flaticon")T5 的[自由派](https://www.flaticon.com/authors/freepik "Freepik")制作的图标*