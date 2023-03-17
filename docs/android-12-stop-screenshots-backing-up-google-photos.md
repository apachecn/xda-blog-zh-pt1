# Android 12 可能会阻止截图被 Google 相册备份

> 原文：<https://www.xda-developers.com/android-12-stop-screenshots-backing-up-google-photos/>

在这一点上，三星手机的功能与其他 Android 设备没有太大的不同，但三星仍然修改了 Android 操作系统的一些方面，导致了一些令人讨厌的问题。多年来，该公司一直将截图保存在 DCIM 文件夹中，该文件夹只存储相机照片和视频。这导致谷歌照片、Dropbox 和许多其他照片备份服务复制你的截图，不管你想不想。谢天谢地，作为 Android 12 的一部分，一个补丁终于要出来了。

Android 设备有两个文件夹用于存储照片和视频。“图片”文件夹是应用程序存储他们下载的媒体的地方(例如，从 Twitter 保存的图片进入“图片> Twitter”)，默认情况下，Android 将截图存储在“截图”子文件夹下的图片中。在 Android 内部存储器的根目录下还有一个“DCIM”文件夹，可以存储你拍摄的任何照片或录制的任何视频。“DCIM”这个名字来自数码相机的设计标准，它代表“数码相机图像”

Google Photos、Dropbox、OneDrive 和其他媒体备份应用程序会扫描 DCIM 文件夹的更改，并可以将找到的任何新文件备份到云存储中。这在大多数手机上运行良好，但在三星制造的设备上则不然。该公司的一个 UI 软件([和之前的三星体验 UX](https://www.reddit.com/r/GalaxyS8/comments/73l2mk/is_it_possible_to_stop_google_photos_from_backing/))总是将截图存储在 DCIM 目录中，导致应用程序将它们检测为新的相机照片。没有办法阻止谷歌照片在三星设备上备份截图，除非你完全关闭自动备份，或者使用像 [PinSync](https://play.google.com/store/apps/details?id=com.kidscrape.prince) 这样的第三方解决方案。对于应用程序来说，检测截图并添加一个忽略它们的设置不会有太多额外的工作，但 Google Photos 和其他人没有做到这一点。

谢天谢地，看起来谷歌可能会在操作系统层面解决这个问题。感谢一个可靠的消息来源，我们已经获得了 Android 12 兼容性定义文档(CDD)的初步修订版，它定义了设备必须满足的标准，才能通过 Android 认证并与谷歌应用一起发布。谷歌提议在第 7.6.2 节“应用共享存储”中添加以下内容，用于 Android 12 的 CDD:

> #### 如果设备实现具有屏幕截图或屏幕录制功能，包括通过硬件快捷方式或软件按钮，它们:
> 
> #### **必须**将生成的图像或视频文件保存在名为“截图”的目录中，该目录是在板载存储器或 SD 卡的可靠端口上的“图片”下自动生成的。可以通过使用 DIRECTORY _ SCREENSHOTS 来访问它。
> 
> #### **不得**将截图和屏幕录像保存在 DCIM、图片、视频或自定义目录中。

Android 12 CDD 尚未最终确定，因此这一新条款仍有可能被取消，类似于 Android 11 中提出的虚拟 A/B 分区要求[所发生的情况。此举将迫使三星将截图存储在预定的位置，修复谷歌照片和其他应用程序中的错误行为。三星也不是唯一的违规者——小米的 MIUI】也在 DCIM](https://www.xda-developers.com/google-virtual-ab-seamless-updates-android-11/) 中存储截图，OPPO 和 Realme 也是如此。

值得注意的是，这不会阻止谷歌照片、OneDrive、Dropbox 和其他服务备份截图。相反，它将使所有谷歌认证的 Android 设备的截屏存储更加可预测。Google Photos 已经可以选择添加额外的文件夹进行备份，这可以与 Pixel 手机和其他类似设备上的截图目录一起使用。

我们已经联系了谷歌进行评论，如果有回音，我们会更新这篇文章。