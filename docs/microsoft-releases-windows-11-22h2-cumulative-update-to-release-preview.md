# 微软发布新的 Windows 11 22H2 更新以发布预览版

> 原文：<https://www.xda-developers.com/microsoft-releases-windows-11-22h2-cumulative-update-to-release-preview/>

# 微软发布 Windows 11 22H2 累积更新发布预览版

微软在发布预览频道为运行下一版本 Windows 11 的用户发布了新的累积更新。

今天，微软向发布预览频道发布了[Windows 11](https://www.xda-developers.com/windows-11/)Insider Preview build 22621.169。这是 Windows 11 版本 22H2 的 RTM 版本的累积更新，像往常一样，它包含一堆修复。

有几个这样的更新围绕着发布预览版渠道，因为在那个渠道中有几个层次。那些不符合 Windows 11 硬件要求的人仍在测试 Windows 10 版本，那些没有选择测试 22H2 版本的人正在测试 21H2 版本的最新更新。这些更新最终将在本月晚些时候作为可选更新向非内部人士展示，然后在下个月的补丁星期二作为强制更新。

当然，实际上这并不是这个特定版本的情况，因为 Windows 11 版本 22H2 还没有对非内部人士开放。这是我们将在今年晚些时候看到的东西，可能在 10 月份左右。

像往常一样，Windows 11 build 22621.169 包含了一大堆修复。虽然以前在累积更新中有一些功能，但这里没有任何正面的功能。

### Windows 11 构建 22621.169 修复程序

*   ***新增！*** 我们增加了服务器消息块(SMB)重定向器(RDR)特定的公共文件系统控制(FSCTL)代码 fs CTL _ LMR _ 查询 _ 信息。
*   ***新增！*** 我们在 Windows 客户端和服务器轻量级目录访问协议(LDAP)实现中增加了对传输层安全(TLS) 1.3 的支持。
*   ***新增！*** 我们在 Windows 客户端和服务器轻量级目录访问协议(LDAP)实现中增加了对传输层安全(TLS) 1.3 的支持。
*   我们更新了 **Remove-Item** cmdlet 以正确地与 Microsoft OneDrive 文件夹交互
*   我们启用了**InternetExplorerModeEnableSavePageAs**组策略。有关更多信息，请参见[微软 Edge 浏览器政策文档](https://docs.microsoft.com/deployedge/microsoft-edge-policies#internetexplorermodeenablesavepageas)。
*   我们修复了一个问题，当你使用一个公共文件对话框打开相机时，拍照按钮会消失。
*   我们修复了一个问题，该问题会阻止设备从 Windows Update 接收相同扩展驱动程序的报价，因为该扩展驱动程序已安装，但没有基本驱动程序。
*   我们修复了导致 Active Directory 从媒体安装(IFM)创建失败的问题，并显示错误“2101 JET_errCallbackFailed”。
*   我们修复了 Active Directory 轻型目录服务(LDS)重置 userProxy 对象的密码时出现的问题。密码重置失败，并出现错误，如“00000005: SvcErr: DSID-03380C23，问题 5003 (WILL_NOT_PERFORM)，数据 0”。
*   我们启用了**InternetExplorerModeEnableSavePageAs**组策略。有关更多信息，请参见[微软 Edge 浏览器政策文档](https://docs.microsoft.com/deployedge/microsoft-edge-policies#internetexplorermodeenablesavepageas)。
*   我们修复了 Active Directory 轻型目录服务(AD LDS)重置 userProxy 对象的密码时出现的问题。当您尝试重置其他人的密码并且您使用简单绑定进行了身份验证时，密码重置会失败。错误类似于“00000005: SvcErr: DSID-03380C23，问题 5003 (WILL_NOT_PERFORM)，数据 0”。
*   我们修复了阻止 Microsoft Edge 在 Windows 沙盒中可用的问题。

像往常一样，您可以通过 Windows Update 获得此更新。如果您不在发布预览频道，您可以转到“设置”->“Windows Update”->“Windows Insider 计划”进行注册。然后，你可以选择测试 Windows 11 版本 22H2 来获得此更新，但你会首先发现许多新功能。

来源:[微软](https://blogs.windows.com/windows-insider/2022/06/30/releasing-windows-11-build-22621-165-to-the-release-preview-channel/)