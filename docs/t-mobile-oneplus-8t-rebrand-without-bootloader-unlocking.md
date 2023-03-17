# 重新命名 T-Mobile 一加 8T，无需解锁引导加载程序

> 原文：<https://www.xda-developers.com/t-mobile-oneplus-8t-rebrand-without-bootloader-unlocking/>

那些在 T-Mobile 上购买了一加 8T(以“一加 8T+ 5G”出售)并对该运营商较慢的更新速度感到失望的人现在可以高兴了。您现在可以摆脱 T-Mobile 软件，并在 T-Mobile 一加 8T 上安装国际 OxygenOS 固件，甚至无需解锁设备的引导加载程序！

**[一加 8T XDA 论坛](https://forum.xda-developers.com/c/oneplus-8t.11579/)**

刷新非运营商固件意味着将有更快的更新可用，将启用双 SIM 卡支持(如果您购买了新的 SIM 卡托盘)，并且您将可以访问 OxygenOS 的最新[公开测试版](https://www.xda-developers.com/tag/oxygenos-beta-program/)。要在 T-Mobile 一加 8T(型号 **KB2007** )上启用所有这些“功能”，您通常必须付清合同，在网络上使用设备至少 40 天，才有资格解锁引导加载程序，执行解锁操作，最后使用 Fastboot 交叉刷新全球、欧洲和印度固件。然而，感谢 XDA 资深会员[克拉兹纳兹](https://forum.xda-developers.com/m/craznazn.2147845/)的辛勤工作，你将不再需要这样做了。

为了简化流程， *craznazn* 想出了一个修改过的 [unbrick 包](https://www.xda-developers.com/oneplus-8t-kernel-source-code-unbrick-tool/)(俗称“MsmDownloadTool”)，在闪存时忽略硬件型号。优势是显而易见的:用户现在可以在锁定一加 8T 的引导加载程序上直接运行该工具，因为一加的 unbrick 工具不管引导加载程序解锁状态如何都可以工作。

## 如何在 T-Mobile 一加 8T 上安装国际固件

在 T-Mobile 一加 8T 上使用了修改后的 MsmDownloadTool 之后，你最终应该会得到欧洲的固件，它比印度的 OxygenOS 版本要少[。与 OxygenOS 的全球版本相比，欧盟固件仍然提供“本地升级”选项，这意味着用户可以轻松地交叉闪存他们选择的不同区域固件，而无需使用 PC。即使在转换之后，5G 频段和](https://www.xda-developers.com/oneplus-announces-india-specific-features-oxygenos/) [Widevine L1](https://www.xda-developers.com/check-widevine-drm-status-android/) 状态(网飞、Prime Video 和类似应用的高清流媒体所需的)也能按预期工作。

**注意:**下面概述的过程将会擦除您的手机。继续之前，请备份所有重要文件。这种方法不会为您提供 T-Mobile SIM 卡解锁。

1.  将修改后的 MsmDownloadTool 从[线程](https://forum.xda-developers.com/t/guide-convert-tmo-to-eu-via-msm-tool-no-sim-unlock-or-bootloader-unlock-needed.4188491/)下载到运行 Windows 的 PC 上。
2.  Run MsmDownloadTool V4.0.exe.
    *   Windows 7 用户可能需要运行该工具附带的 Windows 7 版本。
3.  选择“其他”作为用户类型，然后按下一步。
4.  不更改默认设置，按“开始”
5.  使用以下 ADB 命令将手机置于 EDL 模式:

    ```
     adb reboot edl 
    ```

    *   或者，完全关闭设备，按住调高音量和调低音量按钮，并使用 USB 电缆将其连接到 PC。
6.  等待刷新过程完成。
7.  尽情享受吧！

需要注意的一点是，转换过程不能完全填充“关于手机”页面。这纯粹是表面上的限制，但是如果这个小故障困扰着你，你可以从前面提到的线程下载一个特制的 Magisk 模块，并应用它来修复丢失的条目。