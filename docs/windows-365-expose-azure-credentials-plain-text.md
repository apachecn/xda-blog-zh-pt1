# Windows 365 可用于以纯文本形式公开 Azure 凭据

> 原文：<https://www.xda-developers.com/windows-365-expose-azure-credentials-plain-text/>

Windows 365 问世还不到两周，但研究人员已经在这项服务中发现了安全漏洞。mimikatz 项目的创始人、研究员 Benjamin Delpy 发现，在使用 Windows 365 时，有可能以纯文本形式暴露用户的 Azure 凭据。该漏洞确实需要管理权限来利用，但它仍然是一个威胁窗口。

正如 [*电脑*](https://www.bleepingcomputer.com/news/microsoft/windows-365-exposes-microsoft-azure-credentials-in-plain-text/) 解释的那样，该漏洞利用了微软远程桌面连接中的一个漏洞，德尔皮[最初在 5 月](https://twitter.com/gentilkiwi/status/1397263983221039105)发现了该漏洞。当您创建云 PC 时，它实际上是安装在云中的虚拟机，您可以通过远程桌面连接进行访问。该漏洞允许用户使用 mimikatz 等工具暴露客户端上使用的远程桌面凭据。

使用 Windows 365 访问云 PC 也使用远程桌面协议，因此漏洞在这里的工作方式类似。由于 Windows 365 绑定了 Azure，所以这次曝光的凭证是针对你的 Azure 账户的。此外，即使您通过 web 浏览器访问 Windows 365 云 PC，这也能正常工作，因为它仍然使用远程桌面协议。

正如我们提到的，这也需要访问 PC 和管理权限。但是还有其他漏洞可以被利用来获得对系统的访问。恶意的电子邮件附件可以授权攻击者访问您的 PC，并且可以利用其他漏洞获得管理权限。问题是，在这里获取您的凭据不仅仅是访问您自己的 PC，它可能会允许攻击者传播到您组织中的其他 Microsoft 服务，最终影响整个公司的内部网络。它可能会暴露数百名用户，即使其中只有一人打开了最初的攻击窗口。

通常，避免这种威胁的一种方法是使用传统密码的替代品。Windows Hello 或双因素身份验证通常可以防止这种情况，但 Windows 365 还不支持这些功能。据推测，微软正在努力为云电脑启用这些功能，但目前，如果你使用的是 Windows 365，最好格外小心。