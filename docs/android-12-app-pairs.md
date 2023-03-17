# Android 12 的隐藏应用配对功能并不完整，但显示了前景

> 原文：<https://www.xda-developers.com/android-12-app-pairs/>

如果你错过了上周铺天盖地的新闻，谷歌发布了 Android 12 的第一个开发者预览[，我们对迄今为止发现的所有变化感到非常兴奋。我们在](https://www.xda-developers.com/android-12/)发布前听说的[变化之一是一个叫做应用配对的特性。通过我们自己对 Android 12 开发者预览版 1 的源代码和代码分析，我们可以确认该功能确实正在开发中。我们甚至设法在它未完成的状态下摆弄它。](https://www.xda-developers.com/android-12-picture-in-picture-mode-bubbles-changes/)

作为背景，App Pairs 是 Android 12 开发中的一项新功能，可以让你创建一对应用程序，同时在分屏视图中启动。然后，这对应用程序作为一个任务而不是两个任务，这样在进入最近的应用程序概览后，可以很容易地在分屏视图中重新启动这两个应用程序。你会在三星的 Android 软件中发现类似的功能(它在 Galaxy Note 8 上首次亮相[，在微软的双屏 Surface Duo 上首次亮相](https://www.xda-developers.com/galaxy-note-8-software-spen-apps/)[，](https://www.xda-developers.com/microsoft-surface-duo-review/)，但谷歌版本的软件应该可以在所有运行 Android 12 的设备上使用，前提是它能进入稳定版本。

使用一个隐藏的 shell 命令，我们尝试了一下 App Pairs 特性，但是在它可以使用之前还有很长的路要走。首先，虽然这两个应用程序被视为一个单一的任务，但它们实际上并没有在最近的应用程序概述中组合在一起。目前还没有办法(据我们所知)创建一个主屏幕快捷方式来启动应用对，但奇怪的是，启动应用对中的两个应用中的任何一个实际上都将重新启动应用对。

虽然开发商弗朗西斯科·巴罗佐(Francisco Barroso)的“分屏启动器”等第三方替代品目前提供了一个出色的 UI，但它们依赖于 [Android 的内置 API](https://www.xda-developers.com/everything-devs-need-to-know-about-multiwindow-in-android-n-code-examples/)来逐个手动启动分屏模式下的活动。此外，这些应用程序没有组合在一起，因此它们仍然被视为两个独立的任务。这意味着应用程序对不仅启动有点慢，而且如果要重新启动，还需要刷新活动。谷歌为所有 Android 12 设备制作的第一方实现肯定会受到欢迎。

作为比较，这里有一个视频，显示了我的设备启动由“分屏启动器”应用程序创建的应用程序对:

这里有一个视频显示我的设备启动了由 Android 12 的应用对功能创建的应用对:

## 如何在 Android 12 开发者预览版 1 中制作应用配对

如果你想尝试自己创建一个应用程序对，你需要用[下载](https://www.xda-developers.com/how-to-download-android-12/)和[，然后安装](https://www.xda-developers.com/how-to-install-android-12/)第一个 Android 12 开发者预览版。然后，在 PC 的终端或命令提示符下输入 ADB shell，并运行以下 shell 命令:

```
 dumpsys activity service SystemUIService WMShell pair {taskId1} {taskId2} 
```

其中{taskId1}和{taskId2}是您要分组的两个应用的任务 Id。您可以从“dumpsys activity”的输出中找到 taskIds。运行这个命令后，它将为应用程序对创建一个新任务。如果您想要解除这些应用程序的配对，您可以运行以下命令:

```
 dumpsys activity service SystemUIService WMShell unpair {taskId} 
```

特色图片只是一个模型，并不代表 Android 12 中的应用程序对。