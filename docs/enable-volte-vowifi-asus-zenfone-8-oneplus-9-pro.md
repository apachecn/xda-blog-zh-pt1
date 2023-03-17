# 如何在华硕 ZenFone 8 和一加 9 Pro 上启用 VoLTE/VoWiFi

> 原文：<https://www.xda-developers.com/enable-volte-vowifi-asus-zenfone-8-oneplus-9-pro/>

当你面对不断发展的网络技术时，经常会遇到手机服务提供商和你的手机之间的问题。对于基于 IP 多媒体子系统(IMS)的高级蜂窝功能来说尤其如此，如 LTE 语音(VoLTE)、LTE 视频(ViLTE)和 Wi-Fi 呼叫(VoWiFi)。因此，在你闪亮的新手机和你选择的运营商之间，不可避免地会有一些混淆，什么有用，什么没用。不过，值得庆幸的是，XDA 社区的成员喜欢四处打探，想出简便的方法来克服这些障碍。这正是华硕 ZenFone 8 和 T2 一加 9 Pro 的情况，因为我们现在可以使用一些方法来支持这两款旗舰智能手机在不支持的运营商上支持 VoLTE 和 VoWiFi。

## ASUS ZenFone 8

华硕 ZenFone 8 已经成功回头率，成为智能手机生态系统的一个令人耳目一新的惊喜。ZenFone 8 是台湾 OEM 厂商的新一代“紧凑型”旗舰设备，具有 120Hz AMOLED 显示屏，左上角有一个用于自拍相机的打孔，高达 16GB 的 LPDDR5 RAM，高达 256GB 的 UFS 3.1 存储，以及更新的 ZenUI 皮肤，通过传统的 Android 11 界面保持简单，这款手机与华硕以前推出的任何产品都有明显不同。

 <picture>![There are few small phones on the market with flagship specifications, but the ASUS ZenFone 8 is one of those rare devices. Surprisingly, it doesn't skimp on battery life or performance and doesn't cost a fortune, either.](img/fd0c94dde9a90388d09bc68fba2335f5.png)</picture> 

ASUS ZenFone 8

##### Asus Zenfone 8

市场上很少有旗舰规格的小型手机，但华硕 ZenFone 8 是那些罕见的设备之一。令人惊讶的是，它并不吝啬电池寿命或性能，也不贵。

华硕已经为 ZenFone 8 推出了几个软件更新，其中最新的[在几家欧洲运营商上引入了](https://www.xda-developers.com/asus-zenui-update-zenfone-8-6-rog-phone-5-3/)官方 VoLTE 支持。由于运营商认证是一个漫长的过程，你可能想使用之前演示的“setprop”方法强制启用 VoLTE/VO wifi[——却发现它在这款手机上不起作用。](https://www.xda-developers.com/how-to-enable-t-mobile-volte-vowifi-on-asus-smartphones-root/)

不用担心，因为 XDA 认识到开发者已经设法解决了这个难题。事实证明，ASUS 决定更改变量名，因此 setprop 命令需要修改一点。

### 在华硕 ZenFone 8 的设置中启用 VoLTE/VoWiFi

1.  解锁设备的引导加载程序，并通过使用 Magisk 修补股票引导映像,[获得 root 访问权限](https://www.xda-developers.com/root/)。
2.  使用手机上的 ADB 或终端模拟器应用程序启动提升的 shell。为此，您需要在命令提示符下键入 su，并通过 Magisk 授予 root 访问权限。
3.  执行以下命令:

    ```
     setprop persist.dbg.volte_avail_ovr 1
    setprop persist.dbg.vt_avail_ovr 1
    setprop persist.dbg.wfc_avail_ovr 1 
    ```

4.  进行完全重启。
5.  现在你应该在设置中得到 VoLTE/VoWiFi 选项。

请记住，仅切换选项可能不足以获得 VoLTE/VoWiFi 服务。只有当 ZenFone 8 在其调制解调器固件中包含适合您的运营商的配置数据时，本教程才会起作用。

**[【ASUS zenfone 8 论坛】](https://forum.xda-developers.com/f/asus-zenfone-8.12291/)**

* * *

## 一加 9 专业版

一加 9 Pro 是一加最新的旗舰产品，也是该公司迄今为止最好的智能手机。你甚至可以在手机[上以测试版](https://www.xda-developers.com/oneplus-9-9-pro-android-12-beta/)的形式运行 [Android 12](https://www.xda-developers.com/android-12/) 。由于 VoLTE 的修补友好性，它的激活部分也非常简单。

 <picture>![The OnePlus 9 Pro is a really fast 2021 flagship that still keeps up well today. ](img/e87b0190e6eaa03a7cf726cd74516288.png)</picture> 

OnePlus 9 Pro

##### 一加 9 专业版

凭借 6.7 英寸的大尺寸四高清有机发光二极管显示屏和智能 120Hz 刷新率，一加 9 Pro 可能拥有市场上最好的显示屏。与 Hasselblad 合作调整的相机可拍摄出出色的静态照片，并捕捉精彩的 4K 视频。

与华硕 ZenFone 8 不同，你可以在一加 9 Pro **上强制启用 VoLTE 和 VoWiFi，而无需 root 访问权限**。这是可能的，因为一些官方一加工具允许您访问高通骁龙调制解调器的内部诊断接口，并手动设置所需的参数，以支持高级 IMS 服务。

### 在一加 9 专业版上启用 VoLTE/VoWiFi

1.  1.  从这个线程中获取一加日志包和一加工程模式 APKs [。](https://forum.xda-developers.com/t/working-method-to-enable-volte-and-vowifi-using-pdc-no-root.4270327/post-84960073)
    2.  手动安装两个 APK 文件。
    3.  打开手机 app，拨`*#800#`，选择工程模式。
    4.  进入 OnePlusLogKit 后，向下滚动一点，检查“VoLTE 开关”和“VoWifi 开关”选项。您可能还需要检查某些运营商的“VT 开关”。
    5.  重新启动。
    6.  打开设置并启用 VoLTE 和 VoWiFi。
    7.  再次打开手机 app，拨`*#801#`，选择工程模式。
    8.  点击“全端口开关”选项将其打开。
    9.  打开 USB 调试，将手机连接到 PC。确保 ADB 安装正确。
    10.  执行以下命令，重启进入现场测试模式:

        ```
         adb reboot ftm 
        ```

    11.  现在启用调制解调器的调试接口:

        ```
         adb shell
        setprop sys.usb.config diag,diag_mdm,qdss,qdss_mdm,serial_cdev,dpl,rmnet,adb 
        ```

        *   您可能需要安装所需的驱动程序，以便 Windows 可以识别新的接口。

    12.  现在我们需要使用高通制造的软件 PDC。为此，[下载并安装 QPST 软件套件](https://forum.xda-developers.com/t/working-method-to-enable-volte-and-vowifi-using-pdc-no-root.4270327/post-84960107)。
    13.  打开 PDC，选择配置文件(sub0 和 sub1)，然后单击激活。
    14.  关闭 PDC。
    15.  重新启动到正常模式:

        ```
         adb reboot 
        ```

    16.  在你的一加 9 Pro 上享受 VoLTE！

**[一加九大职业论坛](https://forum.xda-developers.com/f/oneplus-9-pro.12153/)**

* * *

这就是了。请随意在您的华硕 ZenFone 8 或一加 9 Pro 上尝试这些方法，无需等待您的运营商即可体验 VoLTE！