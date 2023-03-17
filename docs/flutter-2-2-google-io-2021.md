# Flutter 2.2 在 Google I/O 2021 上发布，提供新功能

> 原文：<https://www.xda-developers.com/flutter-2-2-google-io-2021/>

Google I/O 正在发生，这意味着，当然，有一堆新的 Android 开发新闻！如果你正在阅读这篇文章，那么这意味着谷歌刚刚(或者已经)宣布了 Flutter 2.2，这是他们跨平台应用开发框架的新版本。

## Flutter 采用统计

事实上，对于一个点发布来说，有相当多的新东西，但是在我们开始之前，我们应该谈谈统计数据。谷歌对 Flutter 非常自豪，这似乎是有充分理由的。从 *SlashData* 引用的数据来看，Flutter 是现在最流行的跨平台开发框架，有 45%的跨平台开发者选择使用它。

这种受欢迎程度是一些相当大的增长的结果。在 2020 年初至 2021 年初的一年时间里，Flutter 的使用量增长了 47%，Play Store 中超过 12%的应用程序是用 Flutter 编写的。12%可能看起来不多，但 Play Store 有大量的应用程序；其中超过 20 万人在使用 Flutter。

## Flutter 2.2 的语言特点

说完了，让我们来谈谈技术方面。

### 摆动

随着 [Flutter 2.0](https://www.xda-developers.com/flutter-2-0-stable/) 的发布，谷歌引入了声音零安全。空安全允许开发人员直接从代码中指示变量或值是否可以为空。Kotlin 也有同样的特性，我可以根据个人经验告诉你，它使得与空指针相关的错误变得不那么常见。在 Flutter 2.2 中，空安全现在在新项目中默认启用。

除了零安全，在 Flutter 2.2 中还有一些性能改进。[当构建 web](https://www.xda-developers.com/flutter-2-0-web-stable/) 时，您现在可以使用服务人员在后台缓存资源。在 Android 上，你可以使用延迟组件，让你根据需要在运行时下载 Flutter 组件，并减少应用程序的大小。对于 iOS，您可以预编译着色器，使动画在首次运行时更加流畅。最后，DevTools 套件中有一些新工具，可以让你分析应用程序中的内存使用情况，并找到问题所在。

Flutter 2.2 还带来了一些新功能和 SDK。首先，在使网络应用程序更易访问方面已经做了更多的工作。虽然在 2.0 版本中有对可访问性的推动，但它并不完全。SDK 方面，Flutter Ads SDK 更新了内置的 null 安全和自适应广告横幅。最后，还有一个新的支付插件，允许开发者在 iOS 和 Android 上处理实物支付。

### 镖

除了前面提到的所有变化，底层语言 Dart 已经更新到 2.13 版。Dart 的外部函数接口在 2.12 中达到稳定，在 2.13 中，包括对数组和打包结构的支持。Dart 2.13 还增加了类型别名支持。对于自动化爱好者来说，Dart 现在有了官方的 GitHub Actions 支持和官方的 Docker 映像，用于自动化构建和执行。

## 新平台

随着 Flutter 和 Dart 的更改完成，您可能会认为这就是本文的结尾。但事实并非如此。不完全是。谷歌在这次发布中还强调了两件事。

首先是为 Tizen 的[颤振。Tizen 是一个基于 Linux 的开源操作系统，三星将其用于智能设备，包括电视和智能手表(](https://github.com/flutter-tizen/flutter-tizen)[似乎不会太久](https://www.xda-developers.com/galaxy-watch-4-ditch-tizen-customized-wear-os/))。通常，你可以使用 JavaScript、C++或 C#开发应用程序。三星一直在努力为 Flutter SDK 构建一个扩展，让开发者可以构建 Tizen 应用。虽然它仍处于早期测试阶段，但这是一个充满希望的开始，并进一步扩大了 Flutter 的覆盖范围。

第二个是[扑向 UWP](https://flutter.dev/desktop#uwp) 。UWP 代表通用 Windows 平台，是 Windows 10 中(一些)现代风格应用程序的构建基础。UWP 支持带来了为 Windows 开发更多具有本机外观的应用程序的能力。类似于 Tizen 的 Flutter，这是一个 alpha，所以它还没有准备好进入黄金时间。

* * *

对于点释放来说，Flutter 2.2 和 Dart 2.13 有很多变化。有新的语言特性，新的 SDK，甚至新的平台。Flutter 已经越来越受欢迎，这些变化不会减慢它的速度。记得查看谷歌关于 [Flutter 2.2](https://medium.com/flutter/whats-new-in-flutter-2-2-fd00c65e2039) 和 [Dart 2.13](https://medium.com/@mit.mit/announcing-dart-2-13-c6d547b57067) 的帖子，了解更多细节和入门指导。