# 微软向 Dev 频道发布了 Windows 11 build 22458，并附有修复程序

> 原文：<https://www.xda-developers.com/microsoft-releases-windows-11-build-22458-to-the-dev-channel-with-fixes/>

今天是周三，这意味着是时候在开发频道发布新的 [Windows 11](https://www.xda-developers.com/windows-11/) 内部预览版了。本周的构建是 22458，和往常一样，没有太多新的东西。事实上，开发频道中出现的大多数新功能都将在 10 月 5 日新操作系统发布后出现。

该操作系统的一个物理变化是，当你点击开始中的电源菜单时，有一个新的选项“登录选项”。当然，这增加了睡眠、关机和重启。

除此之外，这都是关于修复。在 Windows 11 内部版本 22458 中，有一长串的问题得到了修复。

### Windows 11 内部版本 22458 修复程序

**【开始】**

*   修复了一个影响启动可靠性的潜在问题。

**【搜索】**

*   文件夹名称中带有#的文件夹现在可以添加到索引中。

**【设置】**

*   解决了当试图打开显示页面时有时会导致设置崩溃的问题。
*   点击“高级显示设置”中的“关于刷新率的更多信息”,将会打开支持页面。
*   修正了一个问题，即设置中的位置页面不显示警告文本，解释为什么定位服务设置是灰色的，如果它是灰色的。
*   现在应该会保留在“设置”中的“管理应用程序执行别名”下对首选项所做的更改。
*   修正了 [dll](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/ee624057(v=ws.11)) ( [第 206 期](https://github.com/MicrosoftDocs/Console-Docs/issues/206))输出中的几个错别字。

**【开窗】**

*   缓解了在启用自动 HDR 的情况下使用 ALT + Enter(即在全屏和窗口模式之间切换)时可能会导致某些游戏意外崩溃的问题。

**【其他】**

*   解决了在某些情况下导致加密文件系统窗口中的文本截断的问题。
*   修复了一个罕见的情况，可能导致卸载的收件箱应用程序在重新启动后意外重新出现。
*   Appx commandlets 现在应该可以与 PowerShell 7.0+一起工作了([问题#13138](https://github.com/PowerShell/PowerShell/issues/13138) )。

当然，作为一个开发频道构建，也有一长串的已知问题。

### Windows 11 内部版本 22458 已知问题

**【常规】**

*   我们正在修复一个问题，该问题导致一些 Surface Pro X 通过 WHEA _ 不可纠正 _ 错误进行错误检查。
*   我们正在修复一个问题，该问题导致一些设备在尝试更新到最新版本时出现 DRIVER_PNP_WATCHDOG 错误。

**【开始】**

*   在某些情况下，使用“从开始”或任务栏搜索时，您可能无法输入文本。如果遇到此问题，请按键盘上的 WIN + R 启动“运行”对话框，然后关闭它。
*   右键单击开始按钮(WIN + X)时系统丢失。

**【任务栏】**

*   **重要提示:当默认居中对齐时，任务栏上的图标会移到一边，导致当打开太多应用程序时，它们会被“显示隐藏图标”按钮切断。**
*   切换输入法时任务栏有时会闪烁。

**【搜索】**

*   单击任务栏上的搜索图标后，搜索面板可能不会打开。如果出现这种情况，请重新启动“Windows 资源管理器”进程，并再次打开搜索面板。
*   搜索面板可能显示为黑色，并且不显示搜索框下方的任何内容。

**【文件浏览器】**

*   如果您在文件资源管理器中右键单击 OneDrive 位置中的文件，当您将鼠标悬停在打开子菜单的条目上时，上下文菜单将意外关闭，例如“打开方式”

**【微件】**

*   小部件面板可能显示为空。要解决此问题，您可以注销，然后重新登录。
*   外接显示器上的小工具可能会以错误的尺寸显示。如果您遇到这种情况，您可以首先在实际的 PC 显示器上通过触摸或 WIN + W 快捷方式启动小工具，然后在辅助显示器上启动。

**【Windows 沙盒】**

*   我们正在调查一个问题，在升级到此版本后，Windows Sandbox 可能无法为某些内部人员启动。

**【微软商店】**

*   我们将继续努力提高商店中的搜索相关性。

**【Windows Linux 子系统(WSL)&Hyper-V】**

*   我们正在调查 WSL2 和 Hyper-V 在 ARM64 电脑(如 Surface Pro X)上无法运行的报告。

微软也谈到了一个新的提示应用程序，其中有 114 个新的提示。它还包括丙烯酸透明材料，以及你期待 Windows 11 更新的其他 UX 元素，如圆角。还有一个新的提示小部件，你可以在小部件面板中找到，微软表示，该应用程序将在整个操作系统中支持弹出窗口。

与往常一样，如果您在开发人员频道上，您可以从 Windows Update 获取今天的版本，如果您不在，您可以通过“设置”中的“Windows Insider 计划”选项卡注册。在[微软的博客文章](https://blogs.windows.com/windows-insider/2021/09/15/announcing-windows-11-insider-preview-build-22458/)中，它确实澄清了一些内务问题，例如开发频道不能在不进行工厂重置的情况下回滚到测试频道，预发布版本在桌面上带有水印，等等。