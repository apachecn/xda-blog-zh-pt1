# chrome 操作系统可能很快会让你快速访问谷歌照片

> 原文：<https://www.xda-developers.com/chrome-os-easier-access-google-photos/>

在 Chromebook 上管理谷歌照片可能会变得容易得多，因为谷歌正在努力将谷歌照片集成到 Chrome OS 的文件管理器中。现在，Chrome OS 用户不得不手动从 Google Photos 下载他们的照片，然后将它们组织到他们的文件管理器中，这是非常繁琐的。许多用户过去都抱怨过这一点，看起来谷歌似乎终于意识到了 Chrome OS 用户必须采取这种违反直觉的方法来访问他们的照片。

我们在 [*的朋友 Android Police*](https://www.androidpolice.com/2021/02/12/google-photos-may-finally-be-integrated-into-the-chromeos-file-manager/) 在 Chromium Gerrit 上发现了一些新的提交，这表明谷歌正在努力将谷歌照片深度集成到文件管理器的导航窗格中，允许用户从文件管理器中快速访问他们上传的照片。

下面的[提交](https://chromium-review.googlesource.com/c/chromium/src/+/2690121)建议用户在文件拾取器中拾取文件时能够查看他们的 Google 相册。

> [filesapp]仅在文件选取器中显示照片卷
> 
> 只有在 Chrome 中拾取文件时，才会显示 Google 相册的音量
> 
> OS，并在 ARC 中浏览或拾取文件时隐藏。
> 
> BUG=1170198

与此同时，另一个提交提到为 Google 相册添加一个欢迎横幅。

> [filesapp]为 Android 照片添加欢迎横幅
> 
> 显示 Android Photos 文档提供程序卷的欢迎横幅。除非取消，否则横幅最多显示 3 次。
> 
> BUG=1171651

由 *Android Police* 进一步挖掘[代码](https://chromium-review.googlesource.com/c/chromium/src/+/2690041/3/ui/chromeos/file_manager_strings.grdp)证实，该集成将允许用户直接从文件管理器中浏览和选择他们最近上传的照片。用户在 ChromeOS 设备上安装应用程序后，Google Photos 快捷方式将显示在导航窗格中。

对于 Chrome OS 用户来说，这一变化令人兴奋，但不能保证谷歌会将这些提交合并到 Chromium 源代码中，并将该功能变为现实。如果谷歌最终决定将该功能发布到 Chrome 操作系统上，我们一定会让你知道。