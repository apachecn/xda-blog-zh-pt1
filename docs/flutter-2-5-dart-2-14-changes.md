# Flutter 2.5 发布了全屏 Android 应用程序和您支持的材料

> 原文：<https://www.xda-developers.com/flutter-2-5-dart-2-14-changes/>

如果您对跨平台开发感兴趣，那么您可能听说过 Flutter。使用 Dart 语言，Flutter 是一个跨平台的 UI 框架，旨在尽可能简化从 iOS 到 web 的任何东西的开发。昨天，谷歌宣布发布 Flutter 2.5 和 Dart 2.14，其中有很多新内容。

这篇文章仅仅是回顾一下 Flutter 和 Dart 的一些变化。更多详情，请查看最后的链接。

* * *

## 颤动 2.5

### Android 中的全屏

Flutter 2.5 的一大变化是对运行在 Android 上的应用程序提供了更好的全屏支持。此次更新带来了以下新的沉浸式模式:

*   向后倾斜:轻按屏幕上的任意位置以显示系统覆盖图。
*   沉浸式:在屏幕边缘滑动以显示系统覆盖图。
*   沉浸式粘性:类似于沉浸式，但允许框架处理滑动。
*   窄边框:显示半透明系统覆盖层后面的应用程序元素。

 <picture>![Full screen app support for Flutter 2.5](img/49778045b305914a74fcdc68b097d07c.png)</picture> 

New Android edge-to-edge mode: normal mode (left), Edge to Edge mode (center), Edge to Edge with a custom SystemUIOverlayStyle (right). Source: Google.

更多细节，请查看 [Flutter GitHub 库](https://github.com/flutter/flutter/pull/81303)上的 pull 请求。

### 物质的你

Material You 是 Google 最新版本的材质设计。也被称为材质 v3，它是材质设计语言的一个相当大的改进。有新的形状，主题，甚至动态颜色效果。

Flutter 2.5 引入了一些你支持的材质选项，包括新的 FAB 尺寸和更多的主题选项。这还不是一个完整的实现，但它表明谷歌正在取得进展。

 <picture>![Material You FAB sizes in Flutter 2.5](img/e2977b4eb21554b8f7e75e082d784e02.png)</picture> 

New Material You FAB sizes. Source: Google.

* * *

## IDE Plugins

除了 Flutter 2.5，IntelliJ/Android Studio 和 Visual Studio 代码的 ide 插件也在更新。

### IntelliJ/Android Studio

新的 IntelliJ/Android Studio plugin for Flutter 允许开发人员对整个项目进行集成测试。这些测试在它们自己的目录中定义，并在设备上运行。您现在还可以为单元和集成测试生成覆盖率报告。

最后，当从 pub.dev 获取 TrueType 字体时，还有一个小的附加功能可以让您在 IDE 中预览这些字体图标。您必须告诉 IDE 您正在使用哪个包，它只对静态常量有效，但这绝对是一个很好的功能。

### Visual Studio 代码

随着对 Flutter 的 Visual Studio 代码插件的更新，添加了两个新命令，使安装 Dart 和 Dart Dev 依赖项变得更加容易。现在还有一个 Fix All 命令，用于自动格式化和修复当前文件中的 lint 问题。

最重要的是，预览版中有一个新的 Dart 和 Flutter 代码测试运行器，可以在这个版本中启用。这位新的赛跑运动员最终将取代现在的运动员。

## 鸽子

Pigeon 是一个为 Flutter 开发的代码生成工具，帮助开发者在 Flutter 和原生平台之间进行代码桥接。Pigeon 使用一种特殊的接口描述符语法来自动生成 Flutter、Java 和 Objective-C 存根。它甚至是类型安全和空安全的。

Pigeon 1.0 为稳定通道带来了基本的功能，同时支持更好的错误消息、泛型、原语和多参数。

* * *

## Dart 2.14

虽然 Flutter 本身有很多新功能，但其底层语言 Dart 也有一些变化。

### 苹果硅

Dart 2.14.1 对苹果硅片的支持更好。Apple Silicon 的 Dart SDK 现在已经稳定，iOS 模拟器可以在 ARM64 上运行。不幸的是，Flutter SDK 中包含的 Dart SDK 还不支持 Apple Silicon。

### 皮棉状况

自从最初创建以来，Dart 经历了许多变化，包括语法和围绕该语法的样式约定。由于这些变化，旧的风格指南仍然存在，对于如何正确地格式化 Dart 和 Flutter 代码有一些困惑。

Dart 2.14.1 和 Flutter 2.5 现在有一组针对 lint 的条件，这些条件是默认应用的。

* * *

## 结论

在 Flutter 2.5 和 Dart 2.14 中有更多的新特性。从错误修复到新特性，这篇文章肯定没有涵盖所有内容。请务必查看谷歌在 [Flutter 2.5](https://medium.com/flutter/whats-new-in-flutter-2-5-6f080c3f3dc) 和 [Dart 2.14](https://medium.com/flutter/whats-new-in-flutter-2-5-6f080c3f3dc) 上的博客帖子，了解所有新内容。