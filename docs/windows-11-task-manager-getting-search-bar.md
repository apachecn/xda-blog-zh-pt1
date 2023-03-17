# 微软正在为 Windows 11 中的任务管理器开发搜索栏

> 原文：<https://www.xda-developers.com/windows-11-task-manager-getting-search-bar/>

随着 [Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2/) 的推出， [Windows 11](https://www.xda-developers.com/windows-11/) 中的任务管理器最近进行了多年来的首次重大重新设计，看起来微软正准备在未来提供更多重大改进。正如 *DeskModder* 最初发现的那样，开发频道中最新版本的 Windows 11——即版本 25231——在任务管理器中添加了一个搜索栏，让你更容易找到你可能正在寻找的程序。以前，您必须滚动浏览一个很长的程序列表来找到一个特定的进程，这可能会变得很乏味。

目前，这项功能实际上并不打算让公众访问，这就是为什么微软没有提到它。然而，它隐藏在一个可以使用 ViveTool 等工具启用的功能 ID 下。你只需要在命令行或者 Windows PowerShell 中运行 ViveTool，输入**vive tool/enable/id:39420424**(在 PowerShell 中，应该写成**。\ vive tool/enable/id:39420424)**，该功能将被启用，不过您可能需要重新启动电脑才能看到它。如果你不喜欢使用基于文本的工具。你也可以看看 [ViveTool GUI](https://www.xda-developers.com/vivetool-gui-enable-hidden-windows-11-features/) ，我们之前已经介绍过了。您可以搜索功能 ID **39420424** 并在那里启用它，这对于一些用户来说可能更容易。

当然，这个特性还没有完全可用是有原因的。目前看来，似乎只能通过搜索可执行文件的确切名称来找到程序或进程，而不是更容易理解的名称。例如，你不能搜索 *Windows 资源管理器*如果你想重启那个进程，你需要搜索【explorer.exe】T2。搜索栏文本表明您可以搜索进程名称、PID，甚至是发布者，这将使您更容易找到您想要的东西——我们只需要等待该功能真正发挥作用。

开发频道中的 Windows 11 版本主要是测试较小的更新，预计将通过功能下降来交付，内部称为“瞬间”更新。这些只是简单的累积更新，但是它们可以启用某些功能，第一个也是最近的一个例子是在文件资源管理器中添加标签。这个任务管理器搜索栏很有可能在未来的某个时候通过这些更新之一进入 Windows 11 版本 22H2。

* * *

**来源:**[desk moder](https://www.deskmodder.de/blog/2022/11/01/windows-11-microsoft-testet-derzeit-eine-suchleiste-im-task-manager)