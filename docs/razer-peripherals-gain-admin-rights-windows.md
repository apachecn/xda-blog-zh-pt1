# Razer 漏洞允许任何人获得 Windows PC 上的管理员权限

> 原文：<https://www.xda-developers.com/razer-peripherals-gain-admin-rights-windows/>

最近不断有 [Windows 漏洞](https://www.xda-developers.com/windows-10-vulnerability-lets-anyone-get-administrator-privileges/)被发现，甚至在新推出的 [Windows 365 服务](https://www.xda-developers.com/windows-365-expose-azure-credentials-plain-text/)中。现在，一名安全研究人员发现了一个漏洞，该漏洞可以让任何拥有 Razer 外设的人获得 Windows PC 的管理员权限。研究人员[在 Twitter 上被称为 Jon hat](https://twitter.com/j0nh4t)，他发现插入 Razer USB 外设可以让用户轻松获得电脑的管理员权限。

该漏洞的工作方式是，一旦你插入 Razer 设备，Windows Update 将下载并安装 Razer Synapse。这是 Razer 的软件，用于控制诸如宏和色度灯光效果之类的东西。但是，因为安装程序是由 Windows Update 下载的，所以它是以系统用户的身份运行的，这是一个具有管理员权限的高度受信任的用户组。

在安装过程中，安装程序会要求用户选择一个目录来安装 Synapse，并且会打开一个文件浏览器窗口。因为安装程序是由系统用户运行的，所以用户可以按下 *Shift* 键并右键单击空白区域，以管理员权限打开 PowerShell 窗口。从这里开始，PowerShell 允许您使用管理员权限做的任何事情都是可能的。

问题变得更加严重。如果你将 Razer Synapse 文件保存到一个用户可控制的文件夹中——比如桌面、文档和其他——保存在那里的文件之一可能会被劫持。这使得潜在的攻击者能够在以后持续获得管理员权限。最重要的是，你甚至不需要一个真正的 Razer 设备。即使插入了不同的设备，也可以伪造设备 id 来欺骗 Windows Update 下载 Razer Synapse。Twitter 用户 an0n 分享了一段视频，视频中使用 Android 手机而不是 Razer 设备进行了同样的攻击。

Windows 漏洞最初被报告给 Razer，但没有回应，研究人员通过上面的视频将问题公之于众。然而，随着它的公开曝光，Razer [已经联系了](https://twitter.com/j0nh4t/status/1429462941070409728)，并确认它将确实修复这个问题。作为对研究人员的奖励，即使漏洞被公开披露，公司仍将为发现问题提供赏金奖励。