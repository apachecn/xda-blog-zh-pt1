# 谷歌可能会在 Android 12 中让用户管理 Android 的隐藏回收站

> 原文：<https://www.xda-developers.com/android-12-recycle-bin/>

谷歌 I/O 2021 [将于下月 5 月 18 日开始](https://www.xda-developers.com/google-io-2021-registration-dates/)，在这次活动中，我们期待看到谷歌宣布所有即将来到 [Android 12](https://www.xda-developers.com/android-12/) 的功能。在活动开始之前，我们已经从两个公开的开发者预览版中收集了尽可能多的关于最新操作系统发布的信息。前几天，我们还接触到了尚未发布的 Android 12 版本，并展示了我们能找到的许多较小的功能和设计变化。在深入研究了框架和系统应用程序后，我们发现了一些代码，表明谷歌可能会在存储设置中展示 Android 的隐藏回收站/垃圾桶功能。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

去年，谷歌推出了 Android 11，对应用程序访问设备存储的方式进行了重大改变。这些变化被谷歌称为“范围存储”，极大地限制了应用程序默认可以获得的存储访问量。虽然某些应用程序，如文件管理器[可以请求对设备存储的广泛访问](https://www.xda-developers.com/android-11-all-files-access-permission-form/)，但其他应用程序必须使用替代 API 来添加、打开、编辑或删除存储上的文件。其中一个 API 被称为 [MediaStore API](https://developer.android.com/reference/android/provider/MediaStore) ，它提供对音频、视频和图像等常见媒体文件的访问。MediaStore 实际上已经存在了一段时间，但谷歌在 Android 11 发布时为 API 添加了一个新功能:[垃圾处理](https://www.xda-developers.com/android-11-hidden-recycle-bin-trashed-photos-videos/)。

使用 MediaStore API 的应用程序可以丢弃而不是删除文件，让用户有机会在以后恢复文件。大多数桌面操作系统都有类似的功能，但 Android 11 本身并没有提供一个系统范围的“回收站”或“垃圾桶”文件夹来列出所有已被丢弃的文件。相反，拥有垃圾文件编辑权限或要求用户同意的应用程序可以显示隐藏回收站中的项目，我们发现有证据表明，谷歌自己的 Google app 文件正在准备添加这样的功能。

*Google app 的文件中隐藏的垃圾桶文件夹。*

然而，在 Android 12 中，谷歌似乎正在努力在设置>存储中添加一个新条目，以显示所有垃圾项目占用的存储空间。点击这个条目将启动一个片段，显示已被丢弃的文件的数量，并让用户清空垃圾箱，但由于 Google 将其硬编码为 false，该入口点通常是不可访问的。然而，多亏了 XDA 的[扎卡里·旺德](https://twitter.com/Wander1236)的一点努力和帮助，我们设法让入口点和对话框出现了。

虽然用户可以从这里清空垃圾，但我们不知道用户是否也能够通过这个入口点恢复它们。不过，谷歌即将推出的[垃圾文件功能将允许用户查看、恢复或永久删除垃圾文件。如果谷歌计划在 Android 12 发布的同时推出谷歌文件的新功能，我们不会感到惊讶，尽管从技术上讲，谷歌垃圾功能的文件实际上并不需要安装 Android 12。](https://www.xda-developers.com/files-by-google-1-0-345-prepares-trash-folder-restoring-deleted-files/)

Android 上的垃圾项目目前对大多数文件管理器都是隐藏的，因为它们以“.”开头在它们的文件名中，这是 Android 理解文件应该被认为是隐藏的方式。这些隐藏的垃圾文件存储在它们原来所在的目录中，而不是移动到系统范围的回收站/垃圾桶文件夹中。根据我们所知，看起来谷歌并不打算在 Android 12 中添加一个实际的回收站/垃圾桶文件夹，但看起来谷歌确实打算至少让垃圾桶成为一个更突出的功能。一个问题是，应用程序必须使用 MediaStore API 将文件标记为“垃圾”，因此一些应用程序将继续永久删除文件或利用自己的回收站，阻止用户在一个容易访问的位置查看和恢复文件。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*