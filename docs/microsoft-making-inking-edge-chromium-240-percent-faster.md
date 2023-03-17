# 微软正在改进 Edge 和 Chromium 的墨迹

> 原文：<https://www.xda-developers.com/microsoft-making-inking-edge-chromium-240-percent-faster/>

微软正在对 Edge 中的墨迹处理方式进行一些重大改进，这要归功于新的墨迹 API 和 T2 Windows 11 中的新 API。该公司在 Build 2021 上首次宣布了这些改进，但现在，他们可以为运行 Edge Dev 的用户提供尝试。随着这些变化，微软表示，使用 Windows 11 时，延迟提高了 240%。

首先，新的 Ink API 是 web 开发人员的顶级 API，他们可以实现它来支持墨迹书写。这也已经在 Chromium 项目的上游实现了，所以其他基于 Chromium 的浏览器也可以从中受益。Ink API 只需要两个步骤:从浏览器获取 InkPresenter 对象，并通知 InkPresenter 对象来自设备的最后一个指针事件。在第一步中，新的 Ink API 使 web 应用程序调用操作系统支持的渲染实例或本地浏览器支持的 polyfill 实例。

这就是 Windows 11 发挥作用的地方。在 Windows 11 上，微软 Edge 将能够使用一种新的 API，允许网络应用程序直接与操作系统的合成器接口来绘制墨水。这意味着指针事件不必通过浏览器进程本身，消除了一些通常在 web 上输入时增加的延迟。这就是上面提到的操作系统支持的渲染实例。

在没有此 API 的操作系统上，如 Windows 10 和 Linux，Ink API 将使用直接在浏览器中实现的 polyfill 实例。这将允许 Edge 基于最新的指针信息提供墨迹笔划的预测性呈现。这不如 Windows 11 中的实现响应快，但应该比当前的 ink 实现好得多。

这种新的 Ink API 及其优势现在应该可以在 Dev 频道和 Canary 频道的最新版本 Edge 中获得。由于这一改变已经在 Chromium 中实现，其他使用最新 Chromium 代码的浏览器也应该包含并默认启用这一特性。如果你有兴趣了解更多关于 API 的知识，你可以访问 GitHub 上的规范草案[。](https://wicg.github.io/ink-enhancement/)