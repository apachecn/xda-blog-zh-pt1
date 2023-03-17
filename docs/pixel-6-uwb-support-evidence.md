# 谷歌的 Pixel 6 可能会支持超宽带(UWB)

> 原文：<https://www.xda-developers.com/pixel-6-uwb-support-evidence/>

# 进一步的证据表明，谷歌的像素 6 将拥有超宽带支持

最近提交给 AOSP Gerrit 的代码更改表明，Pixel 6 系列可以支持超宽带(UWB)技术。

超宽带(UWB)是一种短距离无线通信协议，可对物联网设备进行精确跟踪和定位，并通过高频无线电频谱进行高速数据传输。苹果的苹果手机 11 是第一款引入超宽带技术的现代智能手机。从那时起，这项技术已经发展到了几款高端智能手机，包括 Galaxy Note 20 Ultra、 [Galaxy Z Fold 3](https://www.xda-developers.com/samsung-galaxy-z-fold-3/) / Fold 2、Galaxy S21+ / S21 Ultra 以及[小米手机 4](https://www.xda-developers.com/xiaomi-mi-mix-4-launch/) 。随着越来越多的证据表明谷歌的下一代像素手机将支持超宽带，很快[像素 6](https://www.xda-developers.com/google-pixel-6/) 系列将加入这一行列。

Pixel 6 支持超宽带的消息是由 XDA 的米沙·拉赫曼在四月下旬首次报道的。在[谷歌 I/O 2021](https://www.xda-developers.com/google-io-2021-recap/) 上，谷歌宣布在 Android 12 中支持[数字车钥匙](https://www.xda-developers.com/android-12-car-unlock-key/)，并表示该功能将在今年晚些时候出现在 Pixel 和三星 Galaxy 设备上。许多人认为这进一步证实了 Pixel 6 将支持 UWB——尽管应该指出的是，Android 12 的车钥匙功能也可以通过 NFC 工作。然而现在，更多的证据表明 Pixel 6 将支持 UWB。最近提交给 AOSP Gerrit 的代码变更[基本上证实了这个消息:](https://android-review.googlesource.com/c/platform/system/sepolicy/+/1808157)

> 因为我们现在正在为 uwb 创建一个 AOSP HAL。将特定于像素的内部 UWB HAL 从 Android S 重命名为 hal_uwb_vendor，以避免与将在 Android T 中添加的 AOSP HAL 分离策略规则冲突

基本上，谷歌还没有一个通用的 UWB HAL(硬件抽象层)准备提交给 AOSP，所以他们推迟到 Android 13T T1。由于这一延迟，谷歌正在重命名 Android 12 中特定于像素的 HAL，以便它们不会与他们为 Android 13 制作的通用 UWB HAL 冲突。首先，HAL 是一个软件，它让设备的硬件组件与操作系统进行交互。事实上，有一个像素特定的超宽带 HAL 意味着有一个像素手机与超宽带硬件，这很可能是即将到来的像素 6 系列。然而，我们不知道 UWB 支持是否将在 Pixel 6 上提供，或者仅在 Pro 型号上提供。

谷歌[早在 2021 年 4 月就为 Android 中的 UWB](https://www.xda-developers.com/google-adding-ultra-wideband-uwb-api-android/) 添加了通用 API 但是，第三方应用程序无法访问它。