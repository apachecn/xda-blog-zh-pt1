# Android 12 设备可能会默认使用更高效的视频录制格式

> 原文：<https://www.xda-developers.com/oems-change-default-video-capture-format-android-12-hevc/>

在 [Google I/O 2021](https://www.xda-developers.com/google-io-2021-recap/) 的“Android Media 中的新功能”会议期间，Google 概述了媒体捕获和回放的诸多挑战，以及他们正在为开发者做些什么。谷歌想要解决的最大挑战之一是高清视频捕捉的巨大文件大小。这个问题的一个显而易见的解决方案是使用更有效的格式来编码视频文件，看起来一些原始设备制造商将在 [Android 12](https://www.xda-developers.com/android-12/) 中这样做。

谷歌长期以来一直建议使用[免版税的 AV1 编解码器](https://www.xda-developers.com/av1-future-video-codecs-google-hevc/)进行视频编码，但很少有硬件产品支持 AV1 编码的硬件加速。另一方面，还有 H.265/HEVC，这是一种视频编解码器，不是免费的，但过去几年发布的大多数高端 Android 设备都支持硬件加速编码。相比 H.264/AVC，即。谷歌表示，H.265/HEVC 可以以相同的质量录制视频，但比特率只有一半，从而大大减小了文件大小。

运行 Android 和其他操作系统的设备也广泛支持解码以 H.265/HEVC 编码的视频，因此以这种格式录制视频不再是一个问题。然而，问题是大多数相机应用程序默认情况下都禁用 HEVC 记录，而且大多数用户不太可能会钻研“高级”设置菜单，通常可以在那里找到启用它的开关。例如，我打开了以下高端 Android 设备上的库存相机应用程序，发现虽然每个应用程序都提供了通过在 HEVC 编码来更有效地存储视频的选项，但它们都没有默认启用这一切换:

然而，从 Android 12 开始，谷歌表示，更多的原始设备制造商将采用 HEVC 作为视频捕捉的默认格式。

虽然谷歌没有说有多少或哪些原始设备制造商将使 HEVC 成为他们相机应用程序的默认视频捕捉格式，但这是有希望听到的。这意味着普通用户将不再需要打开 HEVC 编码，许多人可能甚至不知道这个功能的存在。通过将 HEVC 作为默认的视频捕获格式，用户可以减少视频记录在本地或云存储上占用的空间。此外，较小的文件大小将减少用户在社交媒体和其他平台上上传视频的时间。

然而，并非所有安卓应用都支持处理 HEVC 内容。对于那些不支持的 app，Android 12 增加了一个[媒体转码 API](https://developer.android.com/about/versions/12/features/compatible-media-transcoding) ，自动将格式转换为 H.264/AVC，兼容性更好。

\ r \ nht TPS://www . YouTube . com/watch？v = pX00lybwwIk \ r \ n