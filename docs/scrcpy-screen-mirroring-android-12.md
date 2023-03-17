# 手机到 PC 屏幕镜像工具“scrcpy”现在支持 Android 12

> 原文：<https://www.xda-developers.com/scrcpy-screen-mirroring-android-12/>

Android Debug Bridge，简称为 [ADB](https://www.xda-developers.com/what-is-adb/) ，对于想要在设备上读取系统日志、更改设置或自动化操作的开发人员来说，是一个非常有用的工具。谷歌在制作 ADB 时打算只提供命令行界面，但在 2018 年 3 月初，一名开发者在 ADB 的基础上开发了一个工具，让你不仅可以镜像你的 Android 手机屏幕，还可以从你的 PC 上[远程控制它](https://www.xda-developers.com/scrcpy-control-android-on-pc/)。该工具名为 scrcpy，其最新更新增加了对运行 [Android 12](https://www.xda-developers.com/android-12/) 的设备的支持。

对于那些不熟悉的人来说，scrcpy(scrcpy 是"**SCR**een**c**o**py**")由两个组件组成:一个推送到 Android 设备的服务器应用程序和一个在 PC 上通过 ADB 隧道的套接字与服务器通信的客户端。您的手机屏幕编码为 h.264 视频，由 scrcpy 客户端解码并显示在您的 PC 上。键盘和鼠标输入被发送到服务器，并被转换成设备上的适当输入。虽然 scrcpy 不是唯一的远程控制/屏幕镜像工具，但它是最好的工具之一，因为它是免费的、开源的、可定制的和快速的。

在 Android 12 更新之前，scrcpy 默认创建了一个“安全显示”，以支持镜像内容，否则[会被阻止](https://github.com/Genymobile/scrcpy/issues/36)。然而，Android 12 不再允许具有 shell 权限的进程创建安全显示，如果用户试图在运行 Android 12 的设备上启动 scrcpy，[会立即崩溃](https://github.com/Genymobile/scrcpy/issues/2129)。解决方法很简单:重新构建 Android 服务器，让它创建一个不安全的显示。

scrcpy 的另一个主要新增功能是能够在 Linux 上使用视频流作为网络摄像头。该工具[增加了](https://github.com/Genymobile/scrcpy/pull/2268)V4L2 loopback(Video 4 Linux loopback)支持，使得视频流可以通过 [OBS](https://obsproject.com/) 等支持 v4 L2 的软件打开。视频流可以作为网络摄像头暴露和/或显示在窗口中。

scrcpy 1.18 更新中添加的其他功能包括将视频方向锁定到设备的初始方向的能力，关闭 scrcpy 时关闭设备的电源，第 4 个和第 5 个按钮的新快捷键，自动调整窗口大小以移除黑边，以及将文件保存在/sdcard/Download 而不是/sdcard 中。

1.18 更新的变更日志嵌入在下面。你可以从 GitHub 下载 scrcpy [的最新版本。](https://github.com/Genymobile/scrcpy/releases/tag/v1.18)

### scrcpy v1.18 变更记录档

自 1.17 版以来的变化:

*   增加对 Android 12 的支持( [#2129](https://github.com/Genymobile/scrcpy/issues/2129) 、 [#2402](https://github.com/Genymobile/scrcpy/issues/2402) )
*   添加对 V4L2(作为网络摄像头的设备屏幕截图)的支持( [#2232](https://github.com/Genymobile/scrcpy/pull/2232) 、 [#2233](https://github.com/Genymobile/scrcpy/pull/2233) 、 [#2268](https://github.com/Genymobile/scrcpy/pull/2268) )
*   添加锁定初始视频方向的选项
*   添加一个关闭时关闭设备的选项( [#824](https://github.com/Genymobile/scrcpy/pull/824) )
*   将第四个鼠标键绑定到 APP_SWITCH ( [#2258](https://github.com/Genymobile/scrcpy/pull/2258) )
*   绑定第五个鼠标键来扩展通知面板( [#2258](https://github.com/Genymobile/scrcpy/pull/2258) )
*   在双击展开通知面板上展开设置面板( [#2260](https://github.com/Genymobile/scrcpy/pull/2260) ， [#2264](https://github.com/Genymobile/scrcpy/pull/2264) )
*   默认推送至/SD card/Download([# 2384](https://github.com/Genymobile/scrcpy/pull/2384))
*   将窗口居中调整大小( [#2387](https://github.com/Genymobile/scrcpy/issues/2387) )
*   增加可能的显示 id 范围( [#2009](https://github.com/Genymobile/scrcpy/issues/2009) )
*   以详细模式记录输入事件( [#2371](https://github.com/Genymobile/scrcpy/pull/2371) )
*   修复触摸事件参数( [#2125](https://github.com/Genymobile/scrcpy/issues/2125) )
*   修正三星浏览器的左键点击( [#2169](https://github.com/Genymobile/scrcpy/issues/2169) )
*   移除选项渲染过期帧( [#2268](https://github.com/Genymobile/scrcpy/pull/2268) )
*   将 scrcopy-no console 参数传递给 Windows 上的 scrcopy([# 2052](https://github.com/Genymobile/scrcpy/pull/2052))
*   在 Windows 版本中将平台工具升级到 31.0.2 (adb)
*   各种技术修复