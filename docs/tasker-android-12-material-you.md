# Tasker developer 展示了 Android 12 的变色主题系统

> 原文：<https://www.xda-developers.com/tasker-android-12-material-you/>

Android 12 大更新最令人兴奋的新功能之一是新的基于壁纸的主题系统，代号为“莫奈”这是谷歌新的“[材料*你*](https://www.xda-developers.com/material-you/) ”设计语言的主要部分，强调个性化。新的主题系统在 [Android 12 Beta 2](https://www.xda-developers.com/android-12-beta-2-features/) 中上线，但就像 Android 10 中引入黑暗模式一样，大多数开发者需要一段时间来调整他们的应用程序以支持主题。虽然谷歌尚未发布 Material You 的文档，但 Android 12 Beta 2 使开发者有可能在其应用中实现动态主题化。面向 Android 高级用户的自动化应用 Tasker 的开发者是第一批这样做的人之一。

在他的 YouTube 频道上，Tasker 开发者 joo Dias 展示了他添加到 Tasker 主题设置中的新“材料你”选项。一旦启用，Tasker 的动作栏、底部栏、菜单、切换、分隔线和文本会采用你的壁纸的颜色。该应用程序本身不能以编程方式改变主题，因为[没有针对它的公共 API](https://issuetracker.google.com/issues/188703883)，但很高兴看到它如此快速地适应新的主题系统。

根据谷歌的说法，Android 12 的颜色提取系统使用一种带有材料颜色目标的聚类算法来确定主色和次主色，然后应用与你当前壁纸匹配的色调。然后可以使用调色板来确定与壁纸最接近的色调。颜色的选择是明智的，因此它们不会冲突或引入易读性问题。

第三方应用程序开发人员可以查询系统生成的强调色，以将主题应用到自己的应用程序中，这正是 Tasker 开发人员所做的。通过在运行时简单地从适当的 [R.color](https://developer.android.com/reference/android/R.color) 值中获取颜色，Tasker 应用程序能够将其颜色与用户的壁纸相匹配。基于当前的主题，[也应该可以改变应用程序的图标](https://www.xda-developers.com/android-12-beta-2-features/#android12beta2_icontheming)，但是 Tasker 开发者还没有在他的应用程序中加入对它的支持。

\ r \ nht TPS://www . YouTube . com/watch？v=a_tX1ybgkB8\r\n

由于谷歌还不允许为 Android 12 构建的应用发布在 Google Play 上，Tasker 开发者还没有发布具有该功能的更新。然而，一旦谷歌实现了将针对 API 级别 31 的应用发布到 Google Play，那么预计该功能将首先登陆 Tasker beta 频道。您可以从下面嵌入的 Play Store 链接下载 Tasker 应用程序的最新版本。

虽然 Tasker 应用程序是我见过的第一个包含动态主题的应用程序，但它绝对不是唯一的一个。我采访过的几个开发者已经开始在他们应用的私有版本中测试新的主题化系统，尽管他们还没有准备好展示任何进展。一些开发人员正在开发新的库或更新现有的库，以添加对 Android 12 动态着色的支持，我们预计一旦我们接近 Android 12 的正式发布，将会有更多这样的项目出现。