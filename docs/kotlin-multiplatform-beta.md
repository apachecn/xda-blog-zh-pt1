# Kotlin 多平台进入跨平台开发测试阶段

> 原文：<https://www.xda-developers.com/kotlin-multiplatform-beta/>

如果你曾经接触过 Android 开发，你可能听说过 Kotlin。这是一种由 JetBrains 设计的语言，可以与 Java 完全互操作。你可以在其中为 Android、web 和 iOS 构建应用程序，谷歌实际上说它是应用程序开发人员编写应用程序的首选语言。现在 Kotlin 多平台正在进入测试阶段，这将允许开发者从相同的代码库为 Android 和 iOS 构建。

至于有什么变化，JetBrains 没有给我们太多的工作。Kotlin 项目负责人 Roman Elizarov 表示:“在这个测试版中，我们更新了内存管理方法，以在 Android 和 iOS 目标之间提供一致的体验，现在用户可以在重用现有 Kotlin 代码和访问特定于平台的功能之间取得适当的平衡。“测试版仍有剩余部分需要实现，交付它们是我们的首要任务。”

Kotlin 多平台有许多关键优势，其中最大的优势是 Android 和 iOS 之间的统一代码库。这包括网络、数据存储、分析和应用程序中所有其他逻辑的相同代码库。更重要的是，保留了逻辑元素，但在完全访问 Android 和 iOS SDKs 时，您仍然会保留原生代码的流畅性。Android Studio 中甚至已经有了跨平台开发的工具。

“在其他技术抽离或完全取代特定平台应用开发的情况下，Kotlin 多平台是现有特定平台技术的补充，旨在取代与平台无关的业务逻辑。这是工具箱中的一个新工具，而不是取代工具箱”，网飞的 David Henry & Mel Yahya 说。

有几个[示例项目](https://kotlinlang.org/docs/multiplatform-mobile-samples.html)你可以看一看，以获得如何将 Kotlin 多平台集成到你的项目中的灵感，从而在同时为 Android 和 iOS 创建时使开发更容易。看起来这个测试版主要是对稳定性的改进，但是我们期待着在 Kotlin 多平台的整个生命周期中出现更多的变化。