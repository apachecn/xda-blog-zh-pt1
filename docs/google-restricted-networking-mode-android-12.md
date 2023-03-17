# 谷歌在 Android 12 中增加了受限联网模式

> 原文：<https://www.xda-developers.com/google-restricted-networking-mode-android-12/>

# 谷歌在 Android 12 中增加了受限联网模式

谷歌在 Android 12 中增加了新的受限联网模式。这种新的防火墙模式将阻止所有用户应用程序访问互联网。

随着第一个 [Android 12](https://www.xda-developers.com/android-12/) 开发者预览版预计将于下个月上线，关于谷歌下一个主要的操作系统更新，我们仍然有很多不知道的。鉴于 Android 12 的大部分代码库并不公开，挖掘 Android 开源项目[只能揭示这么多](https://www.xda-developers.com/tag/android-12/)。尽管如此，我们有时会在 AOSP 看到 Android 新功能的证据，尽管它们通常不是很令人兴奋。遗憾的是，我们发现的最新功能，内部称为“受限网络模式”，并没有提供我们希望看到的可配置防火墙，但它确实有一些有趣的含义。

少数合并到 AOSP 的提交描述了新的受限网络模式特性。谷歌[创建了一个新的防火墙链](https://android-review.googlesource.com/c/platform/frameworks/base/+/1505234)——Linux iptables 实用程序遵循的一组规则，以允许或阻止网络流量——以支持受限网络模式。当此模式通过设置开启[时，只有持有](https://android-review.googlesource.com/c/platform/frameworks/base/+/1545865)[CONNECTIVITY _ USE _ RESTRICTED _ NETWORKS](https://android.googlesource.com/platform/frameworks/base/+/master/core/res/AndroidManifest.xml#1867)权限的应用程序才被允许使用网络。由于此权限只能授予特权系统应用程序和/或 OEM 签名的应用程序，这意味着用户安装的所有应用程序的网络访问都将被阻止。实际上，这意味着你仍然可以从使用 Firebase Cloud Messaging (FCM)的应用程序接收推送通知，因为这些通知是通过拥有必要权限的特权 Google Play Services 应用程序发送的，但除了少数其他系统应用程序之外，其他应用程序都不能在后台发送或接收数据。

我们不太清楚谷歌会在 Android 12 中的哪里设置受限网络模式。我们知道它可以在运行时切换和通过 shell 命令以编程方式查询[，就像 Android 的数据保护功能一样，但我们不知道谷歌是否计划让用户制作自己的应用程序允许列表/阻止列表。如果谷歌增加一个面向用户的设置页面来限制每个应用程序的互联网访问，那么这将是一个巨大的进步，这样用户就不必依赖](https://android-review.googlesource.com/c/platform/frameworks/base/+/1545867/3)[像 NetGuard](https://www.xda-developers.com/netguard-gives-you-back-control-over-apps-internet-access-without-root/) 这样使用安卓 VPN API 的应用程序；这些应用程序的运行方式没有问题，但几乎没有[阻止它们被糟糕的 OEM 软件](https://www.xda-developers.com/phone-software-killing-apps-background/)杀死。