# 在任何安卓手机上获取 ROG 手机 5s 实时壁纸

> 原文：<https://www.xda-developers.com/download-rog-phone-5s-live-wallpapers/>

# 在任何安卓手机上获取 ROG 手机 5s 实时壁纸

在任何 Andorid 设备上从 ROG 手机 5s 获取新的实时壁纸。下载帖子中提供的链接和说明。

华硕最近用高通最新的骁龙 888 Plus 芯片更新了其旗舰产品 [ROG 手机 5 系列](https://www.xda-developers.com/asus-rog-phone-5/)。新的 [ROG 手机 5s 阵容](https://www.xda-developers.com/asus-rog-phone-5s/)包括两款手机:ROG 手机 5s 和 ROG 手机 5s Pro。除了新的芯片组和更好的触摸响应之外，两款手机的硬件都与各自的前辈几乎相同。在软件方面，新的 ROG 手机 5s 设备在 Android 11 的基础上配备了最新版本的华硕皮肤和几个新的动态壁纸。

XDA 公认的贡献者 [linuxct](https://forum.xda-developers.com/member.php?u=4787101) 因共享来自 MIUI 和[oxo OS](https://www.xda-developers.com/oneplus-8t-cyberpunk-2077-edition-wallpapers-sounds-boot-animation-download/)的[实时壁纸端口而闻名，现在已经发布了来自 ROG Phone 5s 系列的新实时壁纸端口。您可以通过以下链接在您的设备上下载这些壁纸端口。在你这样做之前，这里有一个新的实时壁纸预览-探测无人机和星际飞船:](https://www.xda-developers.com/download-miui-12-super-earth-mars-live-wallpapers-ported-other-devices/)

linuxct 指出，为了触发这些壁纸的动画，你需要去年的 [ROG Phone 3 动态壁纸端口](https://www.xda-developers.com/download-asus-rog-phone-3-live-wallpapers/)中的 X-Mode toggler。您可以通过下面的链接下载它。这个应用程序添加了一个快速设置磁贴，欺骗实时壁纸，使其认为 X 模式处于活动状态。这将触发动态壁纸外观的变化。你将需要这个应用程序的实时壁纸工作，因为打算在非 ROG 设备。

**下载:[无人机探测实时壁纸 APK](https://www.apkmirror.com/apk/linuxct/drones-of-detection-linuxcts-mod/drones-of-detection-2-1-0-0-5_210702-release/drones-of-detection-1-0-0-5_210702-2-android-apk-download/)|[星际飞船实时壁纸 APK](https://www.apkmirror.com/apk/linuxct/star-ship-linuxcts-mod/star-ship-2-1-0-0-13_210224-release/star-ship-1-0-0-13_210224-2-android-apk-download/)|[X-Mode APK](https://www.apkmirror.com/apk/linuxct/x-mode/x-mode-2-0-release/x-mode-2-0-android-apk-download/)|**

在设备上安装应用程序后，打开命令提示符或终端窗口，输入以下 ADB shell 命令:

```
 adb shell pm grant space.linuxct.rogcontroller android.permission.WRITE_SECURE_SETTINGS 
```

如果您的系统上没有安装 ADB，请查看本教程开始使用。