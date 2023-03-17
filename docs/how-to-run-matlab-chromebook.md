# 如何以两种简单的方式在 Chromebook 上运行 MATLAB

> 原文：<https://www.xda-developers.com/how-to-run-matlab-chromebook/>

人们普遍认为 Chromebooks 无法运行 PC 或 MAC 上的强大软件。如果你是一名工科学生，你可能需要在你的笔记本电脑上运行一些相当密集的应用程序。Chromebooks 是学生的绝佳解决方案，因为它们既安全又经济实惠。

如果你是一名使用 Chromebook 的工科学生，你可能需要运行 MATLAB 来完成一些课程作业。与 Mac 和 PC 不同，MATLAB 不提供原生 ChromeOS 安装。幸运的是，仍然有一些简单的方法可以在 Chromebook 或其他 ChromeOS 设备上利用 MATLAB 的计算能力。我们将看看 MATLAB 的在线版本，并演示如何使用 Linux 应用程序在 Chromebook 上安装完整版本的 MATLAB。

## 使用浏览器在 Chromebook 上运行 MATLAB

如果您只需要 MATLAB 来完成非常基本的任务，比如微积分入门或线性代数课程，那么您最好的选择是在浏览器中运行 MATLAB。MATLAB 为云计算提供了一个强大的在线平台。要使用 MATLAB online，您只需登录您的[大学或组织](https://www.xda-developers.com/best-business-chromebooks/) Mathworks 帐户，并选择 online 选项。如果你已经登录了你的 Mathworks 账户，你可以在 matlab.mathworks.com 的[直接访问这个在线平台。](http://matlab.mathworks.com)

使用 MATLAB online 的主要缺点是，你必须将文件存储在 Mathworks 分配给你的云服务器中。在 ChromeOS 上使用云存储是相当自然的，但遗憾的是你不能将你的 Google Drive 或 Dropbox 链接到你的 MATLAB drive。如果您使用的是大学或专业机构的当前许可证，MATLAB 驱动器的存储空间限制为 5GB。

有时候你需要存储大的矩阵，这样会很快耗尽 GBs。另外，图形也占据了相当大的空间。如果你在学术界或工业界进行严肃的研究，你可能需要一个在云中运行的替代方案。

尽管如此，对于在作业中使用 MATLAB 的学生来说，这应该可以完成任务。你可以随时选择在 MATLAB 的云存储和你自己的 Google Drive 或 Dropbox 文件夹之间来回移动文件。显然，这并不理想，但在必要时可以完成工作。如果你有一台 [LTE Chromebook](https://www.xda-developers.com/best-chromebooks-lte-5g/) ，确保关闭 MATLAB 驱动的自动同步。

## 使用 Linux 应用程序在 Chromebook 上运行 MATLAB

对于那些无法使用在线解决方案的人来说，还有另一个方便的选择。现代 Chromebooks 现在支持 Linux 应用程序。有了 Linux 支持，就可以安装 MATLAB 的 Linux 版本了。要尝试这样做，您需要对终端有一些基本的了解。那些需要快速复习 ChromeOS 上的 Linux 的人可以查看我们的 Chromebooks 上的 Linux 应用的完整指南。

如果你选择在 Chromebook 上通过 Linux 安装 MATLAB，我们强烈建议你安装一个旧版本的 MATLAB。多年来，MATLAB 的功能越来越多。

旧版本的 MATLAB 在 ChromeOS 上的 Linux 容器中运行起来更流畅。此外，一些较新版本的 MATLAB 与某些 Chromebooks 存在一些图形加速不兼容问题。在 Chromebook 上安装旧版本的 MATLAB 不会有太大损失。MATLAB 的核心特性集已经好几年没变了。你将失去一些图形和工具箱的高级升级。然而，对于核心科学计算和测试，2016b 对我来说很好。我们来谈谈如何在你的 Chromebook 上实际安装 MATLAB。

### 从 Mathworks 下载

第一步是从 Mathworks 下载你想要的 MATLAB 版本。为此，您需要与您的大学或公司电子邮件地址相关联的 Mathworks 登录信息。前往 Mathworks 网站上的*下载*部分，选择您想要安装的版本。同样，我使用的是 2016b，但我们认为 2019 年之前的任何东西在 Chromebook 上都可以。确保选择 Linux 下载，并将文件下载到 Chromebook 上的 *Linux apps* 文件夹。

### 解压下载文件

接下来，您需要打开一个终端窗口来解压缩安装包。如果你还没有启用 Linux 应用程序，你需要去[阅读我们的教程，并做第一个](https://www.xda-developers.com/linux-apps-chrome-os/)。要解压缩文件，请键入以下命令:

```
 unzip matlab_R2016b_glna64.zip 
```

在这里，将“matlab_R2016b_glna64.zip”替换为您下载的安装包的名称。这个过程需要很短的时间，你会看到几个文件名向下滚动终端窗口。当这个过程完成时，你会在命令行上再次看到 username@penguin。

### 启动 MATLAB 安装程序

我们准备启动 MATLAB 安装程序。为此，请运行以下命令:

```
 xhost + 
```

后面跟着命令:

```
 sudo ./install 
```

这将在终端窗口之外启动 MATLAB 安装窗口。现在，您需要使用您的 Mathworks 帐户登录并验证相关的许可证，以下载并安装 MATLAB。安装程序将询问您希望使用哪个文件夹进行安装。我建议使用建议的默认文件夹。您可能会收到一个弹出窗口，提示您可能在所需的文件夹中没有足够的空间。

只要你验证你的 Chromebook 上有足够的存储空间，你就可以忽略这个警告，点击 *Yes* 。

### 选择软件包并完成安装

安装的最后一步是选择您希望安装的软件包。如果你只想要基本的 MATLAB，你可以取消所有的选项，只选择第一个复选框。

如果你的大学或组织支付了可选工具箱的费用，那么很可能值得下载所有的工具箱。工具箱是难以置信的昂贵，如果你以后想要的话，比如在离开学校之后。安装将需要一段时间，因为下载的文件可能会很大。如果您选择所有工具箱，您将看到 6-10 GB 的下载大小，这取决于 MATLAB 的版本。

安装完成后，MATLAB 将通过连接到 Mathworks 服务器来验证您的许可证。验证之后，您可以从命令行使用以下简单命令启动 MATLAB:

`matlab`

一切就绪，这就是在 Chromebook 或其他 ChromeOS 设备上安装 MATLAB 的整个过程。对于那些不需要本地安装的人来说，如果你不需要存储太多文件，在线体验也会很好。请在下面的评论部分告诉我们您对每种方法的体验。