# Android 12 测试通知的“自动”声音状态

> 原文：<https://www.xda-developers.com/android-12-tests-automatic-sound-status-notifications/>

谷歌昨晚发布了 Android 12 的第一个开发者预览版，好家伙，有很多很酷的东西可以谈论。我们已经详细介绍了 Android 最新版本中的一些主要变化，包括[滚动截图](https://www.xda-developers.com/android-12-finally-adds-scrolling-screenshots-natively/)功能、[原生单手模式](https://www.xda-developers.com/android-12-is-adding-a-native-one-handed-mode/)、 [UI 优化以实现更好的单手使用](https://www.xda-developers.com/android-12-better-one-handed-use/)、 [iOS 风格的小工具堆栈、](https://www.xda-developers.com/android-12-might-add-support-for-ios-esque-widget-stacks/)等等。随着我们继续深入挖掘新软件，我们不断发现新的功能和微妙的变化，而这些并没有立即引起我们的注意。

我们发现的许多功能都是半成品或仍在开发中，因此在第一次预览中还没有上线。我们在 Android 12 开发者预览版 1 中发现的一个有趣的功能是，系统可以自动决定传入通知的声音状态。

现在，在 Android 11 中，当你在一个通知上半滑动并点击齿轮图标时，你会看到两个选项:默认和静音。默认状态对应于系统范围的声音配置文件，并且可以根据所选的声音配置文件允许通知响铃或振动。同时，在这里选择静音选项会完全禁用该应用程序的声音和振动——无论系统声音配置文件如何。然而，在 Android 12 中，谷歌正在努力增加第三个选项，名为 Automatic，不出所料，它会自动决定通知是否应该发出声音或振动。

我们的主编米沙·拉赫曼[找到了一些与这个新功能相关的字符串](https://twitter.com/MishaalRahman/status/1362580166795526155)，甚至设法让它工作起来。以下是显示该功能运行情况以及与 Android 11 相比如何的截图:

```
 <string name="feedback_alerted">This notification was automatically &lt;b>promoted to Default&lt;/b> by the system.</string>
<string name="feedback_demoted">This notification was automatically &lt;b>ranked lower&lt;/b> in your shade.</string>
<string name="feedback Ok">OK</string> <string name="feedback_promoted">This notification was automatically &lt;b>ranked higher&lt;/b> in your shade.</string>
<string name="feedback_prompt">Was this correct?</string>
<string name="feedback_response">Thanks for your feedback!</string>
<string name="feedback_silenced">This notification was automatically &lt;b>demoted to Silent&lt;/b> by the system.</string> 
```

这项功能尚未在 Android 12 开发者预览版 1 中上线，因为它可能需要更多的时间。我们不知道谷歌计划什么时候实现它，但这肯定是我们希望看到的最终版本。与此同时，请继续关注 XDA 门户网站，因为我们还有更多关于 Android 12 的新闻等着您！