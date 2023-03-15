# 超级用户| XDA 开发人员

> 原文：<https://www.xda-developers.com/superuser-updated-to-v2-2-1/>

[](/kernelsu-gki-root/)

Magisk 的继任者终于来了？

在 Android 的修改圈子里，没有比 [Magisk](https://www.xda-developers.com/how-to-install-magisk/) 更知名的应用了。它有着实至名归的声誉，是 T2 为你的手机、平板电脑以及几乎所有运行安卓系统的东西提供支持的事实上的标准。虽然 Magisk 成功地将自己确立为 [Chainfire 的 SuperSU](https://www.xda-developers.com/chainfire-ending-development-root-apps/) 的继任者，但售后市场开发社区在过渡阶段偶然发现了多种根本解决方案。除了那些著名的，例如认可的开发者 phhusson 的超级用户，我们也遇到了一些独特的实现，例如认可的开发者 Jason Donenfeld 的内核辅助超级用户。

[](/wsl-sudo-windows-hello/)

这个开源应用程序允许您使用 Windows Hello 的生物识别登录来验证在 Windows Subsystem for Linux (WSL)下发出的 sudo 请求。

Linux 的 Windows 子系统(WSL)是 Windows 10 的重要组成部分。WSL 最初是为开发人员构建 web 和云应用程序而设计的，如今它变成了一种更强大的东西，将两种截然不同的操作系统结合在一起。自 [WSL 2](https://www.xda-developers.com/microsoft-windows-10-may-2020-update-wsl-2-revamped-cortana-assistant-your-phone-calls-arm-devices/) 以来，Linux 层由微软 Hyper-V 虚拟化技术的变体提供支持，并且它配备了微软编译和支持的 Linux 内核。WSL 和底层 Windows 10 之间的集成非常灵活，人们可以很容易地从 Linux 命令行运行 Windows 工具，反之亦然。

[](/linux-update-sudo-security-flaw/)

Qualys 的研究人员在 Sudo 程序中发现了一个安全漏洞，利用该漏洞可以获得 Linux PCs 上的 root 访问权限！

尽管事实上成千上万的贡献者积极地仔细研究 Linux 内核和各种 Unix 实用程序的源代码，寻找安全缺陷，但未被注意到的严重错误并不是闻所未闻。就在一天前，Qualys 的人披露了一种新的基于堆的缓冲区溢出攻击向量，该向量以“Sudo”程序为目标来获得根访问权限。这次的 bug 好像还挺严重的，bug 在代码库内部已经存在了差不多 **10 年**！尽管特权提升漏洞已经被修补，但它仍有可能在**几乎所有的 Linux 发行版**和几个类似 Unix 的操作系统上被利用。

[](/lineageos-dropping-superuser-addonsu-implementation-favor-magisk-manager/)

LineageOS 17 将不再推荐自己的 addonsu 包，使得 Magisk 和 Magisk manager 成为超级用户二进制和管理的事实上的选择。

LineageOS 是 Android 设备上最受欢迎的定制 ROM 之一，如果不是最受欢迎的定制 ROM 的话。这个定制的 ROM 采用了 Android 开源项目(AOSP)中的 Android，并在其上添加了自己的特色。许多定制 ROM 倾向于采用 LineageOS 作为自己的基础，因此 LineageOS 为自己进行的任何重大更改都倾向于在整个定制 ROM 社区中传播。LineageOS 背后的开发人员意识到了这种影响，并据此做出明智的决策。LineageOS 即将发布的版本极大地改变了根访问的处理方式，因为 ROM 放弃了对自己的 addonsu 二进制文件的支持，转而支持 Magisk。

[](/chainfire-recommends-staying-in-supersu-2-79-for-xperia-users/)

很难想象没有 SuperSU 的 XDA。最流行和最基本的根应用程序多年来一直在 Android 设备上提供根访问和管理。不幸的是，最新版本并不能完全正常工作，所以 XDA 资深认可开发者 [Chainfire](https://forum.xda-developers.com/member.php?u=631273) 发表了一份声明来揭示这个问题。