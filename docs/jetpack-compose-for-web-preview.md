# Jetpack Compose for Web 是一个新的用于 Web 开发的 UI 框架

> 原文：<https://www.xda-developers.com/jetpack-compose-for-web-preview/>

在过去的几年里，跨平台程序开发得到了相当大的推动。React 和 Flutter 等框架的创建是为了让开发者在 Android、iOS、桌面甚至网络上共享单一代码库。甚至 JetBrains，一些最流行的 ide 和 Kotlin 编程语言背后的公司，也一直致力于跨平台开发。首先是 Kotlin 多平台，但最近是 Jetpack Compose。

不久前，JetBrains 将 Jetpack Compose 移植到桌面上，Jetpack Compose 是谷歌为 Android 开发的声明式设计框架。这允许基于 Java 的 JVM 的跨平台桌面开发。使用 Jetpack Compose，您可以从一个代码库制作一个适用于 Android、macOS、Windows 甚至 Linux 的应用程序。但除了 iOS，Compose 还缺少一个相当大的平台:网络。

不过，这种情况即将改变。JetBrains 发布了他们所谓的 Jetpack Compose for Web 的技术预览。

现在，技术预览基本上是一个前阿尔法花哨的名字。Compose for Web 还远未准备好用于生产。没有教程，只有很少的文档，API 也远未完成。也就是说，让我们看看 Compose for Web 目前提供了什么。

在当前版本中，有两种方式可以在 Compose for Web 中进行开发:使用 DOM API，或者使用现有的 Compose 小部件，比如 Column 或 Text。

如果您使用 DOM API，您将拥有代表不同 HTML 元素的 API 名称，例如 **p** 、 **a** 等等。不过，Compose 和经典 Kotlin JS 的最大区别在于，您可以使用基于状态的声明式设计。这个选项似乎有点像传统 web 开发和完全声明式 UI 开发之间的桥梁。除了创建布局，Compose for Web 还允许您创建动态的、基于状态的样式表。

第二个选项是 Android 和 Compose 开发人员更熟悉的内容。有一些预制的组件，比如列、行和滑块，可以用来构建 web UI。现在，这些还不是很完整，样式和选项也没有完全实现。但它至少让我们了解了 JetBrains 为 Web Compose 准备了什么。

总的来说，目前并没有太多的东西可以为 Web 创作。它仍然处于非常早期的阶段。但这对未来意义重大。就个人而言，作为一名 Android 开发者，我很难进入基于浏览器的布局框架。基本的 HTML 和 CSS 可能很笨拙，React 和 Flutter 语法仍然基于 HTML 设计。

一种不是基于 web 设计原则的全功能、跨平台的设计语言是非常令人兴奋的。虽然 Jetpack Compose 还有很长的路要走，但 JetBrains 的计划对 UI 设计的未来可能意味着很多。

如果你想了解更多关于 Compose for Web 的信息，请查看 JetBrains 的公告。如果你对当前的实现感兴趣，[可以去 GitHub 库](https://github.com/JetBrains/compose-jb/tree/master/tutorials/Web)。