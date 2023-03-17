# Android 12 将自动休眠未使用的应用程序以释放空间

> 原文：<https://www.xda-developers.com/android-12-hibernate-unused-apps/>

尽管在 Pixel 手机的稳定版本准备就绪之前，谷歌不会发布新 Android 版本的源代码，但我们很少能通过提交给 AOSP Gerrit 的代码更改看到一些即将推出的功能。我们一直期待在即将到来的 [Android 12](https://www.xda-developers.com/android-12/) 版本中登陆的功能之一是应用程序休眠，这一功能将通过删除未使用的应用程序中的临时文件来[释放存储空间](https://www.xda-developers.com/android-12-hibernate-apps/)。虽然这一功能没有出现在两个公开的开发者预览版中，但我们可以确认该功能的代码出现在我们最近获得的[泄露版本](https://www.xda-developers.com/android-12-beta-features-leak/)中。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

随着 Android 11 开发者预览版 3 的发布，谷歌[增加了](https://www.xda-developers.com/android-11-developer-preview-3-changes/#:~:text=App%20permissions%20can%20be%20automatically%20revoked%20if%20the%20app%20hasn%E2%80%99t%20been%20used%20for%20months)一个新的“自动撤销权限”功能，如果应用程序几个月没有使用，就会撤销该应用程序的权限。随着 Android 11 的稳定发布，谷歌[分享了关于该功能的更多细节](https://www.xda-developers.com/android-11-developer-preview-3-changes/#:~:text=App%20permissions%20can%20be%20automatically%20revoked%20if%20the%20app%20hasn%E2%80%99t%20been%20used%20for%20months)，包括一个屏幕截图，显示当应用程序的权限被撤销时通知用户的通知，以及一个屏幕截图，显示“未使用的应用程序”设置页面，其中列出了权限被自动撤销的应用程序。

在 Android 12 中，谷歌似乎在扩展“未使用的应用”的概念，推出了新的应用休眠功能。除了自动撤销未使用应用的权限，Android 12 还将清理临时文件以释放存储空间。

我们为每个应用程序在“应用程序信息”页面上激活了一个新的“未使用的应用程序”部分，它包含一个新的“删除权限和释放空间”开关。相比之下，Android 11 的“自动撤销权限”开关(后来更名为“如果应用程序未被使用，则移除权限”)可以在应用程序的“应用程序信息”页面的“应用程序权限”子页下找到。这种位置上的变化是有意义的，因为新的切换处理权限和存储，而不仅仅是权限。

在我们手动休眠了几个应用程序后，“未使用的应用程序”页面出现在设置>应用程序下。该页面显示了几个月没有打开的应用，其描述称，如果一个应用几个月没有使用，权限将被撤销，通知将被停止，临时文件将被删除。

根据我们[今年早些时候发现的代码变化](https://www.xda-developers.com/android-12-hibernate-apps/)，应用程序休眠功能将清除缓存和/或删除编译工件，以释放存储空间。这些操作都不会释放大量空间，但这取决于哪个应用程序正在休眠，以及存储了多少/何种缓存文件。拥有存储容量更少的低端设备的用户将受益更多，但所有用户都将受益于未使用的应用程序的权限被自动撤销。

虽然我们获得的版本比开发者预览版 2 更新，但我们不知道 app 休眠功能是否会在 DP3 或 Beta 1 中公开亮相。但是，一旦它可用，就可以通过“`cmd app_hibernation`”命令访问它的命令行界面。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*