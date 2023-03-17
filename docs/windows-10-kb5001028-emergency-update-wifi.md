# Windows 10 新更新修复了 WPA3 Wi-Fi 崩溃问题

> 原文：<https://www.xda-developers.com/windows-10-kb5001028-emergency-update-wifi/>

# Windows 10 紧急更新修复了导致 BSOD 崩溃的 Wi-Fi 漏洞

建议 Windows 10 用户应用此补丁，以防他们在使用 WPA3 安全连接 Wi-Fi 时遇到问题。

微软正在为 Windows 10 推出新的紧急更新，以修复连接 Wi-Fi 网络时导致 BSOD(蓝屏死亡)的错误。该问题仅与较新的 WPA3 安全性有关，这基本上意味着只有少数用户受到影响。据称，该漏洞是上个月发布的版本号为 KB4598298 和几天前发布的 KB4601315 的 Windows 10 1909 累积更新的一部分。

到目前为止，[微软正在推出](https://twitter.com/WindowsUpdate/status/1359925636723183617)版本为 KB5001028 的带外补丁来解决这个问题。值得注意的是，Windows 10 1909 附带了内部版本 18363。KB5001028 修补程序将内部版本从 18363.1377 提升到 18363.1379。"*当您尝试使用保护无线电脑网络安全系统 3 (WPA3)连接时，您可能会在 **nwifi.sys** 中收到蓝屏 stop 错误 0x7E。断开连接后重新连接到 Wi-Fi 网络时，或者从睡眠或休眠状态中醒来时，您很可能会遇到此问题。**注意:**目前大部分 Wi-Fi 网络都在使用 WPA2，不受影响*，[微软](https://docs.microsoft.com/en-us/windows/release-health/resolved-issues-windows-10-1909#1557msgdesc)表示。

KB5001028 带外更新可通过 Windows Update 获得，或者您可以从 [Microsoft Update 目录](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5001028)中手动下载。您也可以使用以下链接下载修补程序:

此外，Microsoft 还建议尝试以下替代步骤，尽管它们可能不适用于所有用户:

*   将您的设备更新到 Windows 10、2004 版或 20H2 版。
*   使用 WPA2 连接到 Wi-Fi 网络。为此，您可能需要重新配置接入点或路由器设置。
*   使用有线以太网连接。

Windows 10 最近获得了一个新的可选更新，其中包括一个影响少数游戏玩家的重要修复，这些玩家在全屏或平板模式下玩游戏时面临系统崩溃问题。针对 2020 年 5 月更新和 2020 年 10 月更新的 KB4598291 补丁还包括一个针对受 bugbear 影响的用户的重要修复，这些用户在重新启动系统后会被注销应用和网站。