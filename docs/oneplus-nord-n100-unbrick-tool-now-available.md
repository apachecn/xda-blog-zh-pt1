# 一加诺德 N100 解锁工具现已上市

> 原文：<https://www.xda-developers.com/oneplus-nord-n100-unbrick-tool-now-available/>

一加度过了忙碌的 2020 年。除了常规产品，这家中国原始设备制造商还通过一加诺德 N10 5G 和一加诺德 N100 涉足廉价智能手机市场。对钱包友好的 Nord N100 可能不是一个仅支持 4G 的高通骁龙 460 SoC 的发电站，但它确实与它的兄弟姐妹有一些共同点:[90Hz 刷新率的显示器](https://www.xda-developers.com/oneplus-nord-n100-90hz-display/)，可解锁的引导加载器用于修补，最后但并非最不重要的是，能够在用户触发时启动进入高通的紧急下载模式([即 EDL](https://www.xda-developers.com/exploit-qualcomm-edl-xiaomi-oneplus-nokia/) )。嗯，谁不知道 EDL 闪光灯(通常被称为“MsmDownloadTool”)的容易获得是大多数一加设备在很大程度上不可点击的原因？

**[一加诺德 N100 XDA 论坛](https://forum.xda-developers.com/c/oneplus-nord-n100.11817/)**

如果您有一台一加诺德 N100，不禁想知道为什么您的设备还没有 unbrick 工具，我们很高兴地通知您，您的等待结束了。我们最喜欢的一加爱好者 [Some_Random_Username](https://forum.xda-developers.com/m/some_random_username.8234677/) 已经成功镜像了特定于设备的 MsmDownloadTool 软件包，并编写了一个指南，解释了自己完全恢复一个被阻塞的 Nord N100 需要哪些步骤。

**[下载一加诺德 N100](https://forum.xda-developers.com/t/opn100-oos-83ba-unbrick-tool-to-restore-your-device-to-oxygenos.4217855/)** 的 MsmDownloadTool

如果你的一加诺德 N100 已经被屏蔽了，把它连接到运行 Windows 的 PC 上的 USB 端口应该会在设备管理器下显示为“QDLOADER 9008”(或者“QHUSB_BULK”，如果所需的驱动程序没有正确安装的话)。要手动触发 EDL 模式，按住音量增大和音量减小按钮，并将手机插入 PC。

在使用该工具拆卸一加诺德 N100 之前，需要注意一些注意事项。最重要的是，如果您希望在闪存过程中交叉闪存 OxygenOS 的不同区域版本，这将不起作用，因为低级固件现在绑定到内部设备区域 ID。此外，由于一加在构建闪光器时利用 [VMProtect 3.0](https://vmpsoft.com/20150825/vmprotect-3-0/) 作为混淆/反调试措施，您的防病毒软件可能会将其标记为潜在的流氓软件。这是一个典型的假阳性案例，所以只需忽略警告，并将该工具添加到反病毒程序的排除列表中。