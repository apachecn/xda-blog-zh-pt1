# 这就是为什么 Termux 应用程序不再在 Google Play 上获得更新

> 原文：<https://www.xda-developers.com/termux-terminal-linux-google-play-updates-stopped/>

正如你们很多人可能都知道的那样，Android 操作系统是由底层的 Linux 内核支持的。尽管如此，由于不同的运行时系统和库，Android 和 Linux 应用程序不容易交换。然而，你可以在任何 Android 设备上安装并运行类似于 [Termux](https://www.xda-developers.com/termux-the-ultimate-linux-terminal-emulator-for-android-xda-spotlight/) 的终端模拟器应用程序。多年来，狡猾的 Android 用户一直使用 Termux 作为一个方便的终端仿真软件，以及一个强大的 GNU/Linux 环境，这要归功于它相当大的 Linux 软件包集合。不幸的是，该应用程序现在正处于其生命的关键路口，因为其开发者已经决定完全停止更新 Play Store 版本，并迁移到 F-Droid，原因是最近推出的 Google Play 政策和 Android SDK 行为变化。

自 2020 年 11 月 2 日起，Google Play 中现有应用的所有更新都被[要求针对 Android 10 (API level 29)](https://www.xda-developers.com/all-apps-google-play-required-target-android-10-api-level-29/) 或更高版本。虽然先决条件听起来像是带着乐观情绪的好消息，但对 Termux 来说，事情并没有完全朝着那个方向发展。在该项目的 GitHub Wiki 上的一篇帖子中，该软件的主要贡献者 Leonid Pliushch 又名[xeffyr](https://github.com/xeffyr)[解释了](https://github.com/termux/termux-packages/wiki/Termux-and-Android-10)该应用程序与前述 API 级别的兼容性问题。自 Android 10 以来，谷歌一直在强制执行 [W xor X 安全功能](https://en.wikipedia.org/wiki/W%5EX)，这就是为什么一个将`targetSdkVersion`设置为“29”或更高[的不受信任的应用程序无法对应用程序主目录](https://developer.android.com/about/versions/10/behavior-changes-10)内的文件调用`exec()`。这样的[设计](https://www.reddit.com/r/androiddev/comments/b2inbu/psa_android_q_blocks_executing_binaries_in_your/eit1ds7/)在针对 API 级别 29 编译时有效地[破坏了 Termux](https://github.com/termux/termux-app/issues/1072) ，因为它的所有包都包含可执行文件。

你仍然可以在 Play Store 上找到这款应用，但是版本已经严重过时了。由于 Play Store 版本不正式支持 Android 10(或更高版本)，它将不会在某些设备上启动 shell，除非 SELinux 被设置为许可模式，这无疑具有[严重的安全隐患](https://wiki.gentoo.org/wiki/SELinux/Tutorials/Permissive_versus_enforcing)。此外，非根用户[无法访问`/proc/net`](https://www.xda-developers.com/android-q-security-privacy-features/) ，这意味着`netstat`和其他使用该接口数据的实用程序不再工作。

为什么所有这些变化都没有影响到 Termux 的 F-Droid 构建？这是因为在提交包含在 F-Droid 库中的包时，没有严格的 Android SDK 版本要求。与 Play Store 版本不同，针对比 10 更老版本的 Android 的版本在这里不受影响，因此团队可以继续推送更新，而不用担心失去核心功能。

[appbox fdroid "com.termux"]

Termux 开发团队现在希望 Play Store 版本的用户迁移到 F-Droid 变体，以继续获得更新。[迁移过程](https://wiki.termux.com/wiki/Backing_up_Termux)并不简单，因为构建是用一组不同的密钥签署的，因此无法执行无缝更新。正如预期的那样，这些变化确实有效地为那些为了方便起见而喜欢坚持使用 Play Store 更新频道的普通用户设置了障碍。

* * *

如果您的 Android 设备上已经有一个 Termux 实例，请在下面告诉我们您使用它的目的！