# 据报道，微软通过注入广告来破坏 Windows 11

> 原文：<https://www.xda-developers.com/microsoft-breaks-windows-11-by-injecting-ads/>

自从 Windows 10 推出以来，微软一直在其操作系统中推广广告，这显然不会随着 Windows 11 而改变。它始于臭名昭著的 Get Windows 10 应用程序，该应用程序会将自己强加给 Windows 7 和 8.1 用户，通常会提供误导性的选项，诱使你升级。那是很久以前的事了，现在的广告也没那么邪恶了。

除非他们打碎东西。昨天在 [Dev](https://www.xda-developers.com/microsoft-moves-windows-11-dev-channel-prerelease-builds/) 和 [Beta](https://www.xda-developers.com/new-windows-11-build-beta-channel-fixes-issues/) 频道发布了新的 Windows 11 版本(注意，是两个不同的版本)后，内部人士报告说他们的开始菜单和任务栏崩溃了。事实证明，这是由 Windows 11 发送广告引起的，正如丹尼尔·亚历山大报道的[，他深入研究了这个问题。](https://www.ctrl.blog/entry/windows11-empty-taskbar.html)

首先，微软确实发布了一个修复程序。如果你的电脑处于无法使用的状态，而你正在努力摆脱这种状态，这就是你需要做的:

> *   **第一步:**使用 CTRL-ALT-DEL，选择打开任务管理器。
> *   **第二步**:选择任务管理器底部的“更多详情”展开任务管理器。
> *   **第三步**:进入“文件”，选择“运行新任务”。
> *   **步骤 4:** 在“Open”字段中输入“cmd”。
> *   **第五步:**粘贴以下内容(一切以粗体显示): **reg 删除 HKCU \软件\微软\ Windows \ current version \ iris service/f&shut down-r-t 0**
> *   第六步:按回车键，然后你的电脑应该会重启。重启后，一切都应该恢复正常。

没错；为了使您的电脑从因 Microsoft 向其发送广告而导致的严重问题中恢复过来，您需要对注册表进行更改。

广告本身是针对微软团队的，以及它是如何整合到 Windows 11 中的。和大多数注入到 Windows 中的广告一样，即使你关闭了所有的通知，它仍然会以通知的形式弹出。

虽然我们知道原因，但 Aleksandersen 探究的更大问题是，Windows 11 的外壳是如何如此脆弱，以至于广告可以摧毁它。2021 年的 Windows 中有大量的组件，这些组件必须在任何给定的时间从云中获取内容，从 Bing 锁屏壁纸到 Windows Update，再到来自微软的广告。很奇怪，当其中一个功能不正常时，这种情况就会发生。

虽然你的第一个想法可能是将这种不稳定性作为你注册 Windows Insider 计划的原因，但请记住，这种情况在测试版渠道*和开发版渠道*中都发生过。Windows 11 build 22000.176 是后 RTM 版本，这意味着如果你在 10 月 5 日 Windows 11 发布后购买新的笔记本电脑，你应该会获得更早版本的操作系统。测试频道中提供的内容几乎不能再被认为是预览版了。

这里显然有两个问题。一个是云服务可以攻破 Windows 11。另一个原因是微软首先在操作系统中注入广告，这对许多人来说肯定是一个痛点。有一点是肯定的；微软短期内不会缩减在 Windows 上的广告投放。相反，它只是要修复这个小故障，如果这让你把 [*比作*](https://www.youtube.com/watch?v=MR9DHNEYXN8) ，那也没问题。