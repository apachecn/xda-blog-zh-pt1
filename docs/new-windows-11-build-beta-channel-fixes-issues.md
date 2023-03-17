# 新的 Windows 11 测试版修复了更多问题

> 原文：<https://www.xda-developers.com/new-windows-11-build-beta-channel-fixes-issues/>

我们已经期待了几个星期了，但是今天，微软终于把开发频道的 Windows 内部人员和测试频道的内部人员分开了。Dev 频道现在正在测试明年 Windows 11 的更新，版本号为[22449](https://www.xda-developers.com/microsoft-moves-windows-11-dev-channel-prerelease-builds/)，但 Beta 频道也将获得新的更新，这是即将于[10 月 5 日](https://www.xda-developers.com/windows-11-release-date-october-5/)发布的一部分。Windows 11 build 22000.176 现在[在测试频道](https://blogs.windows.com/windows-insider/2021/09/02/announcing-windows-11-insider-preview-build-22000-176/)向 Windows Insiders 发布，它只包括一些错误修复。

这个版本最大的新闻是它现在可以在发布预览频道中为[商业用户提供。如果您的计算机属于某个组织，并且您注册了此渠道，您将可以选择升级到 Windows 11，或者改为测试 Windows 10 版本 21H2。你不必马上升级到 Windows 11。](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/commercial-previews-for-windows-11-and-windows-10-version-21h2/ba-p/2676467)

如上所述，这个版本没有什么新东西。微软表示，你可以通过右键单击任务栏来显示或隐藏任务栏图标，如聊天、搜索或小工具，但这并不新鲜。有可能微软只是想引起人们对这个功能的关注。

然而，这个版本确实包括一些已知问题的修复，包括与微软团队(预览版)通话不会产生铃声。您可以在下面看到完整的修复列表:

### Windows 11 内部版本 22000.176 中的错误修复

**【常规】**

*   我们修复了配对蓝牙 LE 设备的一个问题，该问题导致从休眠状态恢复后或蓝牙关闭时蓝牙可靠性问题和错误检查增加。
*   我们缓解了一个问题，该问题导致一些用户在试图用某些 USB 相机拍照时遇到意外错误。
*   在 OOBE 设置 Windows Hello 时，我们添加了一个新链接来了解有关 Windows Hello 的更多信息。

**【来自微软团队的聊天】**

*   阿拉伯语和希伯来语将允许改变队伍设置。
*   我们修复了这样一个问题:如果你正在拨打电话，没有铃声，但用户界面会显示电话正在连接。

**【微软商店】**

在最近的商店更新中修复了以下问题:

*   我们修复了安装按钮在有限情况下可能不起作用的问题。
*   我们还修复了一些应用程序无法获得评级和评论的问题。

与此同时，已知问题的列表仍然很长，并且开始看起来其中一些问题可能会溜到 10 月 5 日的最终版本中。以下是您仍然需要注意的:

### Windows 11 内部版本 22000.176 中的已知问题

**【常规】**

*   我们正在调查 Beta 频道内部人士的报告，他们在升级到 Windows 11 后，看不到新的任务栏，开始菜单也不起作用。如果您受到影响，要解决此问题，请尝试转到 Windows Update >更新历史记录，卸载最新的 Windows 累积更新，然后通过检查更新来重新安装。
*   我们正在修复一个问题，该问题导致一些 Surface Pro X 设备通过 WHEA _ 不可纠正 _ 错误进行错误检查。

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
    *   通过设置>时间和语言>语言和地区><each ime="" language="">(例如日语)三点>语言选项><each ime="">(例如微软 ime)三点>键盘选项访问 IME 设置。</each></each>
        *   或者，您也可以启用 IME 工具栏，这是一个快速调用特定 IME 功能的替代用户界面。从上面继续，导航到键盘选项>外观>使用 IME 工具栏。
    *   使用与每种 IME 支持的语言相关联的一组独特的硬件键盘快捷键。(参见:[日文 IME 快捷键](https://support.microsoft.com/windows/microsoft-japanese-ime-da40471d-6b91-4042-ae8b-713a96476916)，[繁体中文 IME 快捷键](https://support.microsoft.com/windows/microsoft-traditional-chinese-ime-ef596ca5-aff7-4272-b34b-0ac7c2631a38))。

**【本地化】**

*   有一个问题，一些内部人员可能会从他们的用户体验中丢失一些运行最新内部人员预览版本的语言子集的翻译。为了确认您是否受到了影响，[请访问此回答论坛帖子](https://aka.ms/UnderLocIssue)，并按照步骤进行补救。

我们还没有看到微软为 Windows 11 宣布的一些功能。我们现在知道[的 Android 应用程序不会在](https://www.xda-developers.com/android-windows-11-delayed/)发布时可用，但是几周前由 Panos Panay 开发的[新绘画应用程序](https://www.xda-developers.com/microsoft-shows-off-new-paint-windows-11/)现在也无处可寻。我们还有几个星期的时间，所以希望这将很快与这些已知问题的修复程序一起添加进来。