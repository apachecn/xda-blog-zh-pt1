# Android 版 Swiftkey 准备添加与 Windows 10 同步的剪贴板

> 原文：<https://www.xda-developers.com/swiftkey-android-share-clipboard-windows-10/>

自从谷歌的 GBoard 出现以来，它可能不是本月的特色，但微软拥有的 Swiftkey 仍然继续为其自己的 Android 键盘体验带来改进。下一个主要功能看起来像是 Windows 10 的剪贴板同步。

由于一些逆向工程，Android 开发者 Alessandro Paluzzi 在最近的 SwiftKey 发布中发现了新功能(通过 [*9to5Google*](https://9to5google.com/2020/10/26/swiftkey-on-android-may-gain-windows-10-clipboard-sync-feature/) )。新菜单选项的描述称，你可以“从其他 Windows 设备上复制和粘贴文本”当然，你必须“在你的 Windows 设备上也启用它”，一旦你这样做了，微软警告它“接收你的剪贴板数据以在你的 Windows 设备上同步。”

这当然是有道理的。一段时间前，微软正式采用 Android 作为其移动平台，任何有助于与其自身生态系统实现更无缝体验的东西都将成为开发者的首要任务。

三星用户已经有了类似的“[链接到 Windows](https://www.xda-developers.com/link-to-windows-1-5-allows-drag-drop-between-samsung-galaxy-phones-pc/) ”功能，但这给其他安卓品牌带来了相同的功能，增加了云元素，这应该可以防止任何基于设备的限制。事实上，当合作关系宣布时，微软声称，如果没有个别原始设备制造商的合作，其他设备的原生剪贴板同步将是不可能的，这要感谢[Android 10+](https://www.xda-developers.com/android-q-blocks-background-clipboard-access/)的限制。然而，由于 SwiftKey 是一种输入法，这些限制不适用于它对剪贴板数据的访问。

不过，我们暂时还不知道这在实践中会如何运作，因为这个功能还没有上线。此外，确切的机制还不清楚——它会是一个专用按钮吗？长按？汉堡菜单？在拥挤的键盘空间中，它们都有各自的优点和缺点。

第二个也可能是更为紧迫的是安全和隐私的老问题。我们谈论的是一种功能，它可以将你放在剪贴板上的任何内容发送到云端，然后再返回。这意味着它将通过任何数量的节点，在那里它可以被拦截。在我们考虑用它复制银行信息之前，我们要非常非常确信它是无法渗透的。

无论发生什么，在 SwiftKey 公开这一功能之前，仍有许多问题没有答案。最值得注意的是，我们没有时间表来确定这个特性何时或者是否会达到稳定版本。与此同时，它会返回到您的共享菜单。