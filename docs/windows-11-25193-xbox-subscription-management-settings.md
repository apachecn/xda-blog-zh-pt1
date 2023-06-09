# Windows 11 build 25193 在设置中获得 Xbox 订阅管理

> 原文：<https://www.xda-developers.com/windows-11-25193-xbox-subscription-management-settings/>

虽然比往常晚了一点，但微软今天在 Dev 频道向内部人士推出了新版本的 [Windows 11](https://www.xda-developers.com/windows-11/) ，使版本号达到 25193。在这个版本中没有太多新的东西，但是亮点是在设置应用中增加了 Xbox 订阅管理功能。

这是微软自最初的 Windows 11 发布以来一直在扩展的东西。我们已经看到该公司增加了对微软 365 订阅和独立 OneDrive 计划的支持，现在，Xbox 也在这里。这意味着如果你进入**设置- >账户**，你将能够看到你当前与 Xbox 相关的订阅信息，无论是 Xbox Game Pass for console、PC Game Pass、Xbox Game Pass Ultimate 还是 Xbox Live Gold。与 Microsoft 365 一样，您可以查看您使用的付款方式、您的账单金额，以及您的计划中包含哪些福利。您还可以管理重复计费，兑换套餐代码或预付卡。

除此之外，微软还提到了对盲文显示器的支持以及新的盲文输入和输出语言。一些新支持的显示器包括 APH 变色龙，APH 螳螂 Q40 和 NLS 阅读器。为了利用这一改进的支持，你需要在设置应用程序中卸载当前的盲文支持，然后重新安装，但这对任何使用这些设备的人来说都是好消息。

不过，这个版本实际上删除了一个功能，那就是使用内置的 Windows 共享窗口通过 OneDrive 直接共享本地文件的能力。这是在 build 25163 中添加的，但微软表示，由于 Windows 内部人士的反馈，它将删除它，并希望在改进后恢复该功能。

除此之外，像往常一样，在这个版本中有一个很长的修复列表，解决了部分体验中的广泛问题。你可以在下面找到这些。

### Windows 11 内部版本 25193 中的修复

**【常规】**

*   修复了导致启用的问题。NET Framework 3.5 在以前的版本中不起作用。

**【任务栏】**

*   进行了修复，现在任务栏溢出将使用与任务栏相同的强调颜色。
*   修正了几个导致与任务栏溢出相关的零星 explorer.exe 崩溃的问题。
*   修正了一个与任务栏中的窗口小部件条目相关的问题，这个问题导致任务栏图标在之前的飞行中有时会出现漂移。
*   修复了至少有两台显示器的内部人员的问题，如果显示器具有不同的 DPI，任务栏溢出可能会在需要之前出现，或者最终与辅助显示器上的日期和时间重叠。
*   修复了一个问题，如果你在显示比例改变后打开任务栏溢出弹出按钮，它可能会出现浮动远离任务栏。

**【开始】**

*   修正了一个问题，导致意外的字符显示，而不是在电源菜单的睡眠选项的工具提示撇号。
*   修正了一个问题，可能会导致开始菜单崩溃时，一些人启动搜索亮点启用。

**【文件浏览器】**

*   如果任务栏被设置为自动隐藏并且文件资源管理器被最大化，将鼠标悬停在屏幕底部来调用任务栏现在应该可以工作了。
*   修正了一个问题，当拖放一个文件夹以将其固定到导航窗格时，在黑暗模式下指示其插入位置的线没有足够的对比度。
*   我们修复了一个问题，即文件浏览器中的搜索框背景可能与您当前的模式颜色相反(例如，在亮模式下为暗)。
*   修复了文件资源管理器在从特定位置启动后(例如，当从 Microsoft Edge 打开下载文件的位置时)，在完成绘制之前会出现打开、关闭和重新打开的问题。
*   修正了某些文件在你锁定后无法从主页的收藏夹中移除的问题。
*   进行了另一个修复，以帮助解决在暗模式和亮模式之间切换时，如果文件资源管理器窗口在切换时是打开的 UI 问题。
*   修复了在文件资源管理器中调整导航窗格大小时的 GDI 对象泄漏，对于经常调整导航窗格大小时，这可能会导致文件资源管理器中的内容随着时间的推移而无法正确呈现。
*   做了一些改进，以帮助在使用云存储提供商(如 OneDrive)备份文件资源管理器中的文件时加载 Home 的性能。

**【设置】**

*   修正了一些人在扫描阶段导致设置中的存储页面和磁盘清理崩溃的问题。
*   修复了一个问题，URIs 打开页面下的帐户设置部分不适合某些人-设置会打开，但不会导航到正确的页面。这影响了“开始”菜单中打开登录选项的链接。
*   修正了在隐私与安全>语音激活下导致应用图标显示不正确的问题。
*   修正了使用应用程序>安装的应用程序卸载应用程序时设置崩溃的问题。

**【其他】**

*   修正了当你停止投射到另一个显示器或者切换到复制你的显示器时，有时会导致 ShellExperienceHost.exe 崩溃的问题。
*   如果检测到 Unicode 输入，向 [findstr](https://docs.microsoft.com/windows-server/administration/windows-commands/findstr) 添加一个警告，以更清楚地说明这是否是某些文件没有返回结果的原因。
*   修正了最近航班中的一个问题，导致从某些应用程序打印表格时不包括行。
*   修正了一个在最近的飞行中可能导致某些应用程序挂起的问题。

还有一些需要注意的已知问题，这是任何预发布软件都应该注意的。

### Windows 11 内部版本 25193 中的已知问题

**【常规】**

*   一些使用 Easy Anti-check 的游戏可能会崩溃或导致您的电脑进行错误检查。
*   我们正在调查一些内部人员在升级到最新航班后音频停止工作的报道。
*   我们正在调查一些不同的应用程序在最近的版本中开始崩溃的报告。
*   [ **NEW** 我们正在调查内部人员在某些游戏中移动鼠标时遇到错误检查的报告
*   [ **新功能**我们正在调查一些内部人员在每次电脑重启时看到 OneDrive setup 请求设置权限的报告。

**【文件浏览器】**

*   [ **NEW** ]我们正在调查一小群“在单独的进程中启动文件夹窗口”的内部人员在上周的飞行后无法打开文件资源管理器的报告。
*   [ **NEW** ]我们正在解决一个问题，即命令栏中的复制、粘贴和清空回收站等项目可能会意外地在应该启用的时候被禁用。

**【微件】**

*   任务栏上的通知徽章编号可能会出现错位。
*   在某些情况下，某些徽章的通知横幅不会出现在小部件板上。
*   [ **新** ]我们正在调查一些内部人员的任务栏中天气显示不正确的报告，缺少文本，天气图标升得太高。

至于你什么时候可以期待这些功能在其他渠道出现，应该不会太久。像这样的功能经常在不需要完全更新操作系统的情况下进行调整，这种变化很可能是微软未来推出的较小功能的一部分。报告表明，微软将在 [Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2/) 之后支持这些功能下降，而不是主要的年度更新。

* * *

来源:[微软](https://blogs.windows.com/windows-insider/2022/09/01/announcing-windows-11-insider-preview-build-25193/)