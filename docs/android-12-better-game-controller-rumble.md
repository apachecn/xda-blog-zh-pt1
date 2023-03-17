# 更好的游戏控制器震动可以在 Android 12 中添加

> 原文：<https://www.xda-developers.com/android-12-better-game-controller-rumble/>

随着移动和云游戏的兴起，谷歌希望最终改善 Android 上的控制器隆隆声。目前，如果你通过 USB 或蓝牙将游戏控制器连接到你的 Android 设备，它可能不会像在游戏机上玩游戏时那样振动。这是因为 Android 只为振动连接的输入设备提供了最低限度的支持——要么打开，要么关闭。在 10 月份宣布公司正在考虑增加适当的隆隆声支持后，我们现在已经发现了能够改善游戏控制器隆隆声的代码提交。

当我们[在 10 月份第一次强调这个问题](https://www.xda-developers.com/google-is-finally-considering-adding-controller-rumble-support-to-android/)时，我们最初注意到 Android 没有 API 来在外部设备上产生振动，如连接的游戏控制器。事实证明这并不完全正确，因为 Switch hacker 和 emulator dev [的规章制度](https://forum.xda-developers.com/m/bylaws.9648761/)向我们指出，Android 确实具有对振动外部连接设备的基本支持。当前实现的问题是，开发人员无法控制振动的幅度或在连接的设备上生成定制的振动效果，导致触觉反馈不佳。就目前的情况来看，没有触觉反馈比触觉反馈差要好。

幸运的是，谷歌几个月前终于决定解决这个问题，它的工程师[已经向 AOSP 提交了请求](https://android-review.googlesource.com/q/topic:%22InputDeviceRumble%22+(status:open%20OR%20status:merged))，寻求改善输入设备的隆隆声支持。代码更改增加了对振幅控制的支持，并为生成自定义振动效果铺平了道路。不是所有的游戏控制器都被支持，因为游戏手柄的驱动程序必须支持 Linux 下的[力反馈，但是大多数游戏控制器应该可以工作。这将有助于支持为其设计的游戏中的隆隆声，其中包括许多移动玩家可以通过云游戏服务访问的主机游戏，如谷歌自己的 Stadia，英伟达的 GeForce NOW，微软的 xCloud 等。](https://www.kernel.org/doc/html/latest/input/ff.html)

由于这些提交还没有合并，我们不知道改进的游戏控制器隆隆声是否会进入 Android 12。然而，有可能这个功能已经在内部合并了，谷歌现在只是将提交上传到公开的 AOSP 回购。或者，谷歌可以在未来几天或几周内合并这些变化，给这些变化足够的时间传播到 Android 12。

*特色图片:配有 ROG Kunai 3 游戏手柄的华硕 ROG 手机 3*