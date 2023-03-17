# Android 12 可能会让你休眠不用的应用程序来释放空间

> 原文：<https://www.xda-developers.com/android-12-hibernate-apps/>

**更新 1 (01/25/2021 @ 02:30 PM ET):** 我们现在知道 Android 的应用休眠功能将如何在清除缓存之外进一步释放存储空间。[点击这里了解更多信息。](#update2)

**更新 1 (01/19/2021 @美国东部时间下午 12:32):**我们现在对这个功能如何释放空间有了更多的了解。[点击这里了解更多信息。](#update1)下面保留了 2021 年 1 月 11 日发表的文章。

这可能很难相信，但我们可能离第一个 [Android 12](https://www.xda-developers.com/android-12/) 开发者预览版的发布只有一个多月了。毕竟，第一个 Android 11 开发者预览版是在 2020 年 2 月在[发布的！我们一直在搜索 Android 开源项目(AOSP) Gerrit](https://www.xda-developers.com/android-11-developer-preview-1-google-pixel/) [寻找下一版本 Android 新功能](https://www.xda-developers.com/tag/android-12/)的线索，最近我们发现了谷歌正在为 Android 12 开发应用程序休眠功能的证据。

基于提交给 AOSP 的几个代码更改[，谷歌增加了一个新的应用程序休眠系统服务“管理应用程序休眠状态，应用程序可以进入这种状态，这意味着它们没有被积极使用，可以针对存储进行优化。”](https://android-review.googlesource.com/q/topic:%22add-hibernation-service%22+(status:open%20OR%20status:merged))

不幸的是，我们没有关于这个功能的更多细节。比如我们不知道 app 怎么会进入这种状态。是基于 app 使用统计自动确定的吗？用户可以手动选择强制应用休眠吗？我们也不知道应用程序将如何针对存储进行优化，也不知道操作系统将如何告诉用户哪些应用程序已经休眠。

我们猜测，应用程序休眠将是自动的[,就像 Android 11 中引入的自动撤销权限功能](https://www.xda-developers.com/android-11-features-developers-new-apis/#div-gpt-ad-xda-developerscom35949:~:text=If%20Android%20detects%20that%20you%20haven%E2%80%99t,it%E2%80%99ll%20automatically%20revoke%20all%20granted%20permissions.),优化涉及压缩 APK 和其他应用程序资源，但在提交更多代码更改之前，我们无法确定。我们也不确定这项功能是否会在 Android 12 上实现，因为提交的内容还没有合并。仍然有时间添加这样的新功能，但窗口很快就要关闭了。一旦我们了解了更多关于这个应用程序休眠服务或 Android 12 的任何其他功能，我们将分享这些信息。

*感谢 XDA 公认的开发者 [luca020400](https://forum.xda-developers.com/m/luca020400.5778309/) 的提示！*

* * *

## 更新 1:清除应用缓存

虽然应用程序休眠功能的提交尚未合并——这意味着我们仍然不知道它是否会在 Android 12 中结束——但我们现在已经了解了关于该功能如何工作的更多信息。根据新提交中提交的代码[(再次被 XDA 知名开发者](https://android-review.googlesource.com/c/platform/frameworks/base/+/1550417) [luca020400](https://forum.xda-developers.com/m/luca020400.5778309/) 发现)，应用休眠功能将自动清除应用的缓存文件。释放的存储量取决于相关应用程序——视频流和消息应用程序可以缓存数百兆的数据——但这只是应用程序休眠功能的一部分。在一篇评论中，Google devs 暗示通过“包级休眠”可以节省更多的存储空间。这可能指的是压缩应用程序及其资源，或者其他减少应用程序安装占用空间的操作。

* * *

## 更新 2:删除编译工件

在上周晚些时候提交给《AOSP 精神报》的一份新承诺中，谷歌工程师透露了 Android 的应用程序休眠功能将如何在包/APK 级别优化存储空间。代码更改中留下的注释表明，当一个应用程序对所有用户休眠时，它的编译工件文件(vdex/。odex)将被删除。[根据谷歌](https://source.android.com/devices/tech/dalvik/configure)的说法，vdex 文件包含 APK 的未压缩 dex 代码，而 odex 文件包含 APK 中方法的提前编译代码。通过删除这些文件释放的空间量可能不会很多，特别是与缓存的图像或视频的文件大小相比。然而，在具有少量内部存储的低端设备上，节省几十兆字节将为几十张额外的照片释放空间。