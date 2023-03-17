# 新的 Windows 11 版本带来了新的微软 365 小工具

> 原文：<https://www.xda-developers.com/new-windows-11-build-22000-168-microsoft-365-widget/>

微软为 Windows 内部人士发布了 Windows 11 的罕见周五版本。随着我们继续接近正式公开发布，今天的更新再次是一个相对较小的更新。在新闻方面，Windows 11 build 22000.168 包括一个新的微软 365 小工具，但只针对 Azure 广告帐户

这个新的小部件汇集了您所在组织中与您相关的快速信息。这包括您经常访问的文件夹、SharePoint 上的最新更新和会议录音，以及更多内容。

除此之外，另一个值得注意的变化是，由微软团队支持的聊天功能现在已经本地化为多种语言，而不仅仅是英语。该应用程序将遵循您的操作系统范围的语言设置，并支持以下语言:

### Windows 11 聊天中支持的语言

阿尔巴尼亚语、阿拉伯语、阿塞拜疆语、巴斯克语、保加利亚语、加泰罗尼亚语、中文(简体)、中文(繁体)、克罗地亚语、捷克语、丹麦语、荷兰语、英语(英国)、英语(美国)、爱沙尼亚语、菲律宾语、芬兰语、法语、法语(加拿大)、加利西亚语、格鲁吉亚语、德语、希腊语、希伯来语、印地语、匈牙利语、冰岛语、印度尼西亚语、意大利语、日语、哈萨克语、韩语、拉脱维亚语、立陶宛语、马其顿语、挪威语(博克马尔语)、挪威语(尼诺斯克语)、波兰语、葡萄牙语(巴西)、葡萄牙语(葡萄牙语)、罗马尼亚语、俄语、塞尔维亚语、拉丁语、斯洛伐克语、斯洛文尼亚语、西班牙语(西班牙语)

虽然这不是此次构建的一部分，但微软也强调了对微软商店应用程序的一些更新。库部分已经过重新设计，性能有所提高。它现在还可以对你的库进行排序，让你看到哪些应用程序是最近更新的，这是 Windows 10 中提供的功能，但在 Windows 11 中暂时丢失了。你还会发现微软商店的聚光灯区有一个调整过的设计，你可以将鼠标放在每个项目上预览它的内容。

