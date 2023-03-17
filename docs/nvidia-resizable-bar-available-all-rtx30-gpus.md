# NVIDIA 可调整大小的酒吧现已提供给所有 GeForce RTX 30 桌面图形处理器

> 原文：<https://www.xda-developers.com/nvidia-resizable-bar-available-all-rtx30-gpus/>

# NVIDIA 可调整大小的酒吧推出所有 RTX 30 系列图形处理器，这里的如何使它对你自己的

NVIDIA 已经正式在其所有 GeForce RTX 30 系列台式机显卡上启用了可调整大小栏，下面是如何启用它的方法！

在推出新的 GeForce RTX 30 系列桌面显卡期间，NVIDIA 宣布将推出 Resizable BAR，这是一种基于 PCIe 的技术，允许用户使用兼容的主板，使 CPU 能够同时访问所有的 GPU 内存。与 AMD 的智能访问内存类似，这意味着更快的数据传输，包括纹理、着色器和几何图形，从而在游戏时提供约 10-20%的增益。

这项技术最初于 2021 年 2 月启用，当时 NVIDIA 开始发运 [GeForce RTX 3060](https://www.xda-developers.com/nvidia-geforce-rtx-3060-official/) ，这是该系列中最实惠的选项。现在公司已经[正式启用了对所有 RTX 30 系列的](https://www.nvidia.com/en-us/geforce/news/geforce-rtx-30-series-resizable-bar-support/)支持，包括 RTX 3090、RTX 3080、RTX 3070 和 RTX 3060 Ti。除了受支持的主板，NVIDIA 还分享了一个支持 Resizable BAR 的 CPU 列表，所以除非你有 GPU、CPU 和主板的正确组合，否则你无法利用这项技术。

此外，只有少数游戏可以使用可调整大小的酒吧，这些包括:

*   刺客信条瓦尔哈拉
*   战地 V
*   边疆 3
*   控制
*   赛博朋克 2077
*   死亡搁浅
*   污垢 5
*   F1 2020
*   极限地平线 4
*   齿轮 5
*   戈弗尔
*   刺客 2
*   杀手 3
*   地平线零黎明
*   地铁大逃亡
*   红色死亡救赎 2
*   看门狗军团

## 如何在你的电脑上启用可调整大小栏？

1.  如前所述，你首先需要检查你是否有兼容的 CPU 和主板芯片组组合。以下是 NVIDIA 分享的所有支持的:
    1.  **主板:**
        1.  AMD 400 系列
        2.  AMD 500 系列
        3.  英特尔 Z490
        4.  英特尔 H470
        5.  英特尔 B460
        6.  英特尔 H410
        7.  所有支持第 11 代英特尔处理器的主板
    2.  **CPU:**
        1.  AMD 锐龙 3 5xxx
        2.  AMD 锐龙 5 5xxx
        3.  AMD 锐龙 7 5xxx
        4.  AMD 锐龙 9 5xxx
        5.  英特尔酷睿 i9-10xxx
        6.  英特尔酷睿 i7-10xxx
        7.  英特尔酷睿 i5-10xxx
        8.  英特尔酷睿 i3-10xxx
        9.  英特尔酷睿 i9-11xxx
        10.  英特尔酷睿 i7-11xxx
        11.  英特尔酷睿 i5-11xxx
2.  接下来，确保您已经更新到最新的主板 BIOS，如果需要，通过安装制造商提供的更新。然后转到 BIOS 界面，启用可调整大小栏支持。
3.  更新到最新的 GeForce 游戏就绪驱动程序(版本 465.89 WHQL 或以上)。
4.  如果您拥有 GeForce RTX 3060 Ti、3070、3080 或 3090，那么您可能需要更新的 VBIOS。Founders Edition 显卡的所有者可以直接从他们的网站上使用 NVIDIA 的工具进行更新。
5.  如果您拥有定制的合作伙伴卡，可以通过访问特定制造商的网站来下载每个显卡的固件更新。
    1.  [华硕](https://rog.asus.com/graphics-cards-group/):选择 GeForce RTX 30 系列- >型号- >支持- >驱动&实用程序
    2.  [五彩缤纷](https://en.colorful.cn/event/BAR/index.html)
    3.  [EVGA](https://www.evga.com/articles/01478/geforce-rtx-30-series-gpu-resizable-bar/)
    4.  [增益](https://www.gainward.com/main/download.php?lang=en):选择 GPU - >工具
    5.  [Galax](https://www.galax.com/bar-gtm-update)
    6.  [千兆字节](https://www.gigabyte.com/WebPage/785/NVIDIA_resizable_bar.html)
    7.  [INNO3D](https://www.inno3d.com/static.php?langid=1&refid=22)
    8.  [MSI](https://www.msi.com/Graphics-Cards#?tag=GeForce-RTX%26trade%3B-3090) :选择 GPU - >支持- >实用工具- >选择 MSI 龙中心或者 MSI Live 更新
    9.  [Palit](https://www.palit.com/palit/download.php?lang=en) :选择 GPU - >工具
    10.  [PNY](https://www.pny.com/company/support/nvidia-geforce#BARBIOSUpdate)
    11.  Zotac

要验证是否启用了可调整大小栏，请打开 NVIDIA 控制面板。在 NVIDIA 控制面板的左下方，点击“系统信息”,在新窗口中寻找右边的“可调整大小栏”。如果它说“是”，你就可以走了。