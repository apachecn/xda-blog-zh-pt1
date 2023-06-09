# 英特尔发布首款支持 Windows 11 的显卡驱动程序

> 原文：<https://www.xda-developers.com/intel-releases-first-graphics-driver-with-support-for-windows-11/>

英特尔发布了最新版本的 Windows 图形驱动程序。这次更新将英特尔的驱动程序带到了版本号 30.0.100.9684，重大消息是它增加了对 [Windows 11](https://www.xda-developers.com/windows-11/) 的官方支持。

这意味着几件事。首先，这意味着这是第一个支持 Windows 显示驱动模型(WDDM) 3.0 的驱动程序。这也意味着它增加了对 Linux 的 Windows 子系统的官方支持。Windows 11 将增加对 GUI Linux 应用程序的支持，因此更新的驱动程序应该可以确保更好的性能。

Windows 11 的另一大新功能是游戏的自动 HDR，这个英特尔驱动程序也增加了对它的支持。自动 HDR 意味着超过一千个游戏可以获得 HDR 的一些好处，而不必为它编程。虽然不完全一样，但是如果你有 HDR 显示器的话，它会让游戏看起来更好。但是，该功能仅在英特尔 Iris Plus 显卡(第十代英特尔酷睿 CPU)或更高版本上受支持。

 <picture>![Luminance heatmap for Auto HDR and Native HDR](img/dfbd3622dfb0f65a197d90f7b216e363.png)</picture> 

Image credit: Microsoft

除了对 Windows 11 的支持，这个驱动程序还增加了对一个新游戏的支持， *F1 2021* 。还包括对*月光之刃*和*使命召唤:战区*中性能的一些优化。

当然，驱动程序还包括一堆针对各种游戏和特定场景的修复。这包括修复连接到外部 4K 显示器并尝试复制该显示器时的显示问题。在第 11 代英特尔酷睿 H 系列 CPU 上的电影和电视应用程序中播放 WMV 视频文件也有问题。您可以在下面看到完整的修复列表:

### 30.0.100.9684 版中修复的问题

*   英特尔 Iris Xe MAX 显卡:在堡垒之夜*发现轻微图形异常，Balan: Wonderworld*。
*   英特尔 Iris Xe MAX 显卡:在《刺客信条:瓦尔哈拉》(DX12)、《漫威的拯救者》(DX12)中出现间歇性崩溃或挂起。
*   在 50Hz 设置下，以 5120x2160 分辨率观察到空白显示。
*   在《夏德曼》翻拍版*(Vulkan)、《黑暗之魂 3》(Dark Souls III)、《新奥尔良黑帮》(Gangstar New Orleans)、《沃尔芬斯坦 2:新巨人》(wolfgenstein II):(Vulkan)、《坦克世界》(DX12)中看到的间歇性崩溃或挂起。
*   在 Dirt 5* (DX12)、Watch Dogs: Legion* (DX12)、Control* (DX12)、Far Cry: NewDawn*(从保存的文件开始时)、3DMark: FireStrike*中看到的轻微图形异常。
*   从睡眠或待机状态恢复后，HDMI 2.0 显示器无法亮起。
*   当 4K 监视器连接并切换到重复显示时，显示异常。
*   期间在内部面板上看到视觉异常。在第 11 代英特尔酷睿 H 系列移动处理器的高 CPU 使用率下，在电影和电视应用中播放 wmv 电影。

即使进行了这些修复，此版本仍存在一些已知问题。以下是你需要注意的一切:

### 30.0.100.9684 版中的已知问题

*   在《燃尽天堂重制》*、《使命召唤:黑色行动冷战* (DX12)》、《底特律:变成人类* (Vulkan)、《末日永恒* (Vulkan)》、《地铁出埃及记*(DX12)更改图形设置时、《月光之刃》(DX12)、《死灵世界:雇佣之枪》(DX12)(选择除低以外的阴影选项时)、《速度回报的需要》*、NBA 2K21* (DX12)(将分辨率从 1920 x 1080 切换到 1600 x 900 和 古墓丽影*(切换到 dx12 和 SMAA 4x 玩了 10 分钟后)，《斯派罗:重燃三部曲》*，《黑暗图片:棉兰之人》(inonline 模式)，《汤姆·克兰西的幽灵侦察断点》*，《战争雷霆》*。
*   在播放视频时，可能会在 Adobe Premiere Pro 2020*中观察到轻微的图形异常，《刺客信条》(Assassin ' s CreedValhalla)* (DX12)、《孤岛危机》(Crysis Remastered)、《赛博朋克 2077》(DX12)、《黑暗之魂 3》、《死亡搁浅》(Death Stranding)*(DX12)、《德乌斯人类分裂》(exhuman Divided *(DX12)、《末日永恒》(Vulkan)(游戏内菜单)、Elex*、Forza Horizon 4* (DX12)、《战争齿轮》(Gears ofWar)终极版*(DX12)、《刺客 2》(Hitman 2)、《地平线零点黎明》(DX12)、《正义事业 4
*   英特尔 Iris Xe MAX 显卡:在 Rage 2* (Vulkan)(进入主菜单时)、席德·梅尔的文明 VI*(在 ALT + ENTER 期间)、SMITE*、The Witcher 3*、Warframe* (DX12)中可能会出现间歇性崩溃或挂起。
*   英特尔 Iris Xe MAX 显卡:在《使命召唤:现代战争*(DX12)、《极限竞速 6》(DX12)、《网格 2019》(DX12)、《漫威复仇者联盟》(DX12)、《地铁出埃及记》(DX12)、《火箭联盟》(启用 CMAA 时)、《严肃山姆 4》(Vulkan)中可能会观察到轻微的图形异常。

你可能想从下载中心下载新的英特尔驱动程序[，尤其是如果你已经在运行 Windows 11 预览版的话。如果你还没有尝试，但你想尝试，你可以在这里跟随我们的指南](https://downloadcenter.intel.com/download/30579/Intel-Graphics-Windows-DCH-Drivers)[开始使用 Windows Insider 计划](https://www.xda-developers.com/how-to-prepare-pc-windows-11-beta/)。你也可以在这里阅读所有已经可以在 Windows 11 中试用的[。](https://www.xda-developers.com/windows-11-features-in-preview/)