在这一点上，当 Windows 11 发布时， [Android 应用支持](https://www.xda-developers.com/windows-11-android-apps/)将对普通公众可用的可能性越来越小。该功能仍然是无处可寻，无论是在开发或测试渠道。

Windows 11 build 22000.168 中唯一的其他消息是错误修复，具体如下:

### Windows 11 内部版本 22000.168 中的修复

*   搜索:
    *   我们已经解决了一个潜在的问题，在过去几个航班的笔功能设备，导致搜索进入一个状态，这是不可能从结果中启动应用程序。
*   设置:
    *   我们修正了在设置中的搜索框中输入某些短语有时会导致设置崩溃的问题。
*   小部件:
    *   当使用 Family widget 时，您应该不会再意外地看到消息说“连接设备以查看屏幕时间活动”，尽管有可用的活动显示。
*   来自 Microsoft 团队的聊天:
    *   我们修复了视频通话期间视频有时会冻结或显示黑色图像的问题。
    *   我们还修复了一个问题，即如果您在呼叫之间切换，前一个呼叫不会自动保留，因此音频和视频流会继续两个呼叫。

在这个版本中也有大量的已知问题，这个列表仍然比错误修复要大得多。希望这些问题能在接下来的几周内得到解决，但现在，你需要注意以下几点:

### Windows 11 内部版本 22000.168 中的已知问题

*   **【提醒】**从 Windows 10 升级到 Windows 11 或者安装 Windows 11 的更新时，某些功能可能会被弃用或删除。[详见此处](https://www.microsoft.com/en-us/windows/windows-11-specifications#primaryR4)。
*   我们正在调查一个问题，在一些设备上，当进入[设置> Windows 更新> Windows Insider 程序](https://aka.ms/WIPSettings)时，只有“停止获取预览版本”选项可见。这防止了内部人员选择通道。我们[已经发布了答案](https://aka.ms/WIPSettingsFix)的变通办法。
*   **【BETA CHANNEL】**我们正在调查 BETA CHANNEL 内部人士的报告，他们在升级到 Windows 11 后，看不到新的任务栏，开始菜单也不起作用。如果您受到影响，请尝试转到 Windows Update >更新历史，卸载最新的 Windows 累积更新，然后通过检查更新重新安装。
*   我们正在修复一个问题，该问题导致一些 Surface Pro X 设备通过 WHEA _ 不可纠正 _ 错误进行错误检查。
*   开始:
    *   在某些情况下，使用“从开始”或任务栏搜索时，您可能无法输入文本。如果遇到此问题，请按键盘上的 WIN + R 启动“运行”对话框，然后关闭它。
    *   右键单击开始按钮(WIN + X)时，系统和 Windows 终端丢失。
*   任务栏:
    *   切换输入法时任务栏有时会闪烁。
*   搜索:
    *   单击任务栏上的搜索图标后，搜索面板可能不会打开。如果出现这种情况，请重新启动“Windows 资源管理器”进程，并再次打开搜索面板。
    *   搜索面板可能显示为黑色，并且不显示搜索框下方的任何内容。
*   蓝牙:
    *   我们正在调查来自内部人士的报告，这些内部人士使用配对的蓝牙 LE 设备，在从休眠状态恢复或蓝牙关闭后，蓝牙可靠性问题和错误检查增加。
*   小部件:
    *   小部件面板可能显示为空。要解决此问题，您可以注销，然后重新登录。
    *   外接显示器上的小工具可能会以错误的尺寸显示。如果您遇到这种情况，您可以首先在实际的 PC 显示器上通过触摸或 WIN + W 快捷方式启动小工具，然后在辅助显示器上启动。
*   商店:
    *   我们正在努力提高商店中的搜索相关性，包括解决在某些情况下搜索结果排序不准确的问题。
    *   在某些有限的情况下,“安装”按钮可能还不起作用。
    *   某些应用程序不提供评级和评论。
*   Windows 沙盒
    *   在 Windows 沙盒中，单击任务栏上的切换器图标后，语言输入切换器不会启动。作为一种解决方法，用户可以通过以下任何硬件键盘快捷键来切换他们的输入语言:Alt + Shift、Ctrl + Shift 或 Win + Space(第三个选项仅在沙盒全屏时可用)。
    *   在 Windows 沙盒中，单击任务栏中的 IME 图标后，IME 上下文菜单不会启动。作为解决方法，用户可以使用以下方法之一访问 IME 快捷菜单的功能:
        *   通过设置>时间和语言>语言和地区>(如日语)三点>语言选项>(如微软 ime)三点>键盘选项访问 IME 设置。
            *   或者，您也可以启用 IME 工具栏，这是一个快速调用特定 IME 功能的替代用户界面。从上面继续，导航到键盘选项>外观>使用 IME 工具栏。
        *   使用与每种 IME 支持的语言相关联的一组独特的硬件键盘快捷键。(参见:[日文 IME 快捷键](https://support.microsoft.com/windows/microsoft-japanese-ime-da40471d-6b91-4042-ae8b-713a96476916)，[繁体中文 IME 快捷键](https://support.microsoft.com/windows/microsoft-traditional-chinese-ime-ef596ca5-aff7-4272-b34b-0ac7c2631a38))。
    *   本地化
        *   有一个问题，一些内部人员可能会从他们的用户体验中丢失一些运行最新内部人员预览版本的语言子集的翻译。为了确认您是否受到了影响，[请访问此回答论坛帖子](https://aka.ms/UnderLocIssue)，并按照步骤进行补救。
    *   来自微软团队的聊天
        *   阿拉伯语和希伯来语目前不允许改变团队设置。若要更改团队设置，请注销并切换到另一种语言。
        *   当您拨出电话时，如果听不到铃声，用户界面会显示电话正在接通。

如果您是 Windows Insider 计划的成员，您最近可能会收到一封电子邮件，警告您从开发频道切换到测试频道。那是因为 Dev 频道内部人士即将开始测试明年的 Windows 11 更新，会不稳定很多。如果你想保持一个稳定的版本，一定要检查你的 Windows Insider 设置。