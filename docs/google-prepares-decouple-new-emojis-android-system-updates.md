# 你不需要下载完整的更新就可以在 Android 12 上获得新的表情符号

> 原文：<https://www.xda-developers.com/google-prepares-decouple-new-emojis-android-system-updates/>

**更新 1 (01/26/2021 @美国东部时间下午 1:53):**谷歌已经合并了 Android 中启用可更新系统字体的提交，正好赶上 [Android 12](https://www.xda-developers.com/android-12/) 。[点击这里了解更多信息。](#update1)文章发表于 2020 年 11 月 24 日，下面保留。

表情符号已经成为我们非正式表达中不可或缺的一部分。这些微小的图形资产为纯粹的文字添加了情感、意图和特征。Unicode 标准中频繁添加的新表情符号证明了它们的受欢迎程度。每当 Unicode 获得新的表情符号时，我们需要等待操作系统升级到我们的手机，以支持表情符号，然后我们才能真正让它们成为我们互联网行话的一部分。谷歌似乎准备让这变得更容易，因为一些提交表明，它正在努力将新的表情符号与 Android 系统更新分离。

目前，Android 上的所有字体都存储在系统分区中，更具体地说，是在 */system/fonts* 目录下。特别是表情符号，存在于名为 *NotoColorEmoji.ttf* 的文件中。系统分区是只读的，更新分区内的任何文件都需要在分区未挂载时进行系统更新。所以获得新字体和新表情符号的唯一方法是等待官方 OTA 更新或者[通过 root](https://www.xda-developers.com/android-11-new-emoji-install-root-magisk-module-unicode-13/) 自己非正式安装。

Android 开源项目(AOSP) Gerrit 发现了新的提交，旨在将字体文件从需要升级操作系统中分离出来。请记住，这些提交还没有被合并。我们可以从提交描述中了解他们的目的:

[添加/数据/字体/文件目录](https://android-review.googlesource.com/c/platform/system/sepolicy/+/1501158):

*更新后的字体文件将存储到/data/fonts/files，所有应用程序将读取该文件以绘制文本。因此，/data/fonts/files 需要对应用程序可读，而只对 system_server(和 init)可写。*

[为可更新的系统字体设置/data/fonts 目录](https://android-review.googlesource.com/c/platform/system/core/+/1502269):

*- /data/fonts/files 更新后的字体文件放在这个目录下。任何应用程序都可以读取该目录下的文件。只有 system_server 可以将字体文件写入此目录。*

*-/data/fonts/config system _ server 使用的字体配置存储在这个目录下。只有 system_server 可以读/写此目录。*

这些提交实质上使得 *system_server* 进程能够将更新的字体文件写入 */data/fonts 目录*。数据分区是以读写方式挂载的，因此通过这种改变，Google 只允许 *system_server* 进程对这个目录进行写操作。然后，所有应用程序将从这个目录中读取字体和表情文件来绘制文本。因此，更新的字体文件，以及新的表情符号，可以被推送到手机上，而不需要为此进行整个 OTA 更新。

我们重申，这些提交尚未合并。因此，我们不确定这种变化何时会发生。如果这些提交在未来几个月内合并，我们可以看到这种变化发生在 [Android 12](https://www.xda-developers.com/android-12/) 中。

*感谢 XDA 公认的开发者 [luca020400](https://forum.xda-developers.com/member.php?u=5778309) 的提示！*

* * *

## 更新 Android 12 可能支持

前几天 Google [合并了](https://android-review.googlesource.com/q/topic:%22add_data_font_dir%22+(status:open%20OR%20status:merged))为可更新系统字体设置了/data/fonts 目录的提交。由于表情符号包含在字体文件中，这意味着可以通过将更新的字体文件推送到该目录来添加新的表情符号，而不是通过完整的系统更新。由于这些提交是在几个月后 Android 12 稳定发布之前合并的，因此这一可更新的系统字体功能很可能会在即将到来的 Android 版本中提供。

*感谢@ [LinkofHyrule89](https://twitter.com/LinkofHyrule89/status/1353947218361815045) 的提示！*