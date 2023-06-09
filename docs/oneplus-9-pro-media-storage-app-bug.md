# 据报道，一加 9 Pro 的媒体存储应用程序占用了太多空间

> 原文：<https://www.xda-developers.com/oneplus-9-pro-media-storage-app-bug/>

# 据报道，一加 9 Pro 的媒体存储应用程序占用了太多空间

如果你最近在你的一加 9 Pro 上看到“存储空间耗尽”的警告，尽管没有大量使用，你并不孤单。

如果你最近在你的[一加 9](https://www.xda-developers.com/oneplus-9/) Pro 上看到“存储空间耗尽”的警告，尽管没有大量使用，你并不孤单。显然，一个与媒体存储应用程序相关的错误导致了一加 9 Pro 上异常高的存储使用率，[许多用户报告](https://forums.oneplus.com/threads/high-data-on-mediastorage.1421739/)他们的存储空间几乎被填满。

Android Police 的 Artem Russakovskii 是受影响的一员。Artem 在 Twitter 帖子中分享了他的经历和发现，因为他的 256GB 存储的一加 9 Pro 在存储空间几乎填满后变得缓慢和无响应。像许多其他受影响的[用户一样，](https://forums.oneplus.com/threads/media-storage-literally-duplicating-sd-memory-usage.1475846/) Artem 最初很难找出不寻常的存储使用背后的真正原因，但他能够确定问题出在媒体共享应用程序上，该应用程序独自占用了高达 126GB 的空间。

一些用户[推测](https://www.reddit.com/r/oneplus/comments/mzhpe3/media_storage_app_using_way_too_much_space/)(通过[PiunikaWeb](https://piunikaweb.com/2021/08/23/oneplus-9-pro-media-storage-app-using-too-much-space-you-arent-alone/))不寻常的存储使用可能是由于媒体存储应用程序将媒体文件计数了两次——例如，一个 5GB 的视频文件最终占用了 10GB 的空间。

然而，似乎这个问题实际上可能与一加画廊应用程序的垃圾桶功能有关，该功能要么不能有效地删除已删除的文件，要么根本不能删除它们。如果你的一加 9 Pro 受到这个 bug 的影响，有一个临时的修复方法——清空回收站。

目前还不清楚这个问题有多普遍，也不清楚它是否是由最近的软件更新引起的。一加还没有对此事发表官方评论，但是一旦我们有了更多的信息，我们一定会让你知道的。