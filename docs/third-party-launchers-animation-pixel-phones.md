# 这就是为什么 Nova Launcher 在谷歌 Pixel 手机上工作得更好

> 原文：<https://www.xda-developers.com/third-party-launchers-animation-pixel-phones/>

在过去，第三方启动器应用程序通常比大多数 Android 手机上的股票启动器提供更好的体验。然而，随着最近应用程序屏幕的改造和 Android 9 Pie 中手势的引入，第三方启动器处于劣势，因为这些新的体验被集成到了股票启动器应用程序中。随着时间的推移，谷歌试图让第三方启动器在使用手势时的体验不那么糟糕，最近他们实际上已经开始在这方面取得成功。

如果你在过去几个月里在谷歌 Pixel 手机上使用过 Nova Launcher 测试版，你可能会注意到使用手势导航时的流畅动画。不幸的是，当你在任何其他设备上使用 Nova Launcher 时，你不会看到这些相同的动画，至少现在是这样。为了理解为什么我们首先需要简单解释一下是什么将 Nova Launcher 等第三方启动器与 Google 的 Pixel Launcher 等股票启动器区分开来。

谷歌首先在安卓 9 派中引入了手势导航[。为了让手势感觉尽可能流畅，谷歌需要让应用过渡看起来无缝。他们还想让用户从最近的应用程序屏幕上访问他们的整个应用程序列表。为了实现这两个目标，谷歌决定将处理最近应用程序屏幕的代码从 Android 的 SystemUI 转移到 Launcher3，这是 Android 的开源启动器应用程序，大多数 OEM 库存启动器都是从该应用程序中分叉出来的。因此，](https://www.xda-developers.com/android-pie-google-pixel-google-pixel-2/)[快步](https://android.googlesource.com/platform/packages/apps/Launcher3/+/master/quickstep/)组件诞生了，由于其特权性质，安卓只允许预装的启动器应用程序被设置为最新的应用程序提供商。如果第三方启动器支持，这可以被[用根访问](https://www.xda-developers.com/quickswitch-magisk-module-android-pie-recents-launchers/)覆盖，但是对大多数用户来说，这意味着第三方启动器应用程序将总是依赖股票启动器来处理手势和最近的应用程序屏幕。正如你们中的大多数人可能经历过的那样，结果可能有点困难，过渡看起来不流畅也不流畅。除非你使用谷歌像素手机，也就是说。

在大多数谷歌 Pixel 手机上，存在一个 API，第三方启动器可以使用它来使应用程序返回主屏幕的过渡看起来更自然。一些第三方启动器应用程序，如 [Niagara Launcher](https://www.xda-developers.com/niagara-launcher-out-of-beta/) 和前面提到的 Nova Launcher 都在利用这个 API，尽管后者只在其[开发中的 v7 版本](https://www.xda-developers.com/nova-launcher-getting-major-rewrite-new-animations-version-7/)中包含它。当使用这个 API 时，每当用户执行滑动到主页手势时，第三方启动器应用程序都会收到来自 QuickStep 的意向和回调。第三方启动器然后可以向手势系统提示如何在窗口最小化到应用程序图标上时动画显示窗口。

下面是 Niagara Launcher 的一个例子，由 Launcher 的开发者提供:

这里有一个对比，展示了动画在[华硕 ROG 手机 5](https://forum.xda-developers.com/f/asus-rog-phone-5.12119/) 和[谷歌像素 4](https://forum.xda-developers.com/c/google-pixel-4.9014/) 上的样子，这两款手机都运行 Nova Launcher v7.0.25(发布时的最新测试版)和 Android 11:

\ r \ nht TPS://www . YouTube . com/watch？v=equ-8yDw_Do\r\n

现在你可能会想:这个 API 是谷歌 Pixel 手机独有的吗？答案是不，不是。该 API 是 Launcher3/QuickStep 的一部分，[可以在 AOSP](https://android.googlesource.com/platform/packages/apps/Launcher3/+/30ac97d9386736c3322a3277f74523497627b9f5) 找到，这意味着它对任何 OEM launcher 应用程序开放。虽然 API [承诺在 2020 年 7 月 21 日在内部推出 3](https://android.googlesource.com/platform/packages/apps/Launcher3/+/30ac97d9386736c3322a3277f74523497627b9f5) ，但似乎是在 12 月随着 Android R QPR1 的发布[并入了 AOSP 主分支](https://android.googlesource.com/platform/packages/apps/Launcher3/+/053a3415fecf0aafda359b7b3db935ad770ebbb1)。

 <picture>![](img/48527d7c45886502f492e4bf53e99944.png)</picture> 

The API that makes Nova Launcher and Niagara Launcher feel more native on Google Pixel phones.

Nova Launcher 的开发者凯文·巴里(Kevin Barry)是第一批发现这个 API 的人之一，他告诉我们，他怀疑 OEM 厂商没有在 Launcher3 的分支中使用这个 API 的部分原因是它在 Android 11 的发布周期中来得有点晚。合并大的 AOSP 变化需要相当多的努力，Android R QPR1 更新肯定包含了很多。在过去的几年里，我们称这些代码发布为“维护发布”，但是在原始设备制造商的反对下，谷歌不再这么做了(至少我是这么听说的)。这就是为什么流行的 Android 定制 ROM linea geos 将其最新版本称为“ [LineageOS 18.1](https://www.xda-developers.com/lineageos-18-1/) ”而不是“LineageOS 18”，以表明该 ROM 是基于最新的 Android 11 代码库而不是最初的 Android 11 版本。

另外值得注意的是，这个 API 只有在[12 月 Pixel 功能下降](https://www.xda-developers.com/pixel-feature-drop-adaptive-sound-google-photos-suggestions/)之后才能在谷歌 Pixel 手机上使用，这与公开的 Android R QPR1 发布相吻合。尽管 Pixel 2 在 12 月获得了其[最终更新，但该更新不包括 Android R QPR1 代码库，这就是为什么运行 Nova Launcher v7 的 Pixel 2 用户没有与其他 Pixel 相同的体验。(Pixel 2 的所有者可以从更新的 Pixel 设备下载更新版本的 Pixel Launcher，该设备具有 API，但](https://www.xda-developers.com/google-pixel-2s-final-software-update-now-available/)[用户报告表明](https://www.reddit.com/r/Android/comments/kwbhu2/nova_launcher_now_supports_the_fancy_new_gestures/gj3b4w2/)即使偶尔可以工作，动画仍然有问题。提醒一下，Pixel Launcher 是建立在 Launcher3 之上的，就像大多数股票发射器一样，但它也包括一些 Pixel 专有的功能。)

那么，将这个 API 添加到其他 Android 设备需要什么呢？不幸的是，这个问题没有简单的答案，因为我们不知道每个 OEM 是如何开发其启动器应用程序的。鉴于[谷歌如何严格控制全屏手势导航](https://www.xda-developers.com/google-gesture-navigation-android-10/)，我们怀疑大多数原始设备制造商不会大量修改与手势和/或 QuickStep 相关的代码。除非原始设备制造商故意撤销提交，破坏代码，或者拒绝更新 Launcher3，那么我们应该会看到这个 API 被添加到原始设备制造商的启动程序中，只要他们基于即将到来的 [Android 12](https://www.xda-developers.com/android-12/) 版本。事实上，我们采访的一家 OEM 厂商华硕告诉我们，他们计划在他们的 Android 12 更新中引入这个 API。我们不知道谷歌是否向 OEM 厂商传达了这一变化，但我们希望更多的 OEM 厂商注意到这一变化，并决定将该 API 纳入他们的 Launcher3 分支中，以改善使用第三方启动器的体验。

然而，这项工作不会就此结束。即使包含了这个 API，仍然需要做更多的工作来实现第三方发布者和 OEM 发布者之间的对等。例如，当用户在主屏幕动画出现之前点击屏幕时，一些 OEM 设备会闪烁。有时，会出现系统启动器应用程序，而不是所选的第三方启动器应用程序(我遇到过几次这种情况)。改进的过渡动画很好，但没有人想处理启动器应用程序或最近应用程序屏幕中的错误，所以手势代码仍然需要一些清理和/或标准化。

感谢 Kevin Barry 和 Peter Huber 对本文的帮助！