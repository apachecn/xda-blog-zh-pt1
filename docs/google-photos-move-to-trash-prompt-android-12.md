# Google 相册在 Android 12 上删除文件不会征求你的许可

> 原文：<https://www.xda-developers.com/google-photos-move-to-trash-prompt-android-12/>

如果你在英雄图像中看到过令人讨厌的弹出窗口，要求你允许 Google 相册删除文件，请举手。如果你在一部不是谷歌 Pixel 的手机上运行 Android 11。绝大多数手机)，那么你可能已经看到了弹出窗口。很多。事实上，每次你试图在谷歌照片应用中删除照片时，你都会看到弹出窗口*。幸运的是，[不想要的截图备份](https://www.xda-developers.com/android-12-stop-screenshots-backing-up-google-photos/)并不是 [Android 12](https://www.xda-developers.com/android-12/) 可能为谷歌照片用户解决的唯一问题。新的开发者文档表明，即将发布的操作系统将允许照片等图库应用程序修改文件，而无需不断提示用户。*

Android 11 上的 Google Photos(和其他图库应用)要求用户允许删除文件的原因很复杂，但基本上可以归结为一个事实，即它们不是系统图库应用。嗯，对于 Pixel 手机来说就不一样了，照片应用*是*系统图库应用，这就是为什么 Pixel 用户从来看不到这个弹出窗口。但在三星、小米、一加、华硕和其他公司的大多数设备上，谷歌照片不是(也不能被设置为)系统图库应用。幸运的是，在 Android 12 上不再需要这样了。

在 [Google I/O 2021](https://www.xda-developers.com/google-io-2021-recap/) 发布[首个 Android 12 测试版](https://www.xda-developers.com/android-12-beta-1-hands-on/)的同时，谷歌更新了其“功能和 API 概述”页面，增加了一个关于“[媒体管理访问](https://developer.android.com/about/versions/12/features#media-management-access)的部分根据谷歌的说法，一个以 API level 31 (Android 12)为目标的应用程序可以请求用户授予它修改文件的权限，将文件移入和移出[垃圾桶](https://www.xda-developers.com/android-11-hidden-recycle-bin-trashed-photos-videos/)，或者删除文件，而不需要为每个文件操作提示用户。一旦应用程序更新到 Android 12，它需要做的就是声明三个权限(`MANAGE_MEDIA`、`READ_EXTERNAL_STORAGE`和`ACCESS_MEDIA_LOCATION`)，向用户显示一个 UI，解释为什么应用程序需要媒体管理访问，并指引用户到 Android 12 上新的“媒体管理应用程序”屏幕以授予它权限。

听起来很简单，对吧？由于这是一个全新的 API，大多数图库应用程序还没有更新以利用它。是的，这意味着谷歌照片应用程序也需要更新才能使用。目前，很少有用户运行 Android 12 测试版，他们中的大多数人可能都在 Pixel 手机上，这甚至不存在问题，所以谷歌可能没有太大的压力来立即更新照片应用程序。不过，希望他们能在几个月后 Android 12 开始推出第一批非像素手机之前推出更新。

*感谢推特用户@[doraeigah](https://twitter.com/Doraeigaah)的提示！*