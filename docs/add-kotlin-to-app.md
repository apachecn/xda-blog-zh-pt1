# 如何将 Kotlin 添加到现有的 Java Android 项目中

> 原文：<https://www.xda-developers.com/add-kotlin-to-app/>

科特林很棒。它有一大堆有用的语言特性，语法通常简洁明了。它也是跨平台的，基础语言可以编译成一大堆不同的语言和平台。

Kotlin for Java(称为 KotlinJVM)编译的东西与 Java 编译的东西是一样的——JVM 字节码用于纯 Java，以及 Android 目前用于其 Java 版本的任何东西。这意味着用 KotlinJVM 编写的代码可以访问所有现有的 Java 和 Android APIs，以及应用程序中已经存在的任何 Java 类、方法和字段。

这种兼容性也反过来起作用。也就是说，您可以从 Java 访问 Kotlin APIs。如果您尝试使用更高级的特性，代码可能看起来有点乱，但这是可能的。

本教程将介绍如何将 Kotlin 添加到现有的 Android 项目中。它还假设您使用的是 Android Studio。不过，在我们开始之前，如果您还没有熟悉 Kotlin 的工作方式，您可能想先熟悉一下。JetBrains，这种语言背后的公司，[有一个方便的常见问题解答。](https://kotlinlang.org/docs/faq.html)

## 属国

科特林严格来说是个图书馆。这是一个别致的库，有许多功能和一个附带的 IntelliJ/Android Studio 插件，但它是一个库。因此，要添加它，您需要添加一些依赖项。

在您的**项目级别** build.gradle 中，添加 Kotlin 依赖项。

```
 buildscript {
    ...
    dependencies {
        ...

        classpath "org.jetbrains.kotlin:kotlin-gradle-plugin:1.5.10"
    }
    ...
} 
```

在你的**模块级** build.gradle 中，应用 Kotlin Android 插件并添加依赖项。

```
 ...

apply plugin: 'kotlin-android'

...

dependencies {
    ...

    implementation 'androidx.core:core-ktx:1.5.0'
    implementation 'org.jetbrains.kotlin:kotlin-stdlib:1.5.10'
} 
```

这就是 Kotlin 的实现。最新版本的 Android Studio 已经捆绑了 IDE 插件。

## 基本用法

现在集成完成了，你可以开始使用 Kotlin 了。要创建一个新类，只需右键单击要创建文件的包，单击 *New* ，然后单击 *Kotlin Class/File* 。

一旦你点击它，你会看到一个对话框，询问文件名，以及它应该是什么类型的对象(类，接口，对象，普通文件等)。这非常类似于创建一个新的 Java 类。

选择你想要的，文件就会被创建。现在你可以开始用 Kotlin 编程了。

## 结论

将 Kotlin 添加到现有的 Java Android 项目很容易。只要包含一些 Gradle 依赖项，应用一个插件，就可以开始用这种语言编程了。

关于更高级的用法，包括如何自动将 Java 代码转换成 Kotlin，请查看 [Google 的官方文档](https://developer.android.com/kotlin/add-kotlin)。