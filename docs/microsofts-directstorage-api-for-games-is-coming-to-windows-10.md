# 微软面向游戏的 DirectStorage API 即将登陆 Windows 10

> 原文：<https://www.xda-developers.com/microsofts-directstorage-api-for-games-is-coming-to-windows-10/>

在上个月的 Windows 11 发布会上，微软宣布新操作系统将采用新的 DirectStorage API。这种新的 API 改变了游戏从 NVMe 固态硬盘读取数据的方式，实现了更快的速度和更短的加载时间。然而，看起来 DirectStorage 也将进入 Windows 10，特别是 1909 和更高版本。该声明是在该 API 的[首个开发者预览版](https://devblogs.microsoft.com/directx/directstorage-developer-preview-now-available/)发布的同时发布的。

让我们倒回去一点。DirectStorage 在 Xbox 系列 X 和 S 控制台上首次亮相，成为 Xbox Velocity 架构的主干。微软很快宣布 Windows PCs 将会推出 Windows 10。然而，当微软宣布 Windows 11 的功能时，Windows 10 用户似乎可能不会获得 DirectStorage。现在看来，情况不会是这样，但体验可能不完全一样。

我们知道 DirectStorage 有两个核心优势。首先，它允许同时处理多个 IO 请求。这在最近几年变得越来越重要，因为现在的游戏比过去大得多。这也很重要，因为 NVMe 驱动器有更多的带宽，数以千计的数据访问请求会产生开销。同时处理多个请求时，可以使用 NVMe 驱动器的全部带宽。另一个很大的好处是，GPU 可以处理游戏数据的解压缩，以加快进程甚至更多。

然而，微软现在提到了另外一件事。Windows 11 拥有全新升级的存储堆栈，允许 PC 充分利用 DirectStorage。在 Windows 10 上，该公司针对 DirectStorage 优化了传统存储堆栈，但这并不完全相同。然而，微软没有说明这种差异应该有多大。

游戏将不得不专门为 DirectStorage 开发，但它们将继续在不支持 API 的电脑上运行，所以你不必担心兼容性。但是，您需要 NVMe 固态硬盘才能使用 DirectStorage。对于开发者来说。该 API 只需在游戏引擎中实现一次，它的好处将自动应用于整个游戏。虽然现在第一个预览版已经出来了，但 GPU 解压缩功能还不可用。