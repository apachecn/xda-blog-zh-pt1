# 如何用 MIUI 在小米、米、红米、POCO 智能手机上安装安卓更新

> 原文：<https://www.xda-developers.com/how-to-install-stock-official-miui-android-update-xiaomi-mi-redmi-smartphones/>

# 如何用 MIUI 在小米、米、红米、POCO 智能手机上安装安卓更新

按照这些说明在小米，小米，红米和 POCO 智能手机上安装 Android 更新/股票 MIUI 恢复和快速启动 rom。

库存 ROM 更新适用于所有小米、小米和红米智能手机，有两种格式:恢复 ROM 和快速启动 ROM。顾名思义，恢复 rom 需要通过恢复或者通过本地更新的方式来安装，而快速启动 rom 需要使用 MiFlash 工具通过快速启动来安装。

所有[小米、mi、Redmi，甚至 POCO 智能手机](https://www.xda-developers.com/best-xiaomi-phones/)的使用说明都是通用的。我们为小米的 MIUI 12 和 MIUI 12.5 维护了[恢复 ROM 和快速启动 ROM 数据库，所以你可以从那里获得所有地区和版本的所有支持手机的下载链接。](https://www.xda-developers.com/download-miui-12-stable-update-rolling-out-several-xiaomi-redmi-mi-poco-devices/)

## 从安装中恢复

恢复光盘带有. zip 文件扩展名，可以通过 MIUI 中的本地更新方法进行安装。您也可以使用自定义恢复来安装这些 rom，但请注意，在这种情况下，特定于设备的说明可能会有所不同。

1.  传输下载。zip 文件到您的手机，并确保您将该文件放在设备内部存储器的“downloaded_rom”文件夹中。如果不存在这样的文件夹，请在您的内部存储基本目录中创建一个。
2.  在手机上，导航至“设置”>“关于手机”>“系统更新”,然后按右上角的三点图标，选择“选择更新包”。如果看不到“选择更新包”，需要轻敲 MIUI 版本 logo 7-10 次。
3.  如果“选择更新包”选项丢失，请轻按 MIUI 徽标 10 次以激活该选项。
4.  选择下载的。zip 文件。
5.  等待更新安装。

* * *

## 快速启动 ROM 安装

快速启动 rom 带有一个. tgz 文件扩展名，并且需要一台 Windows 计算机来安装 MiFlash 工具，以及一台带有解锁引导加载程序的电话。然而，尽管安装起来比恢复 rom 相对复杂，快速启动 rom 有时是启动到工作系统的唯一方法。有关解锁手机引导程序的说明，请查看 XDA 上的手机子论坛。您可以使用 Fastboot 二进制文件本身来执行刷新过程，在这种情况下，Fastboot ROM 可以在 Windows、Linux 以及 macOS 上使用。

1.  在您的 Windows 计算机上下载 MiFlash 工具。最新版本可以在本链接的步骤 1 [中找到。下载完成后，解压并安装该工具。也建议安装 ADB 和 Fastboot，以防万一。](https://c.mi.com/oc/miuidownload/detail?guide=2)
2.  关闭手机，然后同时按下电源和音量键，重新启动手机进入下载模式。
3.  使用合适的 USB 数据线将手机连接到电脑。
4.  下载快速启动 ROM。tgz 文件并提取它。记住提取位置，因为您需要将地址粘贴到 MiFlash 工具中。
5.  在您的 Windows 计算机上运行 MiFlash 工具，并在该工具的地址栏中粘贴步骤 4 中的提取位置。
6.  单击 MiFlash 中的“刷新”,应用程序将自动识别您的设备。
7.  单击 MiFlash 中的“运行”,将 ROM 文件闪存到设备中。
8.  MiFlash 中的进度条会变成绿色，表示 ROM 安装成功。您的设备应该会自动启动到新版本。