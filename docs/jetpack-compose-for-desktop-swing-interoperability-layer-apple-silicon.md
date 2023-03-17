# Jetpack Compose for Desktop 增加了 Swing 层和 Apple Silicon 支持

> 原文：<https://www.xda-developers.com/jetpack-compose-for-desktop-swing-interoperability-layer-apple-silicon/>

如果您从事任何类型的开发工作，您可能听说过 JetBrains。他们是庞大的 ide 套件背后的公司，包括 IntelliJ(Android Studio 的基础)、CLion、PhpStorm 和许多其他产品。他们也是制作广受欢迎的跨平台编程语言 [Kotlin](https://www.xda-developers.com/tag/kotlin/) 的人。

JetBrains 又回来了。一年多前，谷歌推出了一个新的 Android 布局引擎，名为 Jetpack Compose。自那以后，它经历了相当多的重大变化，但它已经成为 Android 经典 XML 布局的一个有竞争力的(尽管仍然有些不稳定)替代方案。

Jetpack Compose 和 JetBrains 有什么关系？首先，它是用科特林语写的。但是，JetBrains 也一直在默默努力将 Compose 移植到桌面领域。它已经作为早期开发者预览版公开，现在 JetBrains 准备正式宣布它的存在。

## 什么是 Jetpack Compose？

我在介绍中谈了一点，但我认为它值得更多的解释。如果你以前在 Android 上开发过，你可能已经习惯了布局的工作方式。首先，在 XML 文件中设计布局，然后从 Java 或 Kotlin 与布局进行交互。虽然它是功能性的，但有点过时，而且跨语言的布局可能很难管理。

作为替代方案，Google 开始开发 Jetpack Compose。Compose 是基于 Kotlin 构建的 Android 布局引擎。所有的布局和逻辑代码都在一个地方，这使得交互更加容易。它也是声明性的，而不是 XML 布局的命令式风格。

从命令式引擎转移到声明式布局引擎可能需要一些时间来适应，但是 Compose 无疑是对 XML 的改进，尽管它仍处于早期阶段。

## 桌面版 Jetpack 合成

因此，对于原生 Android 应用程序，Compose 是一个不错的布局选择。但它(通常)不是跨平台的。这就是 JetBrains 的用武之地。该公司已经将 Jetpack Compose 移植到桌面领域，支持 Windows、Linux 和 macOS(英特尔和 ARM)。

虽然也有其他的桌面布局引擎，比如 Electron、JavaFX 和 UWP，但是现在有点混乱。有些不是跨平台的，所以它们只能在一个特定的操作系统上工作。其他的在技术上是跨平台的，但是需要大量的工作来分发。尽管如此，其他的工作起来还是很痛苦，比如 JavaFX。

另一方面，Jetpack Compose for Desktop 相对容易使用，支持显示缩放，具有内置样式，并且(几乎)完全跨平台。虽然您还不能从一个操作系统编译所有发行版，但是代码本身是完全可移植的。就像 Android 一样，打包的应用程序是基于 Java 的，尽管用户不需要安装 JDK 来使用它。

### 交叉兼容性

由于 Compose for Desktop 仍然是新产品，它缺少一些功能。为了帮助开发人员解决这些限制，Compose for Desktop 可以与两个更流行的 Java 布局引擎 JavaFX 和 Swing 进行互操作。如果您有一个在这些引擎中的一个(或两个)开发的桌面应用程序，您可以开始转换到 Compose，同时保持您当前的代码库。

### 安卓+桌面

如果你想把你的 Android 应用程序放到桌面上呢？嗯，你也可以这样做。您的应用程序的 UI 元素可以在 Android 和桌面之间轻松共享。您将无法共享所有内容，但这无疑会使开发变得更加容易。

### 苹果硅支架

上面提到了这个，但是我还打算再提一次。新的苹果硅 MAC 电脑非常惊人，但处理器基于 ARM CPU 架构，这意味着许多 macOS 应用程序目前正在通过 Rosetta 2 x86 translator 运行。虽然苹果在翻译方面做得很好，但原生 ARM 程序仍会运行得更好。

Jetpack Compose for Desktop 原生支持苹果芯片。这意味着你不必担心翻译带来的性能下降，也不必担心苹果停止翻译后的未来支持。

## 功能

因此，JetBrains 为桌面开发了一个新的布局引擎，这很好，但是谁能说它比我们现在拥有的更好呢？

我。

在撰写本文时，我使用了最新的可用版本(0.2.0-build132)为 SystemUI Tuner 制作了一个简单的权限授予程序。因为我不太熟悉组合和声明式设计，所以对我来说，这比 XML 布局应用程序更难，但是我做到了。而且比 JavaFX 好用很多。

虽然主题支持(即黑暗模式)仍然有点不确定，但建立一个交互式布局很容易，除了在调整窗口大小时有一些闪烁外，一切都很好。

如果你想看看这个应用，源代码可以在 [GitHub](https://github.com/zacharee/SUITGranter) 找到。只要用 IntelliJ 或 Android Studio 导入它，它就应该可以运行了。

* * *

就个人而言，我对 Jetpack Compose for Desktop 感到非常兴奋。我以前甚至不知道它的存在，但它已经是我选择的桌面布局引擎。你可以在桌面网站的 [Jetpack Compose 或 GitHub](https://www.jetbrains.com/lp/compose/) 的[上了解更多信息。](https://github.com/JetBrains/compose-jb)

你怎么想？是否值得检验甚至使用它来代替其他可用的框架？让我知道！

*特色图片致谢:[GitHub](https://github.com/JetBrains/compose-jb/blob/master/artwork/readme/apps.png)上的 JetBrains*