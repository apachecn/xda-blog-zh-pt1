# Windows 11 内部版本 22000.832 支持安装期间的版本升级

> 原文：<https://www.xda-developers.com/windows-11-cumulative-update-22000-829/>

微软为 Windows 11 用户发布了一个新的可选累积更新，使该操作系统的内部版本号为 22000.832。这是从上周[在发布预览频道](https://www.xda-developers.com/windows-11-22000-829-major-updates-setup/)向 Windows 内部人士推出的版本的一个小增量，但这个版本对任何想安装它的人都是可用的。更新标签为 [KB5015882](https://support.microsoft.com/en-us/topic/july-21-2022-kb5015882-os-build-22000-829-preview-473e1d95-06a0-4f40-9554-cdc7cca85584) ，你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5015882)手动下载。

此次更新的亮点在于，它允许 Windows 11 在开箱即用体验(OOBE)期间安装 Windows 的主要版本更新。基本上，当您第一次使用用户帐户设置电脑时，如果版本升级可用并且您的设备符合条件，系统会提示您安装版本升级。考虑到我们预计 Windows 11 版本 22H2 将在未来几个月的某个时间推出，这一变化来得正是时候。通过这种方式，购买装有 Windows 11 原始版本的新 PC 的人将能够升级并获得开箱即用的最新功能。

然而，这还不是全部的新内容。还有一个新选项，允许 Windows 11 在对焦辅助开启时显示紧急通知。以下是本次更新中的亮点:

Windows 11 build 22000.832 中的完整更改列表要长得多，正如你所料，它主要是关于修复和微小的改进。各种问题已经解决，您可以在下面找到完整的列表。

### WIndows 11 build 22000.832 中的改进

*   ***新增！*** 使您能够在焦点辅助开启时同意接收紧急通知。
*   ***新增！*** 为符合条件的设备在首次登录时的开箱即用体验(OOBE)期间提供更新至较新的 Windows 11 版本的选项。如果您选择更新到较新的版本，更新过程将在设备上安装更新后不久开始。
*   ***新增！*** 为受硬件重用安全缓解影响的 Windows 自动驾驶部署场景恢复功能。此更新取消了自部署模式(SDM)和预配置模式(PP)的一次性使用限制。此更新还为批准的制造商在用户驱动模式(UDM)部署中重新启用任何用户主体名称(UPN)显示。
*   解决了 **UIAutomation()** 中导致应用程序停止工作的问题。
*   解决了阻止某些应用程序的启动任务 API 按预期工作的问题。

*   提高了操作系统升级后按钮复位的可靠性。
*   解决了删除 EN-US 语言包时导致租户限制事件日志记录通道不可访问的问题。
*   解决了在域控制器上安装 2022 年 5 月 10 日安全更新后，在某些情况下导致基于证书的计算机帐户身份验证失败的问题。
*   解决了影响您使用 Windows 11 软件开发工具包(SDK)构建的 Arm64EC 代码的问题。
*   更新 **Remove-Item** cmdlet 以正确地与 Microsoft OneDrive 文件夹交互。
*   解决了阻止某些故障排除工具打开的问题。
*   解决了导致容器端口映射冲突的问题。
*   解决了导致代码完整性在文件被修改后继续信任文件的问题。
*   解决了在打开智能安全图功能的情况下启用 Windows Defender 应用程序控制时可能导致 Windows 停止工作的问题。
*   将搜索亮点部署到设备。要访问搜索重点的策略(在安装了 2022 年 6 月累积更新预览版或 2022 年 7 月每月质量更新的设备上)，请转到**C:\ Windows \ policy definitions**并找到 **Search.admx** 。为了您的方便，我们将发布管理模板的更新版本。 **admx** ) for Windows 11，版本 21H2 即将到微软下载中心。
*   解决了在某些设备上使用播放和暂停键盘按钮时导致**explorer.exe**停止工作的问题。
*   解决了当您使用“开始”菜单的上下文菜单(Win+X)并且外部显示器连接到您的设备时，**explorer.exe**停止工作的问题。
*   解决了当鼠标悬停在任务栏上的搜索图标上时显示无法关闭的空白窗口的问题。
*   在许多线程争用一个文件的高每秒输入/输出操作(IOPS)情况下，减少资源争用的开销。
*   解决了导致 Windows 配置文件服务偶尔失败的问题。登录时可能会出现故障。错误消息是，“gpsvc 服务登录失败。拒绝访问”。

如果您想获得这些修补程序，只需在 Windows Update 中查找更新，然后选择安装 KB5015882 累积更新。否则，您可以使用我们在顶部提供的链接手动下载。

虽然这是一个可选的更新，但所有这些变化都将在下个月向每个人公布，届时微软将为 Patch Tuesday 推出新的累积更新。这些是强制性的更新，它们通常包括额外的修复。不过最近，微软主要发布了补丁星期二更新，没有太多的变更日志，所以大部分变化都在这次更新中。

**【更新 7 月 25 日@美国东部时间 5:38AM】**该更新最初被标记为内部版本号 22000.829，但这是不正确的。正确的内部版本号是 22000.832。我们相应地更新了文章。