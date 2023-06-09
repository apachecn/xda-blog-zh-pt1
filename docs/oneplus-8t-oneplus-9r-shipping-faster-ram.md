# 较新的一加 8T 和一加 9R 装置配有更快的内存

> 原文：<https://www.xda-developers.com/oneplus-8t-oneplus-9r-shipping-faster-ram/>

一加 8T T1 大约在一年前发布，是 2020 年下半年唯一的一加旗舰手机(“T”型号通常会有一个额外的 Pro 版本)。这款手机在今年早些时候进行了小幅升级，并作为[一加 9R](https://www.xda-developers.com/oneplus-9r-launch/) 与其余的[一加 9](https://www.xda-developers.com/oneplus-9/) 系列一起发布。两款手机都配备了 LPDDR4X 内存，但一加悄悄地将两款手机都换成了更快的 LPDDR5 RAM 模块。

一加 8T 配备了 8GB 或 12GB 的 RAM(取决于你选择的型号)，官方规格表[仍然说](https://onepluscom.pxf.io/c/2233363/916678/12532?subId1=UUxdaUeUpU4223&subId2=exda&u=https%3A%2F%2Fwww.oneplus.com%2F8t%2Fspecs%23%3A%7E%3Atext%3DLPDDR4X)这款手机使用 LPDDR4X RAM。一加 9R 的同一页从未提到所用的具体 RAM 类型，但独立测试后来证实，它也配有 LPDDR4X RAM。

然而，一些买家发现他们的设备具有更快的 LPDDR5 内存，尽管一加从未宣布它已在一加 8T/9R 上改用更快的 RAM。当他们试图使用 MSMDownloadTool 取消绑定他们的 [8T](https://www.xda-developers.com/oneplus-8t-kernel-source-code-unbrick-tool/) 或 [9R](https://www.xda-developers.com/oneplus-9-9-pro-9r-unbrick-msmdownloadtool/) 时，这种差异变得很明显，由于不兼容的 XBL(可扩展引导加载程序)映像，MSMDownloadTool 与 LPDDR5 变种不兼容。LineageOS 的固件更新指令已经根据 RAM 类型更新为不同的可闪存映像。

很容易判断出你的一加 8T 或 9R 使用的是哪种内存类型。如果您的 PC 上安装了 ADB，在连接了一加 8T 或 9R 的情况下运行以下命令，它会为 LPDDR4X RAM 返回 0，为 LPDDR5 RAM 返回 1。你也可以使用 [Termux](https://play.google.com/store/apps/details?id=com.termux) 在手机上运行该命令，但你不必键入“亚行外壳”部分。

```
 adb shell getprop ro.boot.ddr_type 
```

XDA 的 Aamir Siddiqui 在他的一加 9R 审查单元上测试了它，它有 LPDDR5 RAM。相比之下，XDA 的米沙·拉赫曼在 1 月下旬购买的零售一加 8T 单元具有宣传的 LPDDR4X RAM。

过去有许多看似相同的手机内部硬件比其他设备更好或更差的案例，例如 [Galaxy S8 的不同内部存储](https://www.xda-developers.com/the-hardware-lottery-continues-with-the-samsung-galaxy-s8s8-varying-between-ufs-2-1-and-ufs-2-0/)和旧款 iPhones 中的[不同调制解调器](https://forums.macrumors.com/threads/definitive-qualcomm-a1660-a1661-v-intel-a1778-a1784-iphone-7-7-plus-thread.1998028/)。然而，大多数人可能无法区分这两种 RAM 类型。

我们已经就此事向印度一加求证，如果有回音，我们会更新这个帖子。