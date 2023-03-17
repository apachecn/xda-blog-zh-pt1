# Visual Studio 2022 预览版 2 现在提供了新的图标和功能

> 原文：<https://www.xda-developers.com/visual-studio-2022-preview-2-now-available/>

大约一个月前，微软[发布了 Visual Studio 2022 的首个预览版](https://www.xda-developers.com/visual-studio-2022-is-now-in-preview-built-for-64-bit-pcs/)。这是专门为 64 位 PC 构建的 IDE 的第一个版本，所以第一个版本的重点是发现和修复过渡中的问题。没有太多新的东西。然而今天，我们得到了 [Visual Studio 2022 预览版 2](https://devblogs.microsoft.com/visualstudio/visual-studio-2022-preview-2-is-out/) ，它带来了更多的新功能。

对于初学者来说，这个新的预览实际上是本地化的，所以如果你说英语以外的任何语言，你现在可以使用 Visual Studio 2022。Preview 2 还带来了更新的图标和微软今年早些时候承诺的新 Cascadia 代码字体。新图标旨在更易于理解，使 Visual Studio 更易于使用。

微软还在 Visual Studio 2022 Preview 2 中增加了一些新的生产力改进，首先是 XAML 和 web 应用程序的新实时预览。实时预览允许用户在 IDE 中进行更改，并在他们构建的应用程序中实时查看这些更改。可以使用代码编辑器或直接从预览中进行更改。微软还增加了一个名为 Force Run 的新选项，允许开发人员运行应用程序直到特定的点，而不管代码中的任何其他断点。

Visual Studio 2022 Preview 2 中的另一大新功能是支持 C++应用程序中的热重新加载。热重载允许开发人员在应用程序运行时对其代码进行更改，并在不关闭应用程序的情况下应用这些更改。虽然这取决于您所做的更改，但您甚至可以在根本不暂停应用程序的情况下应用这些更改。

如果您想深入了解更多的技术细节，还有更多的新内容。以下是完整的 changelog:

### Visual Studio 2022 预览版 2 的完整变更日志

**C++**

*   现在，您可以在 WSL2 上进行本地构建和调试，而无需建立 SSH 连接。跨平台 CMake 项目和基于 MSBuild 的 Linux 项目都受支持。
*   v143 构建工具现在可以通过 Visual Studio 安装程序以及[独立构建工具](https://aka.ms/vs/17/pre/vs_BuildTools.exe)获得。
*   Visual Studio 现在支持 CMakePresets.json 中的`buildPresets.targets`选项。这允许您在 CMake 项目中构建目标的子集。
*   CMake 项目中的项目菜单已经过简化，并显示了“删除缓存并重新配置”和“查看缓存”选项。
*   代码分析现在强制要求必须检查用`_Check_return_`或`_Must_inspect_result_`标注的函数的返回值。
*   Visual Studio 附带的 LLVM 工具已经升级到 LLVM 12。详见 [LLVM 发行说明](https://releases.llvm.org/12.0.0/docs/ReleaseNotes.html)。
*   Clang-cl 支持更新到 LLVM 12。
*   C++ AMP 头现在已被弃用。在 C++项目中包含<amp.h>会产生构建错误。要消除错误，请定义`_SILENCE_AMP_DEPRECATION_WARNINGS`。详情请见 https://aka.ms/amp_deprecate 的[。](https://aka.ms/amp_deprecate)</amp.h>
*   在调试器下运行时，本机 C++应用程序现在可以获得新的热重新加载体验。欲了解更多信息，请参见下面的[热重装部分](https://docs.microsoft.com/en-us/visualstudio/releases/2022/release-notes-preview#HotReload-170P2)。

**调试&诊断**

*   附加到进程对话框改进
*   异常助手改进
*   强制运行点击
*   内存转储诊断分析

**。净生产率**

*   引入参数重构可以将新参数从方法实现移动到其调用方。
*   跟踪数据流分析的价值源
*   给重新赋值的变量加下划线的选项
*   在生成覆盖对话框中增加了搜索选项
*   XML`标签的快速信息现在保留空白和 CDATA 块`
*   “查找所有引用”窗口现在将对多目标项目进行分组
*   重构以移除 Visual Basic 中的重复类型
*   “转到实现”将不再导航到具有也被重写的抽象声明的成员。

**剃刀(ASP.NET 核心)编辑**

*   Razor 文件中的热重装支持
*   性能改进
*   格式和缩进增强
*   新 Razor 编辑器颜色
*   标签助手现在是彩色的，并且有快速信息分类支持和完成工具提示
*   Razor 构造的尖括号突出显示和导航
*   注释现在有自动完成、智能缩进、自动包含注释延续和块注释导航

**热重装**

*   热重装(两者皆适用。NET 和 C++代码)使得对正在运行的应用程序进行多种类型的代码编辑并应用它们成为可能，而无需像断点那样暂停应用程序的执行。在这个版本中我们继续改进这个特性，亮点包括:支持 C++。NET 热重载，支持更多类型的编辑等等。

**可信位置**

*   我们改进了“信任设置”功能，现在可以在 ide 中打开不受信任的代码(如文件、项目或文件夹)时显示警告。

**XAML 现场预告**

*   XAML 现场预览版现已面向 WPF 开发者开放，作为这一全新体验的第一次预览。通过实时预览，我们能够捕获桌面应用程序用户界面，并将其带入 Visual Studio 内的停靠窗口，从而更容易使用 XAML 热重装来更改应用程序，并在您进行更改时轻松查看更改。该功能改善了单屏幕设备上的 XAML 热重装体验，同时还可以使用深度缩放、标尺、元素选择和信息提示等工具来完善应用程序 UI。

**远程测试**

*   **非常早的试验预览，支持在远程环境上运行测试，比如 linux 容器、WSL 和 over SSH 连接。**

**用户界面**

*   默认图标已经更新和刷新。

**Azure 云服务**

*   现在支持 Azure 云服务(经典)和 Azure 云服务(扩展支持)项目。

**JavaScript/类型脚本**

*   我们已经发布了一个新的 JavaScript/TypeScript 项目类型，它可以使用额外的工具构建独立的 JavaScript/TypeScript 项目。您将能够使用计算机上安装的框架版本在 Visual Studio 中创建 Angular 和 React 项目。
*   JavaScript 和 TypeScript 测试现在在 Visual Studio 测试资源管理器中可用

**本版本中解决的问题**

*   修复了在 IIS Express 中运行 ReactRedux 时网站无法加载的问题。
*   修复了导致错误消息的问题:“未捕获的引用错误:notifyHotReloadApplied 未定义”。
*   修复了使用 Ctrl+F5 时无法连接到 6.0 signalR 项目的服务器的问题。
*   修正了包含搜索顺序可能不正确的问题。
*   修复数据库项目:从解决方案资源管理器拖动文件到一个打开的文件是从文件系统中删除文件！

**来自开发人员社区的顶级投票问题**

如果你想亲自尝试一下 Visual Studio 2022，现在可以从这里[下载预览版 2](https://devblogs.microsoft.com/visualstudio/visual-studio-2022-preview-2-is-out/) 。如果你不想使用潜在的不稳定软件，你可以将它与 Visual Studio 2019 一起使用。