# 如何在 Windows 10 和 Windows 11 上安装 Windows 包管理器

> 原文：<https://www.xda-developers.com/how-install-windows-package-manager/>

如果你曾经使用过 Linux，也许在 Steam Deck 上使用过，或者在 macOS 上使用过 Homebrew，你可能对包管理器很熟悉。尤其是在 Linux 上，这是大多数用户安装软件的方式，尽管传统的安装程序仍然存在。可以通过命令行访问软件包管理器，从而实现快速、静默的安装和更新。

Windows 以前也有第三方包管理器，比如 Chocolatey，但是微软现在有自己的了。几乎任何使用 Windows 10 或 Windows 11 的人都可以使用 Windows 包管理器。在许多情况下，它通过其清单从网络上下载软件。但它现在也可以与微软商店集成。Windows 包管理器是开源的，它的目录是建立在社区贡献之上的。

Windows 包管理器不一定适合所有人，尤其是如果你主要从微软商店获得你的应用。对于那些花费大量时间在终端、企业部署上的开发人员，或者只是那些从网络上获取软件的人来说，它当然可以改善你的工作流程。以下是如何安装和开始使用它。

## 使用 Windows 包管理器的要求

 <picture>![](img/8e4125268ecf01a9f14467f50a1b1dc7.png)</picture> 

Image: Windows Package Manager (GitHub)

使用 Windows 包管理器的要求如下:

> 目前，客户端需要 Windows 10 1809(内部版本号 17763)或更高版本。不支持 Windows Server 2019，因为 Microsoft Store 不可用，也没有更新的依赖项。可能可以安装在 Windows Server 2022 上，这应该被视为实验性的(不支持)，并且需要手动安装依赖项。

除上述要求外，没有其他特定要求，您可以使用一些不同的方法来访问 Windows 包管理器。

## 如何安装 Windows 包管理器

确保您的电脑上安装了 Windows 软件包管理器的最简单方法是从微软商店获取最新版本的[应用安装程序](https://apps.microsoft.com/store/detail/app-installer/9NBLGGH4NNS1)。这通常用于侧面加载 Windows 应用程序包。但它也包含了 Windows 包管理器所需的内容。

或者，您可以加入 [Windows 软件包管理器内部计划](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR-NSOqDz219PqoOqk5qxQEZUNFkzQVcxMkJXWEFCUkE4WThQWUJMVlA1Ty4u)，或者使用 Windows 内部版本。在这两种情况下，您将获得最新的开发版本，而不需要安装任何其他东西。

只需打开 PowerShell 窗口，输入 **winget** ，然后按 enter 键，就可以检查安装是否正确。如果您看到一个响应，那么您知道您正确地启用了它。

### 使用 Windows 包管理器安装应用

winget 提供的应用程序库非常庞大，安装也很简单。但是你也希望能够找到你要找的东西，有几种方法可以做到这一点。

首先是使用优秀的第三方工具， [winstall.app](https://winstall.app/) 。这是 winget 库的 GUI 前端。它可以让你像浏览其他商店一样浏览和搜索。它还会为你提供安装所需的命令，你可以用一个字符串下载许多不同的应用程序。

或者，您可以使用 **winget search** 命令在 PowerShell 中进行搜索。如本例所示:

```
 winget search chrome 
```

这将返回任何匹配搜索词的 winget 清单。在这种情况下，您将看到类似下图的内容。

一旦您知道自己想要什么，要安装的模板就很简单:

```
 winget install <your-app-here> 
```

Windows 包管理器现在将为您所需的应用程序使用清单。将其从远程位置拉出，并在可能的情况下静默安装。不过，有些仍然会弹出安装框，您必须与之交互，所以值得呆在附近。

* * *

这是 Windows 包管理器最基本的设置和使用情况。如前所述，它并不适合所有人。但是，例如，那些从事开发工作的人，或者那些只想用比微软商店更精简的东西的人，可能会发现它很有用。