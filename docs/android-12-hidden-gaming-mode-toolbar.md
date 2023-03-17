# Android 12 有一个隐藏的游戏工具栏，悬浮在你的屏幕上

> 原文：<https://www.xda-developers.com/android-12-hidden-gaming-mode-toolbar/>

# Android 12 有一个隐藏的游戏工具栏，悬浮在你的屏幕上

第一个 Android 12 开发者预览版有一个隐藏的游戏工具栏，浮动在屏幕上，有一个按钮来记录你的游戏。

从我们发现的所有很酷的新功能来看，今年的 [Android 12 更新](https://www.xda-developers.com/android-12/)将成为谷歌多年来最大的发布。今天早些时候，XDA 承认网站的开发者和朋友 [Quinny899](https://forum.xda-developers.com/m/quinny899.3563640/) 让我们第一次看到了 Android 12 的[隐藏对话小工具](https://www.xda-developers.com/android-12-conversation-widget-first-look/)，但这不是他启用的唯一功能。由于一些逆向工程，他设法让谷歌的隐藏游戏仪表板功能工作。它目前非常简单，只有一个浮动工具栏和两个非功能按钮，但这是我们第一次看到另一个未发布的 Android 12 功能。

正如你在下面的截图中看到的，两个图标重叠在屏幕的顶部:一个记录图标和一个控制器图标。

 <picture>![](img/272146253046be7bb9522df3190d6e60.png)</picture> 

Android 12's hidden, in-development gaming toolbar. Credits: Kieron Quinn/Quinny899.

根据 Android 12 的 SystemUI 中包含的游戏仪表板代码，录制按钮只是启动一个屏幕录制会话。当你想通过拉下快速设置面板来录制屏幕而不中断游戏时，这将非常有用。至于带有控制器图标的按钮，我们不知道它会做什么，因为它不起作用，代码中也没有明显的功能。

游戏仪表板类是`com.google.android.systemui`名称空间的一部分，而不是`com.android.systemui`，这表明该功能可能是像素专有的。然而，许多原始设备制造商已经有了他们自己的游戏模式功能，现在这个版本没有什么突出的。在第一个开发者预览版发布之前，我们得知谷歌[正在为 Android 12](https://www.xda-developers.com/android-12-smart-autorotate-game-mode-reduced-brightness/) 开发游戏模式。我们不知道这种新的游戏仪表板和我们听说的游戏模式是否是同一个，或者前者只是建立在新的 GameManager 服务之上的一个功能。不过，我们可能会从后续的 Android 12 开发者预览版中了解更多信息。