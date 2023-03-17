# 谷歌文件将很快得到一个垃圾文件夹，以帮助您恢复被删除的文件

> 原文：<https://www.xda-developers.com/files-by-google-1-0-345-prepares-trash-folder-restoring-deleted-files/>

回到今年 6 月，谷歌发布了一段视频，详细介绍了 Android 11 中存储访问的变化。视频[强调了一种新的“垃圾处理”机制](https://www.xda-developers.com/android-11-hidden-recycle-bin-trashed-photos-videos/)，它将允许应用程序垃圾处理文件，而不是删除它们，这实质上给了用户一个在 30 天内恢复垃圾文件的机会。但是我们还没有看到一个应用程序利用这种新的垃圾机制，尽管 [Android 11](https://www.xda-developers.com/tag/android-11/) 已经推出几周了。然而，这可能很快就会改变，因为谷歌现在正准备通过谷歌应用程序向文件添加一个垃圾桶文件夹。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

谷歌最新版本的文件(1.0.345 版)今天开始在 [Play Store](https://www.xda-developers.com/tag/google-play-store/) 上发布。在面向用户的变化方面，更新对音频播放器进行了改进，以增强背景播放，文件分组以实现更轻松的浏览体验，以及屏幕截图清理以帮助用户检测和删除旧屏幕截图。

除了这些变化，更新还包括指向一个名为“Trash”的新菜单项的新字符串，以帮助用户恢复已删除的文件。我们的主编[米沙·拉赫曼](https://www.xda-developers.com/author/mishaalrahman/)设法手动启用了这个新功能，下面是它的样子:

正如你在附上的截图中看到的，点击左上角的汉堡菜单图标可以进入新的“垃圾桶”选项。点击该选项会打开一个新页面，按时间倒序列出所有已删除的文件。在页面的顶部，你可以看到一个提示，上面写着:*“任何在回收站中保存了 30 天的文件都将被永久删除。*”页面底部还包括两个按钮，用于恢复和永久删除选中的文件。此外，页面右上角有一个按钮，用于在列表和网格视图之间切换。

虽然这些截图让我们很好地了解了垃圾桶功能，但值得注意的是，该功能尚未向任何人推出。我们通过在运行 Android 11 的 [ZenFone 7 Pro](https://www.xda-developers.com/asus-zenfone-7-pro-review-a-flipping-fantastic-flagship-smartphone/) 上侧载谷歌 APK 的[最新文件来验证这一点，我们看不到垃圾桶选项。同样值得注意的是，该功能应该可以在运行旧版本 Android 的设备上使用，但我们目前只在 Android 11 上测试了它。](https://www.apkmirror.com/apk/google-inc/files-go/#description)

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*