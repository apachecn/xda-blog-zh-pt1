# 微软推出阻止 Windows 11 用户登录问题的修复程序

> 原文：<https://www.xda-developers.com/microsoft-fixes-issue-windows-11-msa-sign-in/>

微软已经确认并发布了 Windows 11 中一个漏洞的修复程序，该漏洞可能导致用户在向 Windows 添加新的微软帐户后无法登录。该问题首次出现在 8 月 25 日推出的 Windows 11 最新可选更新(标记为 [KB5016691](https://support.microsoft.com/en-us/topic/august-25-2022-kb5016691-os-build-22000-918-preview-59097044-915a-49a0-8870-49823236adbd) ，或 build 22000.918)之后，因此除非你选择安装该更新，否则你可能不会注意到。

据微软解释，该问题只会影响拥有微软帐户的用户-这意味着 Active Directory 和 Azure AD 帐户不会受到影响-并且只有在安装更新后向 Windows 添加微软帐户时才会发生。此外，登录问题仅在首次登录时出现，并且仅在重启或注销电脑后的“短暂时间”内出现，这意味着它会及时消失。

在承认问题的同时，微软立即发布了使用已知问题回滚的修复程序，这是修复累积更新问题的常用方法。这是一个微小的配置更改，您看不到，但只要您连接到互联网，问题应该会在 24 小时内得到解决。微软表示，如果你重启设备，修复程序可能会更快应用，以防你等不起。

如果您在企业环境中，并且需要立即修复，您可以使用组策略编辑器来手动应用修复。可以到**电脑配置** - > **管理模板**->**kb 5016691 220722 _ 051525 已知问题回滚** - > **Windows 11(原版本)**安装配置策略。这应该允许您再次使用 Microsoft 帐户登录 Windows 11。

这种问题在 Windows 累积更新中并不罕见。就在上周，微软不得不发布另一个修复程序——这一次是针对 Windows 10——这个问题可能导致[在某些情况下无法播放音频](https://www.xda-developers.com/windows-10-update-audio-issue/)。考虑到这个问题出现在周二补丁发布的强制更新中，这个问题实际上更令人担忧。

* * *

来源:[微软](https://docs.microsoft.com/en-us/windows/release-health/status-windows-11-21h2#2896msgdesc)

Via: [Neowin](https://www.neowin.net/news/microsoft-confirms-windows-11-may-not-let-you-sign-in-after-adding-microsoft-account/)