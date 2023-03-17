# Google Play 系统更新显示启动动画的进度百分比

> 原文：<https://www.xda-developers.com/google-play-system-update-percent-progress/>

# Google Play 系统更新现在显示启动动画的进度百分比

在 Google Play 系统更新期间，您很快就可以在设备启动时看到应用更新的进度百分比。

随着 2019 年 Android 10 的发布，谷歌[推出了](https://www.xda-developers.com/android-q-project-mainline-security/)项目主线，这是一项让谷歌直接向关键 Android 组件提供更新的举措。目标是通过标准化某些系统组件并按照一致的时间表向它们交付更新来增强安全性、保护隐私并提高开发人员的一致性。项目主线的[机制对用户来说是不透明的，更新是分批交付的，没有变更日志。用户唯一看到的是“Google Play 系统更新”正在他们的设备上等待，在下载一个小软件包后，他们会被提示重新启动以应用更改。今天下载了最新的更新后，一些用户已经注意到启动动画现在显示更新过程的完成百分比。](https://www.xda-developers.com/android-project-mainline-modules-explanation/)

Twitter 用户@ [jas0nsg](https://twitter.com/jas0nsg) 是第一个发现这一新功能的人，他与我们分享了以下视频，并在他的 Pixel 5 上演示了这一功能，Pixel 5 今天获得了 Google Play 系统更新:

\ r \ nht TPS://www . YouTube . com/watch？v=R7ltNPmx4Q8\r\n

XDA 知名开发者 luca020400 也发现了他的 Pixel 5 在 Google Play 系统更新后的百分比进步。我们认为该功能是通过更新的 APEX 模块触发的，尽管我们不知道具体是哪个模块负责。这项功能的代码在二月初由[提交给 AOSP](https://android-review.googlesource.com/c/platform/frameworks/base/+/1545805) ，但当时，谷歌工程师[说](https://android-review.googlesource.com/c/platform/frameworks/base/+/1545805/1#message-aa0a33a69d3406a7ab6755547df2d0c0bb86bddb)代码仅仅是为了展示该功能的概念证明。Luca020400 认为，启动动画的进度百分比仅在对艺术模块进行更新[时显示，该模块是在](https://www.xda-developers.com/google-android-runtime-art-mainline-module-android-12/) [Android 12](https://www.xda-developers.com/android-12/) 中添加的。他说，这是因为在重启后对 ART 应用更新需要额外的步骤。

无论如何，这是一个小的功能更新，今天登陆了少数运行 Android 12 的 Pixel 手机。如果您在设备上发现了 Google Play 系统更新，并希望了解发生了什么变化，您可以在更新前后运行以下命令来比较每个 APEX 模块的版本代码:

```
 pm list packages --apex-only --show-versioncode -f 
```