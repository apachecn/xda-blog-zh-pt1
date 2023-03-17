# 微软将 Android 应用支持引入 Windows 11

> 原文：<https://www.xda-developers.com/windows-11-android-apps/>

今天，微软正式公布了新版 Windows: Windows 11。在这次活动中，微软详细介绍了桌面操作系统在视觉和生产力方面的一些变化。活动接近尾声时，微软宣布了一个令人惊讶的消息:该公司将通过与亚马逊应用商店的合作，将安卓应用程序带到 Windows 11 上。

在最初关于 Android 应用程序集成功能的主题演讲中，很少分享技术细节，但在随后的开发者主题演讲中，微软表示他们开发了一个“Android Windows 子系统”(WSA)，类似于 Windows 中已经存在的“Linux Windows 子系统”。应用程序显示在顶层窗口中，可以固定在开始菜单上，调整大小，捕捉，并像任何原生 Windows 应用程序一样进行管理。微软表示，在幕后，Windows 11 创建了一个代理本地应用程序，处理 Android 应用程序模型和 Windows 应用程序模型之间的桥梁。为了让代码运行，微软采用了他们在开发 WSL 时取得的进步——并将 Linux 内核引入 Windows——来构建 WSA。Android 应用运行在虚拟机中，虚拟机提供了与 AOSP 框架的兼容性，键盘、鼠标、触摸、笔和蓝牙音频耳机等设备都是兼容的。

由于大多数 Android 应用程序都是为 ARM 处理器构建的，因此微软与英特尔合作，使用后者的英特尔桥技术在英特尔和 AMD PCs 上运行 ARM 二进制文件。在另一篇博客文章中，英特尔[将](https://www.intel.com/content/www/us/en/newsroom/news/intel-tech-unleashes-windows-experience.html#gs.45lbc1)英特尔桥描述为“一个运行时后编译器，支持应用在基于 x86 的设备上本地运行。”目前尚未明确证实哪些基于英特尔的处理器将支持 Android 应用，尽管英特尔的博客帖子提到，该公司“预计将在今年及以后为 Windows 11 提供最广泛的计算体验，为消费者、企业、教育、爱好者等提供基于第 10 代、第 11 代和未来几代英特尔酷睿处理器的平台。”至于基于 ARM 的 Windows 个人电脑，据 [*The Verge*](https://www.theverge.com/2021/6/24/22549303/windows-11-intel-bridge-android-apps-amd-arm-processors) 报道，他们也将得到支持，尽管微软还不准备分享任何细节。

除了硬件兼容性，我们对这个消息的另一个担忧是，通过亚马逊的 Appstore 提供的应用数量与通过谷歌的 Play Store 提供的数量相比相形见绌。此外，Windows 11 不太可能会搭载谷歌移动服务，所以我们不知道某些应用程序是否会因为缺乏谷歌 Play 服务而在操作系统上表现不佳。鉴于亚马逊的 Fire 设备没有 GMS，因此提交到亚马逊应用商店的许多应用程序都是考虑到这一点而制作的，这应该不是太大的问题。

据《华尔街日报》的乔安娜·斯特恩称，你必须先下载并登录亚马逊应用商店，然后才能从微软商店下载安卓应用。这有点笨拙，但希望微软以后能改进这个过程。

Android 应用程序在 Windows 11 上的到来显然是为了应对苹果最近在 macOS 中集成 iOS 和 iPadOS 应用程序。苹果的整合之所以成为可能，是因为新款 MAC 电脑转向了基于 ARM 的处理器——苹果的 M1 芯片——而前者的实现要归功于与英特尔的合作。谷歌的 Chrome OS 也支持运行 Android 应用，也有办法[在 GNU/Linux 发行版上运行 Android 应用](https://www.xda-developers.com/anbox-allows-you-to-run-android-apps-on-any-gnulinux-os/)。

我们对这一宣布感到兴奋，并将在下周微软发布第一批 Windows 11 版本时深入研究 Android 应用集成。我们特别感兴趣的是了解在没有亚马逊应用商店的情况下将 Android 应用程序下载到 Windows 11 的过程，这显然是[有可能做到的](https://www.xda-developers.com/windows-11-support-installing-android-apps-amazon-appstore/)。