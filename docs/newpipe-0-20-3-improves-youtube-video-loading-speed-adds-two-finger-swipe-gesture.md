# NewPipe 0.20.3 提高了 YouTube 视频加载速度，并增加了新的双指滑动手势

> 原文：<https://www.xda-developers.com/newpipe-0-20-3-improves-youtube-video-loading-speed-adds-two-finger-swipe-gesture/>

# NewPipe 0.20.3 提高了 YouTube 视频加载速度，并增加了新的双指滑动手势

第三方 YouTube 客户端 NewPipe 的最新更新提高了 YouTube 视频加载速度，并带来了新的双指滑动手势。

Android 的开源 YouTube 客户端 NewPipe 上个月初收到了一个重大更新。此次更新包括我们[在之前的测试版本](https://www.xda-developers.com/newpipe-tests-unified-player-ui-seamless-fullscreen-switching/)中看到的统一视频播放器 UI 和其他几项改进。推出后不久，该应用程序收到了另一个更新，修补了 YouTube 搜索的一个漏洞。NewPipe 背后的开发人员现在正在推出另一个更新，为 YouTube 视频加载速度和新的滑动手势带来了改进。

根据 NewPipe 博客上最近的一篇文章,最新的更新(v. 0.20.3)引入了一个新的双指向下滑动手势，使关闭嵌入式播放器变得更加容易。在之前的版本中，关闭嵌入式播放器需要两步。你首先必须向下滑动嵌入式播放器以切换到迷你播放器，然后再次向下滑动以关闭它。现在，您可以使用新的双指向下滑动手势一次性关闭嵌入式播放器。

最新更新的第二个重大改进是，NewPipe 现在加载 YouTube 视频的速度快了很多。正如博文所解释的，*“YouTube 已经移除了大部分 URL 的模糊处理，所以现在我们可以直接访问它们，大大加快了视频加载速度！deobfuscation 代码仍被缓存，以备不时之需。*其他值得注意的变化包括:

*   所有不同的排队选项现在都被一个统一的选项所取代
*   该应用程序现在有一个新的设置，允许用户清除 reCAPTCHA cookies
*   增加了一个新的选项，关闭 Android 8.0 及以上版本播放流时弹出的彩色通知。启用后，通知具有静态颜色。
*   增加了对 YouTube 短网址的支持
*   增加了对类似于“youtube.com/username”的缩短频道链接的支持
*   增加了对丢弃重定向 URL 上的额外链接的支持，以帮助用户在 NewPipe 中打开来自 Google 的链接。

如果你已经在你的设备上安装了 NewPipe，当你打开它的时候，这个应用会提示你更新到最新的版本。如果你没有旧版本，你可以从 NewPipe 的 [GitHub](https://github.com/TeamNewPipe/NewPipe/releases) 获取最新版本。要查看最新版本中的所有其他改进/修复，请查看下面的 changelog 部分。

### 新管道 0.20.3 变更日志

*   新的
    *   仅用一个#4425 替换特定的入队选项
    *   两指关闭玩家手势#4476
    *   在设置中添加按钮以清除 reCAPTCHA cookies # 4453
    *   添加不着色通知#4643 的选项
*   改良的
    *   不显示通知创建/更新时间#4410
    *   删除记住弹出窗口属性设置#4367
    *   甚至在更换单个视频队列之前也要求确认#4463
    *   删除流历史#4413 时也删除流状态
    *   改进年龄限制和 yt 限制内容字符串#4354
*   固定的；不变的
    *   修复了当流暂停和快进/快退按钮被点击时的崩溃#4410
    *   修复当不存在本地播放列表时播放列表显示对话框#4345
    *   不要通过拖动缩略图来重新排列列表#4550
    *   修复开放的 VideoDetailFragment 和更多#4562
        *   修复无限缓冲
        *   更好地检测何时自动播放，何时不自动播放
        *   让 NewPipe 的共享更加一致
    *   修复播放列表选择对话框并做一些重构#4771
    *   将 YouTube 订阅导入说明更改为 Google 外卖#4759
    *   将 Gigaget 的许可证从 GPLv2 更正为 GPLv3 #4892
*   本地化
    *   添加 Santali 语言#4749
    *   添加 Central Atlas Tamazight 本地化
    *   添加自述文件#4845 的韩语翻译
    *   更新的翻译
*   发展
    *   在 VideoPlayerImpl #4338 中使用 DisplayCutoutCompat
    *   使用 DrawableCompat。#4592
    *   使用上下文兼容方法#4276
    *   请使用 textviewcompt . setcompoundrawablesrelativewithitrinsicbounds()。#4594
    *   隐藏泄漏启动器图标#4436 #4450
    *   格式化所有 XML 资源#4471
    *   禁用 Ktlint 挂起上游更新#4517
    *   使用核心 KTX 函数#4547
    *   对所有生成类型使用 multidex。#4557
    *   将 AboutActivity 迁移到 ViewPager2 # 4553
    *   优化和缩小应用程序 PNGs #4610
    *   将通知操作转换为自定义首选项#4652
    *   使用 Java 8 APIs # 3817 # 4556
    *   分离玩家手势逻辑和 UI #4587
    *   使用 RxJava 代替 AsyncTask #4499
    *   将循环索引从 float 改为 int #4784
    *   更多杂项小修复和改进#4710
    *   修复队列处理中的 NullPointerException 并提高性能#4555
*   其他的
    *   拉动式请求模板返工#4317
    *   问题模板已返工#4378 #4379 #4415 #4431 #4606
    *   添加关于如何使用本地新管道提取器版本#4528 的信息
    *   将 Weblate 小部件添加到自述文件#4530

https://f-droid.org/en/packages/org.schabi.newpipe/