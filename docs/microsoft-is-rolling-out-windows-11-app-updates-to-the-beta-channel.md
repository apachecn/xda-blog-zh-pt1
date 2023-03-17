# 微软正在向测试频道推出 Windows 11 应用更新

> 原文：<https://www.xda-developers.com/microsoft-is-rolling-out-windows-11-app-updates-to-the-beta-channel/>

今天，微软向测试频道发布了 Windows 11 版本 22000.194。首先，没什么新鲜的。Windows 11 将于 10 月 5 日推出；可以肯定地说，它的功能是完整的。然而，你会发现一件事，那就是大量的 Windows 11 应用程序更新。

这些工具包括剪辑工具、计算器和带焦点的时钟会话。所有这些都已经在 Dev 频道上发布了一段时间了。但如果你在测试频道，你会开始看到他们出现。

可能其中最引人注目的是[带焦点会话的时钟](https://www.xda-developers.com/windows-11-clock-focus-sessions/)。整个想法是，你可以设置时间来聚焦，将它链接到你的 Spotify，它甚至可以与微软集成来做。新的[截取工具](https://www.xda-developers.com/windows-11-snipping-tool/)实际上更像是 UX 的一次革新，与其说是提供了一堆新功能，不如说是超越了它的前辈。

当然，Windows 11 build 22000.194 也有一大堆修复和已知问题。以下是修复的内容:

### Windows 11 构建 22000.194 修复程序

*   解决了一个问题，如果你启用然后禁用一个对比主题，它会导致在标题栏的文物，在某些情况下，使最小化/最大化/关闭按钮难以看到和使用。
*   修复了某些连接的设备可能导致无法使用蓝牙的崩溃。
*   缓解了某些应用程序中字幕无法正常显示的问题，尤其是日语字幕。
*   修正了导致某些电脑在现代待机状态下出现错误检查的问题。
*   缓解了使用某些第三方 ime 在设置中的搜索框中键入时可能导致候选窗口呈现在屏幕上的其他位置(未附加到搜索框)和/或插入到搜索框中的字符不显示的问题。
*   我们修复了导致 PowerShell 创建无限多个子目录的问题。当您使用 PowerShell **Move-Item** 命令将目录移动到其子目录之一时，会出现此问题。结果，卷被填满，系统停止响应。
*   该版本包括一项更改，即在虚拟机(VM)上强制执行 Windows 11 系统要求，使其与物理 PC 相同。之前创建的运行 Insider 预览版的虚拟机可能不会更新到最新的预览版。在 Hyper-V 中，虚拟机需要创建为第二代虚拟机。关于 Windows 11 系统需求的更多细节——[点击这里](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fblogs.windows.com%2Fwindows-insider%2F2021%2F08%2F27%2Fupdate-on-windows-11-minimum-system-requirements-and-the-pc-health-check-app%2F&data=04%7C01%7Cbleblanc%40microsoft.com%7Cb630fd734c404096c1dd08d978a7337b%7C72f988bf86f141af91ab2d7cd011db47%7C0%7C0%7C637673481840356309%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&sdata=oFiOE87fVrMvYEc%2F9j12K6uURmR2wysH2k5bdvsFwbg%3D&reserved=0)看这篇博文。

以下是仍然存在的问题:

### Windows 11 内部版本 22000.194 已知问题

**【常规】**

*   我们正在调查 Beta 频道内部人士的报告，他们在升级到 Windows 11 后，看不到新的任务栏，开始菜单也不起作用。如果您受到影响，要解决此问题，请尝试转到 Windows Update >更新历史记录，卸载最新的 Windows 累积更新，然后通过检查更新来重新安装。
*   我们正在修复一个问题，该问题导致一些 Surface Pro X 出现 WHEA _ 不可纠正 _ 错误的错误检查。

**【开始】**

*   在某些情况下，使用“从开始”或任务栏搜索时，您可能无法输入文本。如果遇到此问题，请按键盘上的 WIN + R 启动“运行”对话框，然后关闭它。
*   右键单击开始按钮(WIN + X)时，系统和 Windows 终端丢失。

**【任务栏】**

*   切换输入法时任务栏有时会闪烁。

**【搜索】**

*   单击任务栏上的搜索图标后，搜索面板可能不会打开。如果出现这种情况，请重新启动“Windows 资源管理器”进程，并再次打开搜索面板。
*   搜索面板可能显示为黑色，并且不显示搜索框下方的任何内容。

**【微件】**

*   小部件面板可能显示为空。要解决此问题，您可以注销，然后重新登录。
*   外接显示器上的小工具可能会以错误的尺寸显示。如果您遇到这种情况，您可以首先在实际的 PC 显示器上通过触摸或 WIN + W 快捷方式启动小工具，然后在辅助显示器上启动。

**【微软商店】**

*   我们将继续努力提高商店中的搜索相关性。

**【Windows 沙盒】**

*   在 Windows 沙盒中，单击任务栏上的切换器图标后，语言输入切换器不会启动。作为一种解决方法，用户可以通过以下任何硬件键盘快捷键来切换他们的输入语言:Alt + Shift、Ctrl + Shift 或 Win + Space(第三个选项仅在沙盒全屏时可用)。
*   在 Windows 沙盒中，单击任务栏中的 IME 图标后，IME 上下文菜单不会启动。作为解决方法，用户可以使用以下方法之一访问 IME 快捷菜单的功能:
    *   通过设置>时间和语言>语言和地区>(如日语)三点>语言选项>(如微软 ime)三点>键盘选项访问 IME 设置。
        *   或者，您也可以启用 IME 工具栏，一个替代的用户界面，以快速调用特定的 IME 功能。从上面继续，导航到键盘选项>外观>使用 IME 工具栏。
    *   使用与每种 IME 支持的语言相关联的一组独特的硬件键盘快捷键。(参见:[日文 IME 快捷键](https://support.microsoft.com/windows/microsoft-japanese-ime-da40471d-6b91-4042-ae8b-713a96476916)，[繁体中文 IME 快捷键](https://support.microsoft.com/windows/microsoft-traditional-chinese-ime-ef596ca5-aff7-4272-b34b-0ac7c2631a38))。

微软还增加了对虚拟机上 TPM 的要求，这是我们今天早些时候报道的内容。事实上，虚拟机现在具有与裸机硬件相同的要求。

与往常一样，只要您使用测试版，就可以通过 Windows Update 获得最新版本。如果您不是，可以转到“设置”中的“Windows Insider 程序”选项卡开始。