# Google 发布带有稳定 API 的 Jetpack Compose beta

> 原文：<https://www.xda-developers.com/jetpack-compose-beta-released/>

我们又来了。我写了关于 Jetpack Compose 的文章，这是谷歌的新 UI 引擎，当它进入 [alpha](https://www.xda-developers.com/jetpack-compose-google-ui-toolkit-android-alpha/) 的时候，以及当 JetBrains [将它移植到桌面平台](https://www.xda-developers.com/jetpack-compose-for-desktop-swing-interoperability-layer-apple-silicon/)的时候。今天，Jetpack Compose 的测试版已经发布。

如果你不了解现有的所有新的 UI 技术(我不怪你)，也不想通读其他文章(现在我要怪你)，这里有一个快速描述。Jetpack Compose 是一个用 Kotlin 编写的声明式 UI 引擎，旨在取代(或至少成为)传统命令式 UI 引擎，如 Android 的 XML 布局。我不会讨论声明式和命令式布局之间的区别，所以我们只能说 Jetpack Compose 是一个强大的纯代码布局引擎，它可以使 UI 实现更加容易。

这样一来，Compose 的测试版到底意味着什么？让我想想。

## 应用程序接口

每个好的框架都需要一个 API(根据定义)。在 pre-alpha 和 alpha 阶段，Google 努力构建尽可能直观和有用的 Compose API。就像每一个好项目一样，它经历了许多修改。在这些阶段使用 Compose 可能很困难，因为 API 可能会在没有太多警告的情况下被删除或重命名。

现在我们处于测试阶段，谷歌有信心 API 是完整和稳定的。这意味着没有更多(激烈的)删除或更改，所以你可以花更多的时间实际制作你的应用程序，而不是跟上 API 的变化。

当然，稳定的 API 并不意味着一成不变。谷歌仍然会添加功能和改变周围的东西，但现在会有适当的弃用通知和更换周期。

## 协程支持

还记得 Google [弃用 Android 中的 AsyncTask](https://www.xda-developers.com/asynctask-deprecate-android-11/) 时，所有人都很担心，然后就完全忘记了吗？你可能要为此感谢 Kotlin 的协程框架。在其最基本的形式中，它是 AsyncTask 的替代品，但它也更强大、更灵活、更跨平台。

虽然 Jetpack Compose 在某种程度上支持协程的使用，但它主要是作为一个互操作层。不过，在测试版中，协同程序被内置到 Compose 中，所以您可以再次正确地使用异步调用。

## 动画片

在 Android 中构建动画可能有点烦人，有一段时间，它们也在 Compose 中。然而，在测试版中，谷歌承诺一个“易于使用”的动画 API 来使事情变得更容易。他们还更新了 Android Studio，以包括对预览这些动画的支持，所以你不必部署你的应用程序来测试它们。

## 布局

Android Studio 有一些非常好的工具来处理布局。一个是布局预览，可让您大致了解您的布局在设备上的外观，另一个是布局检查器，可让您确切了解应用程序在设备上的布局。

在此之前，布局预览确实可以用于撰写布局，但每次更改内容时，您都必须重新构建应用程序才能更新预览。现在我们处于测试阶段，不过，Android Studio 已经更新，包括您的撰写代码的实时预览。

此外，在此之前，布局检查器基本上不能用于编写布局。它会显示应用程序的截图，但它不能实际提取和显示所有布局组件的线框。就像布局预览一样，Android Studio 已经更新了一个新的布局检查器，支持撰写布局。

## 对讲系统

现在让我们来谈谈可访问性，一个非常重要的特性，不幸的是，它经常被遗忘。幸运的是，谷歌没有忘记，尽管它可以来得更快:Compose layouts 现在支持 [Talkback](https://www.xda-developers.com/google-talkback-screen-reader-galaxy-s21/) ，这是一款 Android 上的高级屏幕阅读器，既可以为你朗读内容，也可以让你使用简单的手势与显示屏进行交互。

虽然这是目前唯一的主要辅助功能，但谷歌承诺，到稳定时，将添加其他辅助功能。我想，迟做总比不做好，希望这些特性与 Compose 的集成比与 XML 的集成更紧密。

* * *

这差不多就是全部了。

如果您想开始使用 Jetpack Compose，现在是一个非常好的时机。您已经有了一个功能完整的 API 来玩和学习，还有大量直接来自 Google 的教程。查看[谷歌的开发者网站](https://developer.android.com/jetpack/compose/tutorial)了解更多关于更新和如何使用 Compose 的信息。

当然，请告诉我们您对 beta 中的变化有何看法，或者您对 Compose 的总体看法。