# 微软让在 ARM 上为 Windows 11 构建应用变得更加容易

> 原文：<https://www.xda-developers.com/64-bit-office-windows-11-arm/>

微软刚刚在 Dev 频道向内部人士发布了第一个 Windows 11 版本,它包括了大量的新功能。但是你在构建中看到的并不是一切。微软还宣布，它将让开发者更容易在 ARM 上为 Windows 11 开发更快的应用程序。微软[称之为 ARM64EC](https://blogs.windows.com/windowsdeveloper/2021/06/28/announcing-arm64ec-building-native-and-interoperable-apps-for-windows-11-on-arm/) ，EC 代表“仿真兼容”。这是开发人员更容易将其 x64 应用移植到 ARM 的一种方式，而不必重新编译整个应用。与此同时，在 ARM 上有一个新的 64 位版本的 Office for Windows 11。

正如微软所说，ARM64EC 是 ARM 上 Windows 11 的应用程序二进制接口(ABI)，可以与 x64 互操作。这意味着开发人员可以创建一个应用程序，将 ARM64EC 用于一些进程或模块，将 x64 用于其他进程或模块。ARM64EC 代码原生运行在 ARM 上，而 x64 组件使用仿真层，这也是 Windows 11 中的新功能。然而，开发人员可以将 ARM64EC 单独用于他们的应用程序。

这意味着开发人员可以逐渐过渡他们的应用程序，使其在 ARM 设备上完全原生，而不是必须一次转换所有内容。通过利用 ARM64EC，x64 组件仍然可以用在最有意义的地方，例如，如果某个特定功能不需要本机性能或不常使用。每个模块和进程都可以在开发人员认为合适的时候过渡到 ARM64EC。

## 用于 ARM 上的 Windows 11 的 64 位 Office

为了证明新 ABI 的价值，微软[今天](https://insider.office.com/en-us/blog/64-bit-office-for-windows-on-arm)还宣布在 ARM 上推出 64 位版本的 Office for Windows 11。包括 Word、Excel、PowerPoint、OneNote 和 Outlook 在内的核心 Office 应用程序现在都可以作为 ARM64EC 应用程序使用。这些都是复杂的应用程序，有大量的模块，所以并不是所有的都转换到原生的 ARM 架构。但有了这个新工具，部分代码现在可以本机运行，所以所有这些模块现在第一次可以在 ARM PCs 上使用。此外，微软表示，在基于英特尔或 AMD 的电脑上运行这些应用程序，你不会感觉到性能差异。

你可以通过查看任务管理器中的架构选项卡来判断哪些应用是基于 ARM64EC 的。这些应用程序将被标记为 ARM64 (x64 兼容)。其他应用程序将被标记为 x64 应用程序，它们将在 x64 仿真模式下运行。

要尝试这一点，你必须运行新的 Windows 11 Insider 预览版，并拥有一台基于 ARM 的 PC。然后，如果你有 32 位版本的 Office，你需要卸载它，然后从 Office.com 下载最新版本。安装完成后，你必须进入账户菜单，注册 Office Insider 程序的测试版。更新到最新的内部版本后，您应该启用这些功能。

这个初始版本有一些限制，比如团队与 Outlook 的集成还没有完成。您可能还会发现，有些搜索在 Outlook 和 OneNote 等应用程序中不起作用。

你可以期待这些事情在今年晚些时候 Windows 11 发布时得到解决。到那时，应该会有其他应用程序利用这个新工具。