# 谷歌推出新的 Firebase 功能来简化应用程序开发

> 原文：<https://www.xda-developers.com/firebase-news-google-io-2021/>

Google I/O 今天早些时候开始了，在大开发者主题演讲上，我们得到了许多与 Android 开发相关的新闻。Flutter 有了一些变化，Jetpack 有了一些新特性，如果这篇文章的标题没有给你提示的话，Firebase 也有了一些新的东西。

如果你不知道，Firebase 是谷歌基于云的应用工具套件。它具有从分析收集到在线文件存储的各种功能，如今这一功能列表还在扩展。

## 存储模拟器加入 Firebase 模拟器套件

不久前，Google 向 Firebase 引入了模拟器套件。这个特性允许开发者在 Firebase 中运行一些工具的本地版本。本地版本意味着调试更容易，开发更便宜，甚至可以离线编程。虽然模拟器套件包含了相当多的工具，但并不是全部都有。现在它仍然没有全部拥有它们。但是它还有一个。

开发人员现在可以通过模拟器套件在本地使用 Firebase 存储 API。使用这个 API 的任何东西现在都可以完全离线测试，从而节省了成本并增强了测试自动化。

## 安卓应用捆绑包(。aab)支持

Firebase 的另一个特性是它的内部测试分发工具。与 [Play Store 的内部测试功能](https://www.xda-developers.com/google-play-store-developers-internal-test-channel/)类似，开发者可以使用 Firebase 向 iOS 和 Android 用户分发其应用的内部测试版本，并从一个中心位置跟踪统计数据。

虽然[应用分发](https://firebase.google.com/products/app-distribution)工具自发布以来一直支持 APKs，但它不支持 Android 应用捆绑包。应用捆绑包是一种更有效的应用分发方式(如果平台支持的话)，因为它们只提供不同设备所需的应用部分。今天，Firebase 应用分发获得了对应用捆绑包的[支持](https://firebase.google.com/docs/app-distribution/android/distribute-console?apptype=aab)，有望使内部测试更容易运行。这是一个重要的公告，因为从 2021 年 8 月开始，Google Play 控制台将[要求所有新应用](https://www.xda-developers.com/google-android-app-bundle-play-store/)以 Android 应用捆绑格式发布。

## 应用程序检查

Firebase 可以存储一些非常敏感的数据。它可以包含游戏保存状态、个人信息或开发者选择的任何其他内容。虽然 Firebase 相当安全，但谷歌更进一步，推出了目前处于测试阶段的 [App Check](https://firebase.google.com/docs/app-check) 。应用程序检查是一个可选的功能，以防止任何东西或任何人连接到 Firebase，除非它得到特别授权。

目前，App Check 仅适用于云存储、实时数据库和云功能，但谷歌计划随着时间的推移扩大支持范围。

## 性能监控

性能监控是 Firebase 的另一个有用的特性。它让开发人员可以从一个页面上监控性能问题并查明其原因。但它并不完美。显示的数据会有延迟，这意味着新版本中的问题可能在几分钟、几小时甚至几天后才会出现。

然而，现在性能监控可以实时处理数据。一旦出现任何问题，开发人员都会看到。

## 新用户界面

并不是每个公告都是关于 Firebase 的一个新特性。还有一些 UI 大修。

远程配置、发布流和 A/B 测试结果页面都有了新的和改进的用户界面。谷歌表示，这些变化应该会让你更容易看到你想看的数据，同时排除更详细或不相关的数据。

## 新的 Web SDKs

到目前为止，很多新闻都是关于 Firebase 本身或 Android 和 iOS 的。但是也有一些新的网络内容，包括[一组新的网络应用软件开发工具包](https://firebase.google.com/docs/web/learn-more#modular-version)进入测试阶段。这些 SDK 是模块化的，这意味着开发人员可以只导入他们需要的 Firebase 部分，从而减少加载时间并节省空间。

## 新的 Firebase 扩展

在一些新的 SDK 之上，还有一些 Firebase 的新扩展。开发者可以与各种第三方提供商集成，为 Firebase 带来更好的体验。与 Algolia 的合作允许[通过 Firestore](https://firebase.google.com/products/extensions/firestore-algolia-search/) 进行搜索。MailChimp 扩展帮助开发者[向用户](https://firebase.google.com/products/extensions/mailchimp-firebase-sync)发送个性化电子邮件。MessageBird 集成为用户增加了另一种通信方式。最后，开发人员可以利用 Jigsaw 的[透视图 API 来自动分析用户生成的内容。](https://github.com/FirebaseExtended/experimental-extensions/tree/next/firestore-perspective-toxicity)

## Crashlytics

Crashlytics 可能是最受欢迎的 Firebase 工具之一，它也正在发生一些变化。首先，开发人员现在可以使用自定义键做更多的事情，查看它们的趋势，甚至根据键值过滤会话。

NDK 的和 T2 的也得到一些更新。NDK 现在提供更详细的堆栈跟踪，而 Unit 提供更好的崩溃分组和额外的游戏相关设备元数据，如 GPU、DPI 和屏幕分辨率。

* * *

这无疑是 Firebase 的一大变化。虽然其中许多是增量的，但它们只是加强了谷歌已经令人难以置信的一套工具。请务必查看谷歌的博客帖子，了解新内容的更多细节，或者查看我们在[谷歌 I/O 2021](https://www.xda-developers.com/tag/google-io-2021/) 上的其他报道，了解更多新闻。