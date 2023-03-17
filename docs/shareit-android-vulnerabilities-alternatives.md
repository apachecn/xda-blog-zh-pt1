# PSA:如果你在 Android 上使用 ShareIt，你可能应该寻找替代品

> 原文：<https://www.xda-developers.com/shareit-android-vulnerabilities-alternatives/>

如果你正在手机上使用 ShareIt 应用程序，你可能需要立即卸载它。网络安全巨头*趋势科技*在文件共享应用中发现了明显的安全漏洞，这些漏洞可以被*滥用来泄露用户的敏感数据并使用 ShareIt 权限执行任意代码。*

在关于此事的[报告](https://www.trendmicro.com/en_us/research/21/b/shareit-flaw-could-lead-to-remote-code-execution.html)中，*趋势科技*透露([via*Ars Technica*](https://arstechnica.com/gadgets/2021/02/shareit-android-app-with-over-a-billion-downloads-is-a-security-nightmare/))share it 由于其提供的功能，可以访问 Android 上的无数[权限](https://www.xda-developers.com/tag/permissions/)。该应用程序可以访问整个存储和所有媒体，使用摄像头和麦克风，访问位置信息，等等。它甚至可以删除其他应用程序，启动时运行，创建帐户，设置密码。此外，ShareIt 还拥有完整的网络访问权限。由于这一广泛的权限列表，损害应用程序可以帮助攻击者获得对您的手机和所有敏感信息的几乎完全的访问权限。它还让攻击者远程执行恶意代码。

在阐述其中一个漏洞时， *Ars Technica* 透露，ShareIt 有一个[常见的 Android 应用漏洞](https://blog.oversecured.com/Android-Access-to-app-protected-components/)，该漏洞可以让攻击者对其所有文件进行读/写访问。该出版物指出:*“Android 以应用内通信为傲，部分原因是任何应用都可以创建一个内容提供商，并向其他应用提供其内容和服务。如果 Gmail 想要在电子邮件中附加文件，它可以通过显示安装在手机上的可用文件内容提供商列表来实现(这基本上是一个“打开方式”对话框)，用户可以选择他们最喜欢的文件管理器，浏览他们的存储，并将他们想要的文件传递给 Gmail。开发人员需要清理这些跨应用程序的功能，并且只向 Gmail 和其他应用程序展示必要的文件管理器功能。”*

然而，ShareIt 背后的开发人员并没有考虑限制该应用程序的内容提供商功能，这可能会让攻击者访问 ShareIt“私人”目录中的所有文件。实际上，该漏洞允许攻击者调用 ShareIt 的文件内容提供商，并向其传递文件路径，以访问其所有数据文件。这允许第三方应用程序编辑 ShareIt 用于运行的数据，包括安装和运行时生成的应用程序缓存。*趋势科技*声称*“攻击者可能会创建一个伪造的文件，然后通过上述漏洞替换这些文件来执行代码。”*

由于 ShareIt 也有一个 Android 应用安装程序，它也容易受到“中间人”攻击。由于上面提到的漏洞，攻击者能够在下载后立即用恶意应用程序替换安装包。这可能会导致用户在不知不觉中在他们的设备上安装恶意应用程序。此外，ShareIt 的游戏商店能够通过不安全的 HTTP 下载应用程序数据。这可能会受到“中间人”攻击。正如 Ars Technica 解释的那样，*“share it 将自己注册为任何结束其域名的链接的处理程序，如“wshareit.com”或“gshare.cdn.shareitgames.com”，当用户点击下载链接时，它会自动弹出。大多数应用会强制所有流量流向 HTTPS，但 ShareIt 不会。Chrome 将关闭 HTTP 下载流量，因此这必须通过主浏览器以外的网络界面来完成。”*

趋势科技已经向 ShareIt 报告了这些漏洞，但其开发人员迄今尚未发布任何补丁来解决这些问题。我们建议卸载应用程序，直到开发人员发布修复程序。在那之前，你可以使用谷歌的[文件应用](https://www.xda-developers.com/tag/google-files-go/)来满足你所有的本地文件共享需求。