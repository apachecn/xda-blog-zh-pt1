# RootMyRoku 可以越狱许多 Roku 电视和机顶盒

> 原文：<https://www.xda-developers.com/rootmyroku-jailbreak-roku-tv-set-top-boxes/>

Roku 最近[从其频道商店中移除了 YouTube 电视应用](https://www.xda-developers.com/roku-removes-the-youtube-tv-app/)，原因是[与谷歌](https://www.xda-developers.com/roku-could-lose-youtube-tv-google-spat/)的分歧，阻止用户在几周内观看他们最喜欢的节目。虽然谷歌已经找到了一种方法，通过巧妙地将服务[嵌入到主要的 YouTube 应用](https://www.xda-developers.com/google-youtube-tv-roku-youtube-app/)中来恢复 YouTube 电视，但它还没有与 Roku 达成妥协。这可能会导致 Roku 再次报复，最终可能会影响您的观看体验。

如果你想在将来避免这样的问题，你可以选择 root 你的 Roku 设备。root 将让你更好地控制你可以在设备上安装哪些应用/频道，所以你不必担心任何这样的不便。苹果世界的许多人都称之为“越狱”,这在安卓设备上非常简单。只需解锁引导加载程序，并使用一个名为 [Magisk](https://www.xda-developers.com/how-to-install-magisk/) 的工具为您修补引导映像，这是最难的部分。不过，Roku 设备不运行 Android，因此实现 root 访问/越狱的过程并不完全相同。

谢天谢地，有一个新的根漏洞将帮助你做到这一点。根据 [*Engadget*](https://www.engadget.com/rootmyroku-exploit-035749524.html) 最近的一份报告，“RootMyRoku”使用的漏洞利用了几乎所有 Roku 电视和一些 Roku 机顶盒上发现的一对漏洞。据开发者称，它可以在运行 RokuOS v9.4.0 build 4200 或更早版本的设备上工作，这些设备都有 Realtek Wi-Fi 芯片。

根据该项目的 [GitHub 页面](https://github.com/llamasoft/RootMyRoku)，RootMyRoku 提供了以下特性:

*   在端口 8023 上生成一个以 root 用户身份运行的人才服务器。
*   启用低级硬件开发人员模式。
*   增加了许多新的秘密屏幕和调试功能到主菜单。
*   阻止频道更新、固件更新以及与 Roku 服务器的所有通信。

最后一点值得注意，因为这意味着不能安装新频道，某些功能如“我的订阅源”和“搜索”将不再工作。然而，与非 Roku 服务(如 YouTube、网飞或 HBO)通信的频道仍将工作。

如果你有兴趣在你的 Roku 设备上尝试新的漏洞，只需按照上面链接的 GitHub 页面上的说明进行操作。请注意，该漏洞无法在运行 [RokuOS 10](https://www.xda-developers.com/roku-express-4k-streambar-pro-voice-remote-pro-roku-os-10/) 的设备上运行，因此您应该在对您的设备进行根操作之前检查您当前的软件版本。为此，请转到“设备设置”中的“系统”部分，选择“关于”选项。您应该在下一页看到您当前的软件版本。

该漏洞的技术细节和源代码可以在该项目的 GitHub 页面上找到。

* * *

## 更新:Roku 解决了 RokuOS v9.4 中的漏洞

Roku 发言人就上述漏洞联系了我们，并分享了以下声明:

> #### “作为我们持续监控的一部分，Roku 安全团队发现并解决了 Roku OS 中的漏洞——尽管这些漏洞没有暴露客户数据，我们也没有发现任何恶意活动。我们总是想尽一切努力为 Roku、我们的合作伙伴和我们的用户维护一个安全的环境，因此我们在不影响最终用户体验的情况下缓解了漏洞并更新了 Roku OS 9.4。”

当我们要求确认时，Roku 发言人明确告诉我们，OS 9.4“修复”了 RootMyRoku 使用的漏洞。