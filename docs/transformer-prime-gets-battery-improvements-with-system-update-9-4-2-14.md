# 如何自定义 Android 内置的省电模式

> 原文：<https://www.xda-developers.com/transformer-prime-gets-battery-improvements-with-system-update-9-4-2-14/>

Android 内置电池省电模式已经很多年了。如果你的手机快没电了，你可以激活它，让手机多运行几个小时。电池保护程序禁用了相当多的耗电功能，并调整了一系列设置以延长电池寿命。虽然它对大多数人来说很有用，但有些人可能想调整它，使它不关闭某些设置或使它更积极地节省电池。如果这样描述你，那么这里有一个关于如何定制 Android 的电池节电模式的教程。

在我们开始之前，我们需要解释一下节电模式实际上是做什么的。[根据谷歌支持页面](https://support.google.com/pixelphone/answer/6187458#what_changes&zippy=%2Cwhat-battery-saver-limits)，以下是 Pixel 手机的电池保护限制:

### 什么电池节电限制

*   只有当你打开应用程序时，应用程序才会刷新它们的内容，如电子邮件或新闻。
*   当您的屏幕关闭时，定位服务会停止。
*   应用程序不会在后台运行，除非您关闭电池优化。
*   您的手机无法接听“Ok Google ”,无法继续对话。相反，每次点击谷歌助手。
*   黑暗主题开启。
*   您的通知可能会延迟。
*   “总是显示时间和信息”将关闭。
*   带有 Active Edge 的 Pixel 手机不会对挤压做出反应。
*   在 Pixel 3、Pixel 4 以及更高版本的 Pixel 手机上，汽车碰撞检测功能会关闭。
*   在 Pixel 4 手机上，运动感应关闭。
*   在 Pixel 4 和更高版本的 Pixel 手机上，平滑显示关闭。
*   5G 的 Pixel 手机回落到 4G 服务。

(谷歌 Pixel 3 和更高版本独有的是一个更强大的[极端电池节省模式](https://www.xda-developers.com/google-pixel-5-review/#:~:text=extreme%20battery%20saver%20option)，但鉴于这是一个 Pixel 专有的功能，我们不会进一步谈论它。)

上面显示的列表实际上是不完整的:Android 手机上的电池节省模式实际上比谷歌在支持页面上所说的更多。事实上，电池保护程序还会禁用应用启动增强、振动和动画等功能，并且还会限制面板的最大亮度。由于 Android 的电池节电模式是[开源](https://android.googlesource.com/platform/frameworks/base/+/master/services/core/java/com/android/server/power/batterysaver/BatterySaverPolicy.java)的，并且可以通过设置表的命令行界面[来控制，因此可以调整电池节电模式，使其在禁用的方面更积极或更不积极。](https://android.googlesource.com/platform/frameworks/base/+/master/core/java/android/provider/Settings.java#11478)

## 自定义安卓的省电模式

### 方法 1 -亚行外壳

1.  遵循[这个指南](https://www.xda-developers.com/install-adb-windows-macos-linux/)在你的电脑上设置 ADB 或者阅读[这篇文章](https://www.xda-developers.com/debloat-your-phone-run-adb-shell-commands-no-root-no-pc)来学习如何设置一个本地 ADB 外壳。
2.  ADB 启动并运行后，打开命令提示符或终端窗口，在 shell 中运行以下命令:

    ```
     settings put global battery_saver_constants "advertise_is_enabled=BOOLEAN,datasaver_disabled=BOOLEAN,enable_night_mode=BOOLEAN,launch_boost_disabled=BOOLEAN,vibration_disabled=BOOLEAN,animation_disabled=BOOLEAN,soundtrigger_disabled=BOOLEAN,fullbackup_deferred=BOOLEAN,keyvaluebackup_deferred=BOOLEAN,firewall_disabled=BOOLEAN,gps_mode=INTEGER,adjust_brightness_disabled=BOOLEAN,adjust_brightness_factor=FLOAT,force_all_apps_standby=BOOLEAN,force_background_check=BOOLEAN,optional_sensors_disabled=BOOLEAN,aod_disabled=BOOLEAN,quick_doze_enabled=BOOLEAN" 
    ```

    其中 BOOLEAN 是`true`或`false`，INTEGER 是整数，FLOAT 是小数。
3.  如果您想知道 battery saver 模式下的参数当前设置为什么，您可以运行以下 ADB shell:

    ```
     dumpsys power | grep -A 128 "Battery saver policy" 
    ```

    这将显示当前的 battery saver 策略和所有参数值。或者，您可以检查:

    ```
     settings get global battery_saver_constants 
    ```

    的输出...但是，只有在您对该设置值进行了至少一次更改之后，它才会被填充。
4.  如果您想将节电模式恢复到默认参数，那么您可以运行

    ```
     settings delete global battery_saver_constants 
    ```

    或

    ```
     settings put global battery_saver_constants "advertise_is_enabled=true,datasaver_disabled=true,enable_night_mode=true,launch_boost_disabled=true,vibration_disabled=true,animation_disabled=false,soundtrigger_disabled=true,fullbackup_deferred=true,keyvaluebackup_deferred=true,firewall_disabled=true,gps_mode=2,adjust_brightness_disabled=true,adjust_brightness_factor=0.5,force_all_apps_standby=true,force_background_check=true,optional_sensors_disabled=true,aod_disabled=true,quick_doze_enabled=true" 
    ```

自从我们上次讨论了如何通过命令行调整 Android 内置的电池节省模式之后，一个开发者开发了一个应用程序，它提供了一个 GUI 来改变这些参数。如果您不想手动运行 shell 命令和/或查看 AOSP 来找出每个参数的确切作用，那么请继续阅读。

### 方法 2 -浮标应用程序

XDA 认可的开发者 [tytydraco](https://forum.xda-developers.com/m/tytydraco.8155542/) ，我们前几天报道的 [LADB 应用](https://www.xda-developers.com/debloat-your-phone-run-adb-shell-commands-no-root-no-pc)的开发者，带着另一个名为 Buoy 的应用回来了。它被描述为“内置 Android 电池节省程序的扩展”，它所做的是暴露 Android 的隐藏参数，以自定义电池节省模式的行为。该应用程序允许您切换以下内容:

*   向其他应用通告低功耗模式已启用
*   Android 的计量 WiFi 或移动数据连接的数据保护程序
*   内置黑暗模式
*   启动 boost 以加速应用启动
*   震动
*   显示窗口和活动动画
*   允许应用程序使用声音触发器 HAL
*   将完整设备备份推迟到以后
*   将应用程序设置备份推迟到以后
*   使用内置的 web 防火墙来防范可能的恶意站点
*   更改应用程序的位置访问模式限制
*   降低面板的最大亮度
*   强制所有应用程序进入待机模式
*   强制所有应用程序不在后台检查数据
*   禁用不必要的传感器
*   使用永远显示
*   屏幕一关闭，设备就进入深度睡眠状态

它还可以让你切换“粘性”低功耗模式，这是 Android 9 Pie 中添加的一个功能[，当设备被拔掉电源或重新启动时，它可以让电池节电模式自动重新启用。](https://twitter.com/MishaalRahman/status/1040351524378079233)

为了使用 Buoy，你需要一台运行 Android 8.0 Oreo 或更高版本的 Android 设备，尽管可用参数会因 Android 版本而异。此外，您必须授予应用程序 WRITE_SECURE_SETTINGS 权限或 root 访问权限，才能更改设置值。Global.battery_saver_constants。我再一次向你推荐我们关于[如何建立 ADB](https://www.xda-developers.com/install-adb-windows-macos-linux/) 或 [tytydraco 的 LADB 应用](https://www.xda-developers.com/debloat-your-phone-run-adb-shell-commands-no-root-no-pc)的文章，这样你就能做到。

如果您安装该应用程序并进行任何更改，请注意卸载该应用程序时更改不会自动恢复。你必须点击 Buoy 中的“reset”按钮，或者发送之前步骤 4 中提到的命令之一，以便将电池节电模式的参数恢复为默认值。

在美国，Buoy 在 Google Play 上售价 0.99 美元，但它也是开源的，所以如果你愿意，你可以自己编译它。或者，你可以像我前面提到的那样，手动设置节电模式参数。如果你想让事情变得更简单，并支持开发者，那么你可以从 Play Store 购买应用程序。如果您有任何问题或反馈，请查看下面链接的 XDA 论坛上的开发人员帖子。

**[浮标- XDA 论坛线程](https://forum.xda-developers.com/t/meet-buoy-a-foss-battery-saver-configuration-tool.4258757/#post-84906249)**