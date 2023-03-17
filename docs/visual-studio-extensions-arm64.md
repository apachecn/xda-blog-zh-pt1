# Visual Studio 扩展现在可以支持 Arm64 设备

> 原文：<https://www.xda-developers.com/visual-studio-extensions-arm64/>

微软正在大力扩展对基于 Arm64 的设备的支持，今天该公司宣布，您现在可以构建支持 Arm64 的 Visual Studio 扩展。今年早些时候，微软[宣布打算提供一个完全兼容 Arm64 的开发者工具链](https://www.xda-developers.com/microsoft-is-finally-taking-windows-on-arm-development-seriously/)，包括一个 Arm 版本的 Visual Studio，目前在 17.4 版本中提供预览版。还有 Project Volterra，一个我们知之甚少的基于 Arm 的开发机器。

现在，除了为 Arm64 处理器(如高通骁龙 8cx Gen 3)构建 Visual Studio 本身之外，微软还让开发人员有可能构建自己的 Visual Studio 扩展，这些扩展也是该架构的原生部分。当创建或更新扩展时，开发人员需要将正确的 ProductArchitecture 标记添加到 VSIX 清单中，以针对 Visual Studio 的 Arm64 版本，然后在构建包时将 Arm64 作为平台目标。您需要最新版本的 VS SDK 构建工具来完成这项工作，并且您可能还需要对现有的扩展进行一些更改，这取决于它们当前的构建方式。

您还可以将 Arm64 版本的扩展发布到 Visual Studio Marketplace，即使您已经有了一个针对 AMD64 的版本，您也可以在同一列表中添加 Arm64 版本，这样用户就可以轻松地下载适合他们机器的版本。对于已经有 AMD64 和 Arm64 的单独列表的扩展，微软正在努力将列表合并为一个。

微软已经确认，Visual Studio 2022 17.4 将是第一个正式支持 Arm64 的版本，它应该会在 11 月的某个时候推出。微软的路线图表明，新的小更新应该每三个月进行一次，【17.3 版本于 8 月初发布。这应该给开发者时间在 Arm64 正式发布之前更新他们的扩展。现在，如果你很好奇， [Visual Studio 17.4 预览版 2.1](https://visualstudio.microsoft.com/vs/preview/) 于本周早些时候发布，供那些想尝试一下的人使用。

* * *

**来源:** [微软](https://devblogs.microsoft.com/visualstudio/now-introducing-arm64-support-for-vs-extensions/)