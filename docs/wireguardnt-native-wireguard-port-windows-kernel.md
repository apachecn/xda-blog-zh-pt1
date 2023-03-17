# WireGuard 正在获取 Windows 内核的本地端口

> 原文：<https://www.xda-developers.com/wireguardnt-native-wireguard-port-windows-kernel/>

如果你经常使用 VPN(虚拟专用网)，你会很高兴听到一个叫做 WireGuardNT 的新项目。对于那些不熟悉的人来说，WireGuard 是一种相对较新的 VPN 隧道协议，它采用了现代加密标准，具有安全的代码库，并且具有很好的性能。它被集成到版本为 5.6 的 Linux 内核中，但是到目前为止，在 Windows 上只有一个用户空间实现。这就是 WireGuardNT 的用武之地:它是 WireGuard 对 Windows 内核的一个本地移植，它承诺让事情变得更快。

Windows 上的 WireGuard 目前使用一个共享的 Go 代码库，带有一个名为 [Wintun](https://www.wintun.net) 的 TUN 驱动程序。它在用户空间工作，正如[公告](https://lists.zx2c4.com/pipermail/wireguard/2021-August/006887.html)所说，它“在 Wintun 接口之间传递数据包”。使用 WireGuardNT，整个协议被直接实现到 Windows 的网络堆栈中，就像在 Linux 上一样。

虽然 WireGuard 在 Windows 上的性能已经很好了，但计划是让它在 WireGuardNT 上变得更好。虽然这个项目仍处于早期阶段，但即使在进行额外的调整和优化之前，它仍然因为是内核原生的而更快。这在一定程度上可以归因于旧的 wireguard-go/Wintun 实现减少了所有上下文切换的开销和延迟。

但是新的 WireGuardNT 实现比旧的用户空间版本快多少呢？通过有线连接，开发人员看到速度高达 7.5Gbps 开发者也注意到了 Wi-Fi 的显著性能提升。例如，一名使用英特尔 AC9560 WiFi 卡的测试人员在没有 WireGuard 的情况下获得了约 600Mbps 的速度，在旧用户空间版本的 WiFi 上获得了约 95Mbps 的速度，在 WireGuardNT 实施的 WiFi 上获得了约 600Mbps 的速度。基本上，由于新的本机内核端口，旧用户空间版本对无线性能的影响已经消除，有线性能也得到了显著升级。

如上所述，该项目仍处于早期阶段。为了做好发布准备，WireGuard for Windows client 版的项目分为三个阶段。第一阶段，我们现在所处的阶段，看到 WireGuardNT 隐藏在“ExperimentalKernelDriver”注册表旋钮后面，所以如果你不打开它，它就不会被启用。第二阶段将看到默认启用的本机内核实现。第三阶段，也是最后一个阶段，将从 Windows 客户端移除旧的 wireguard-go/Wintun 用户空间实现，但仍将保留它以支持其他应用程序和用途。

就像这样的实验性发布一样，开发者 Jason Donenfeld 希望人们可以尝试它来找到错误并留下反馈。WireGuardNT 是 Windows now 的 WireGuard 客户端的一部分，其版本为 0.4。你可以[在这里](https://www.wireguard.com/install/)下载，或者你可以在这里阅读更多关于项目[的信息。](https://git.zx2c4.com/wireguard-nt/about/)

*本文的早期版本指出，只有通过无线连接，网络性能才会有显著提高。*