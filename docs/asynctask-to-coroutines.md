# 如何用 Kotlin 的协程替换 AsyncTask

> 原文：<https://www.xda-developers.com/asynctask-to-coroutines/>

很长一段时间以来，在 Android 中，如果你在制作应用程序时需要异步地做任何事情，你可能会使用 AsyncTask。AsyncTask 是 Android 框架中的一个 API，它使得在后台运行操作并在完成时返回值变得很容易。这很有道理。与 Kotlin 的协同程序不同，AsyncTask 已经存在了一段时间，而且是内置的。

然而，AsyncTask 的设计理念和实现都已经有些过时了。正因为如此，谷歌[否决了 AsyncTask API](https://www.xda-developers.com/asynctask-deprecate-android-11/) 。如果你愿意，你仍然可以使用它，但谷歌不建议这样做。幸运的是，AsyncTask 有一大堆替代品，包括 Kotlin 语言的一个特性——协程。

Kotlin 的协同程序 API 是一个非常强大的框架，可以让你做很多事情。这篇文章只是触及了可能性的皮毛。我们将讨论从 AsyncTask 迁移到协程所需的基础知识。

## 添加协程支持

在开始使用协程之前，您需要将它们添加到您的项目中。

### 添加 Kotlin 支持

如果您已经实现了 Kotlin，请跳到下一节。否则，您需要在项目中添加 Kotlin 支持。查看我的关于将 Kotlin 添加到现有项目的教程，了解更多细节。

### 添加协程库

在您的模块级 `build.gradle`中，包含以下依赖项。

```
 dependencies {
    ...
    implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-core:1.5.0'
    implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.5.0'
} 
```

同步您的项目，现在就可以使用 Kotlin 的协同程序了。

## 使用协程

### 实现协同作用域

为了使用协程，您需要有一个可用的协程作用域实例。一个简单的方法是在你的包含类中实现它。

例如，要在活动中实现协同作用域:

```
 class SomeActivity : AppCompatActivity, CoroutineScope by MainScope() {
        ...

        override fun onDestroy() {
            super.onDestroy()

           cancel()
        }
} 
```

这将使 SomeActivity 通过 MainScope 类实现 CoroutineScope 接口。MainScope 将处理协程 Scope 的所有实现逻辑，同时允许您使用协程 Scope 方法。在`onDestroy()`中调用`cancel()`确保在活动退出后没有异步逻辑继续运行。

### 用协程替换 AsyncTask

假设您在一个活动中有一个 AsyncTask，它在后台执行一个长时间运行的操作，并最终返回一个字符串。大概如下。

```
 private inner class SomeTask : AsyncTask<Void, Void, String>() {
    override fun doInBackground(vararg params: Void): String {
        try {

            Thread.sleep(10000);
        } catch (e: InterruptedException) {}

        return "SomeString";
    }

    override fun onPostExecute(result: String) {
        val someTextView = findViewById(R.id.some_text_view)
        someTextView.text = result
    }
} 
```

用协程替换它很容易。就用`async()`的方法。Kotlin 的`async()`可以在任何线程上运行，但是它是异步运行的。这意味着您可以更新视图等，而不必担心使用正确的线程。

```
 class SomeActivity : AppCompatActivity(), CoroutineScope by MainScope() {
    ...

    private fun doOperation() {
        async {

            delay(10000)

            val someTextView = findViewById(R.id.some_text_view)
            someTextView.text = "SomeString"
        }
    }
} 
```

如您所见，使用协程比使用 AsyncTask 简单得多。不过，你不必只是调用`async()`并让它做自己的事情。您可以持有对它的引用，甚至等待它完成。

```
 val asyncJob = async {

}

asyncJob.await()

doSomethingElse() 
```

### 使用异步返回值

如果你愿意，你甚至可以从`async()`返回一个值。所以最初的例子可能会变成这样。

```
 class SomeActivity : AppCompatActivity(), CoroutineScope by MainScope() {
    ...
    private fun doOperation() {
        val asyncJob = async {

            delay(10000)

           "SomeString"
        }

        val result = asyncJob.await()

        val someTextView = findViewById(R.id.some_text_view)
        someTextView.text = result
    }
} 
```

### 使用 withContext

为了方便，Kotlin 提供了`withContext()`。这内联了整个`await()`的东西，只是把值返回给你。

```
 class SomeActivity : AppCompatActivity(), CoroutineScope by MainScope() {
    ...
    private fun doOperation() {

        val result = withContext(Dispatchers.Main) {
            delay(10000)

            "SomeResult"
        }

        val someTextView = findViewById(R.id.some_text_view)
        someTextView.text = result
    }
} 
```

## 结论

上面的例子只是 Kotlin 协程的一些基本用法，帮助您入门。您不必将协程局限于活动，甚至任何具有适当生命周期的事物。你可以在任何地方运行它们。还有更高级的操作，比如选择哪个线程应该运行异步逻辑。本指南主要展示如何用一个简单的协程替换一个简单的 AsyncTask。

有关协程如何工作的更多细节，以及如何利用它们更高级的特性，请查看官方 Kotlin 文档。