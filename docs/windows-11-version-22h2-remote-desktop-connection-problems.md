# Windows 11 版本 22H2 导致远程桌面出现问题

> 原文：<https://www.xda-developers.com/windows-11-version-22h2-remote-desktop-connection-problems/>

9 月 20 日，Windows 11 开始接收其第一次重大更新——[Windows 11 version 22 H2](https://www.xda-developers.com/windows-11-22h2/)，或 2022 更新，其中有很多好的补充。然而，正如许多 Windows 更新的情况一样，也有一些问题。微软已经承认了一些打印机的问题，现在，一些用户遇到了远程桌面连接的问题。

这些问题最初是在微软社区论坛上报告的，随后许多用户确认他们也遇到了这个问题。根据最初的报告，Windows 11 版本 22H2 中的远程桌面客户端存在一个 bug，它只尝试通过 UDP 建立连接，完全忽略 TCP 连接。因此，许多连接会失败，因为一些组织被设置为仅使用 TCP。

虽然微软尚未将该问题添加到 Windows 11 发布健康信息页面，但该公司确实对论坛帖子做出了回应，最终表示正在调查该问题。幸运的是，如果您遇到了这个问题，有一个解决方法。您需要使用注册表编辑器导航到**Computer \ HKEY _ LOCAL _ MACHINE \ SOFTWARE \ Policies \ Microsoft \ Windows NT \ Terminal Services \ Client**，然后在该文件夹中创建一个名为 **fClientDisableUDP** 的新 DWORD 值，并将该值设置为 1。这应该允许远程桌面 TCP 连接再次工作，直到微软解决这个问题。

这也不是最近在 Windows 11 版本 22H2 中发现的唯一问题。微软在 Windows 11 发布信息页面中添加了一个单独的问题,声明配置包可能无法在 Windows 11 版本 22H2 中正常工作。如果您设置安装了此更新的电脑，设置包可能不会在安装过程中完全安装，从而导致某些选项配置不正确。也有可能导致安装过程意外重启或无法完成。

解决这个问题的一个简单方法是在安装更新之前提供设备。如果初始设置已经完成，升级到 Windows 11 版本 22H2 不会导致任何问题。此外，使用 Windows 自动修补进行设置不受此问题的影响。微软表示，它正在努力修复更新，但尚未提供时间表。

* * *

**来源:** [微软社区](https://answers.microsoft.com/en-us/windows/forum/all/issues-with-remote-desktop-on-windows-11-after/2f0b90c8-9549-46bb-bede-41c2d3990380)

**Via:**[bleeding computer](https://www.bleepingcomputer.com/news/microsoft/microsoft-investigates-windows-11-22h2-remote-desktop-issues/)