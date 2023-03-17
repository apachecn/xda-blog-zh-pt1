# 谷歌暗示 Pixel 6 将采用谷歌制造的“白教堂”芯片

> 原文：<https://www.xda-developers.com/google-pixel-6-gs101-whitechapel-aosp/>

# 谷歌暗示 Pixel 6 将拥有代号为“白教堂”的定制芯片

一名谷歌人留下了一条评论，强烈暗示 2021 Pixel (Pixel 6)将由谷歌自己的代号为 whitechapel 的 GS101 芯片驱动。

本月早些时候，一份报告声称谷歌将在 2021 年推出自己的像素设备。现在，一名谷歌人在网上发表了一篇评论，提供了我们可以指向即将到来的 Pixel 6 将由传言中的谷歌制造的芯片驱动的第一个公开证据。

在提交给安卓开源项目(AOSP)的一份[代码变更](https://android-review.googlesource.com/c/device/google/coral-sepolicy/+/1694487/)中，一个谷歌团队正试图更新 OsloFeedback 应用的 SELinux 策略，该应用负责 Pixel 4 上的 Soli 雷达手势。大多数用户对代码更改本身并不感兴趣，但在评论中，一位谷歌人[回复了](https://android-review.googlesource.com/c/device/google/coral-sepolicy/+/1694487/1#message-b9e6832d7997ff6a17b3484d76d681aa43ca51b8)一个指向谷歌内部源代码回购的链接(H/T XDA 成员 [cstark27](https://forum.xda-developers.com/m/cstark27.2712580/) )。“使用 binder_use 不需要 coredomain。这位谷歌工程师说:“这个在 P21 上运行良好。P21 可能指的是“像素 21”，如果不是预计今年晚些时候推出的另一款设备，它可能至少由像素 6 组成。谷歌很可能不是指这里的 [Pixel 5a](https://www.xda-developers.com/google-pixel-5a/) ，因为早先的一份报告表明，该设备将由与 Pixel 4a 5G/5 相同的芯片[驱动。](https://www.xda-developers.com/pixel-5a-5g-same-chip-pixel-4a-5g/)

公众无法访问该链接，但该 URL 提供了一些有用的信息。

```
 https: 
```

正如你在上面看到的，这个 URL 指向位于/Android/device/Google/**GS 101**-sepolicy/**white chapel**分支中的文件的特定部分。“白教堂”是传闻中谷歌与三星合作设计的芯片的[代号](https://www.xda-developers.com/google-is-working-on-its-own-chip-for-pixel-phones-and-chromebooks/)。“GS101”很可能是指定制“谷歌硅”系列中的第一个芯片，正如本月早些时候由 *9to5Google* 报道的，并得到我们的证实。

这不是谷歌第一次在 AOSP 泄露其即将推出的 Pixel 设备的关键细节。在 Pixel 4 发布之前，[我们发现了](https://www.xda-developers.com/google-pixel-4-90hz-display-android-10-source-code/)Android 10 源代码中的一条评论，该评论基本上确认了 2019 年的 Pixel 将拥有 90Hz 显示屏。今天的泄露没有透露任何关于谷歌硅芯片的实际细节，但这是第一份将 2021 像素与 GS101 和白教堂联系起来的公开证据。

*特色图片:谷歌 Pixel 4*