# 开发者在一加 6T 上启动 Windows 11

> 原文：<https://www.xda-developers.com/windows-11-boot-on-oneplus-6t/>

上周，微软正式发布了 Windows 11。虽然公众[要到今年年底](https://www.xda-developers.com/microsoft-teased-windows-11-launch-date/)才能看到，但[Windows 11](https://www.xda-developers.com/windows-11-preview-live/)的首个预览版已经面向 Windows 内部人士发布。除了大多数用户已经安装的 x64 版本，还有用于 Surface Pro X 等 ARM 设备上的 Windows 的 ARM64 版本。ARM64 版本旨在安装在支持[的高通处理器](https://www.xda-developers.com/cpus-compatible-windows-11/)上，但这并没有阻止修补程序使用它将 Windows 11 移植到不支持的设备上。

几天前，我们看到开发人员设法让 Windows 11 在 Lumia 950 XL 和 Raspberry Pi 4 上运行。现在，一些开发者已经在安卓手机上安装了 Windows 11。一些支持[叛徒项目](https://github.com/edk2-porting)的开发人员——一个将 EDK2 移植到[各种平台](https://github.com/edk2-porting/edk2-sdm845)的团队——成功地让 Windows 11 在 OnePlus 6 和一加 6T 上启动。其中一名团队成员分享了一段视频，我们在下面嵌入了该视频，展示了在一加 6T 上安装 ARM 上的 Windows 11。

视频显示用户 *edi194* 使用已经在 ARM 上运行 Windows 10 的一加 6T。然后，用户继续在 ARM 上刷新 Windows 11 的预览版，尽管安装需要花费很长时间，但手机最终还是成功启动了新的操作系统。据用户报告，触摸屏、USB 和 GPU(部分)等功能正在工作。不过 Wi-Fi，蓝牙，音箱上的音响好像坏了。

它远非完美，但看到微软全新的、成熟的桌面操作系统在为运行 Android 而设计的智能手机上运行，仍然很酷。

该团队还整理了一份他们在 OnePlus 6/6T 上测试的游戏的[电子表格。令人惊讶的是，一加 6T 可以处理相当多的 PC 游戏，包括 *GTA IV* 、 *CS:GO* 、 *Far Cry* 、*《我的世界》*、*极品飞车:通缉犯*、*模拟城市 5* 等等。](https://docs.google.com/spreadsheets/d/1XYuoySgYQE0HL573sA-0RGMX7I4lt5rWJuQ8Z8yRJNY/edit#gid=0)

当然，这不是我们第一次看到有人在骁龙 845 驱动的设备上运行 Windows。早在 2019 年，巴斯·蒂莫尔(用户名为 *NTAuthority* ) [设法在一加 6T](https://www.xda-developers.com/windows-10-arm-oneplus-6t/) 和谷歌 Pixel 3 上启动 Windows 10。

如果你有兴趣了解更多关于这个项目的信息，或者试着自己在骁龙 845 驱动的设备上启动 Windows，你可以从网站上了解更多关于 Renegade 项目的信息。同时，你可以在这里找到它的 GitHub [页面](https://github.com/edk2-porting/edk2-sdm845)。