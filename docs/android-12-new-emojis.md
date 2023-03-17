# 谷歌在 Android 12 中更新了近 1000 个表情符号

> 原文：<https://www.xda-developers.com/android-12-new-emojis/>

表情符号已经成为在信息传递中分享情感和意图的重要手段，特别是由于仅通过文字难以传达你的语气。新的表情符号经常被添加到 Unicode 标准中，通常需要发布操作系统升级以在系统级别上支持这些新的表情符号。谷歌[一直致力于](https://www.xda-developers.com/google-prepares-decouple-new-emojis-android-system-updates/)使包含新表情符号的字体文件可更新，而不需要更新 Android 系统，今天该公司暗示这将成为 [Android 12](https://www.xda-developers.com/android-12/) 的一个功能。

在一篇博客文章中，谷歌还宣布数百个有趣的小图标——准确地说是 992 个——已经被修饰和改进，使它们更通用、更易访问、更真实，而且还有新的图标。例如，一个“派”的表情符号现在不那么美国化了，它指的是世界上大多数人可能知道的“派”，而不是南瓜派。

根据谷歌的说法，所有支持 Appcompat 库的应用程序都会自动从谷歌获得最新的表情符号。无论你的手机有多旧，或者你的应用程序需要多长时间才能更新，从 Android 12 开始，你将在使用 Appcompat 的应用程序中获得最新的表情符号。目前，你可以在任何根植的 Android 设备上获得新的 [Android 12 表情符号，但根植显然不是那么用户友好。没有什么比让你的应用程序自动抓取所有新的表情符号更简单的了。](https://www.xda-developers.com/get-android-12-new-emojis-rooted-android-device/)

我们在 [*的朋友 Android Police*](https://www.androidpolice.com/2021/07/16/android-12-is-getting-new-emoji-and-googles-making-familiar-promises-about-decoupling-them-from-future-updates/) 做了一些挖掘来了解更多关于这个公告的信息。如果你已经关注 Android 很长时间了，那么表情符号与 Android 系统的分离可能听起来很熟悉。这无疑给我敲响了警钟，我不知道为什么。事实证明，早在 2017 年，谷歌就说过几乎完全相同的话，当时他们宣布[支持名为“EmojiCompat”](https://www.xda-developers.com/android-o-redesigns-the-emojis-get-them-now-on-any-rooted-android-5-0-device/)的支持库，该库工作在 API 级别 19 或以上(Android 4.4+)。像 Gboard 和 Google Messages 这样的第一方应用程序利用了这一点(这也是为什么你可以在 Gboard 中获得新的表情符号)，但很少有第三方应用程序这样做。基本上，它可能不是系统的一部分，而是开发者实际上需要选择的东西。因此，我们不清楚今天的声明是否与新增加的通过 Google Play 服务更新字体文件的支持有关。

当安卓警察联系谷歌时，他们问 T2 为什么没有实现主线模块 T3。在这种情况下，“主线”意味着它是 Android 核心服务的一部分，但这是一个面向 GMS 核心的变化，是 Google Play 服务和 [Android Jetpack](https://www.xda-developers.com/google-io-2021-new-features-jetpack-android-studio-kotlin/) 的一部分。谷歌的回应相当于说，GMS-core 集成的变化不需要“额外的开发人员工作”，坚持 EmojiCompat 方法意味着“它将在旧设备上工作”。不过，这似乎忽略了一个事实，即谷歌特别宣传这是 Android 12 的一个变化。

很久很久以来，很多人一直呼吁将表情符号与安卓系统分离。每当发布新表情符号，iPhone 用户首先得到它们时，你很可能会因为缺乏另一方可能正在使用的表情符号的上下文而导致沟通失误。因为它们被认为是“字体”，并且字体最终可能能够在 Android 智能手机的/data 分区中更新，所以你*可能*能够通过 Google Play 服务获得未来将包括表情符号的更新。

无论如何，可更新的表情符号是一种生活质量的改善，对一些人来说可能看起来很傻，但鉴于表情符号已经成为我们日常用语的一个重要部分，在必要时让它们容易更新并跟上速度是很重要的。无论如何，我们希望这是等式的一部分。