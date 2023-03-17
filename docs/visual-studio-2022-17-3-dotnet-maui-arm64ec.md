# Visual Studio 2022 17.3 增加了对的官方支持。NET MAUI 和 Arm64EC

> 原文：<https://www.xda-developers.com/visual-studio-2022-17-3-dotnet-maui-arm64ec/>

微软发布了面向 Windows 的 Visual Studio 2022 17.3，为开发人员带来了一些新功能，以及一系列其他改进。其中，如果你一直关注微软应用开发的新闻，有两个可能会很突出:官方支持。NET MAUI 和 Arm64EC。

随着这些功能成为官方功能，您现在可以开始在您想要发布的应用程序中使用它们，并对它们将按预期工作充满信心。。NET MAUI(或多平台应用程序 UI)是一套工具，让您使用单一共享代码库为 Windows、Android、iOS 和 macOS 创建应用程序。对于跨平台应用的开发者来说，这应该是一个很大的帮助，它还支持热重装等功能，这样你就可以实时看到你的代码变化如何影响应用。。NET MAUI 已经预览了一段时间，所以很高兴看到它终于得到官方支持。

同时，虽然在 Visual Studio 2022 17.3 的声明中没有提到 Arm64EC 支持，但有一篇单独的博客文章宣布了官方支持。这距离 [Arm64EC 首次发布](https://www.xda-developers.com/64-bit-office-windows-11-arm/)已经一年多了。如果你不知道，Arm64EC (Emulation Compatible)是一个应用程序二进制接口(ABI ),它允许开发人员在同一进程中创建混合 Arm64 和 x64 代码的应用程序。从本质上说，作为一名开发人员，这意味着您可以逐渐过渡到添加 Arm64 支持的应用程序，而不必完全重写。这对于像 Microsoft Excel 这样的应用程序也很重要，这些应用程序严重依赖于为 x64 设计的扩展。这样，核心应用程序本身可以过渡到 Arm64，而不会破坏与 x64 扩展的兼容性。事实上，微软的 Office 应用已经在 Arm 设备上使用 Arm64EC。

除了这些大的增加，Visual Studio 2022 17.3 还为 C++带来了更好的性能，以便在构建 C++应用程序时使用更少的 CPU 资源。此外，在 Visual Studio 中索引和着色 C++代码现在要快得多，微软分享了一个新的 Unreal Engine 5 解决方案的示例，其中 Visual Studio 173 需要 72 秒来索引，而 17.2 版本需要 146 秒。一个新的团队工具包现在也可以帮助你为微软团队开发应用程序。

还有许多其他的改进，如果你想深入了解这次更新中添加的所有内容，你可以在这里找到完整的发行说明。随着 Visual Studio 2022 17.3 的发布，微软也发布了。NET Framework 4.8.1，这是第一个完全支持 Arm64 的版本。在这方面，微软还宣布，Visual Studio 17.4 将是第一个在 Arm64 上完全原生的 Visual Studio 版本，今天发布了第一个预览版。你可以在这里下载 Visual Studio 2022 17.3 for Windows，或者如果你好奇的话在这里获得 17.4 预览版 1。

如果你用的是 macOS，那么面向 Mac 17.3 的 Visual Studio 2022 今天也发布了。该版本支持用户机密，新的代码修复可以帮助您提高工作效率，并且支持 App Store Connect 帐户，这是个人 Apple 开发者所必需的。这里有一个[变化的完整列表](https://docs.microsoft.com/en-us/visualstudio/releases/2022/mac-release-notes)。Visual Studio for Mac 17.4 今天也将进入预览版，最初支持。网毛伊岛。

不管你在找什么版本，你都可以在这里找到最新的 Visual Studio 下载。

* * *

来源:[微软](https://devblogs.microsoft.com/visualstudio/visual-studio-2022-17-3-is-now-available/)