# DotOS 5.1 将增加一个新的基于壁纸的主题系统和受 Android 12 启发的 QS 用户界面

> 原文：<https://www.xda-developers.com/dotos-5-1-new-wallpaper-based-theming-system-qs-ui-inspired-by-android-12/>

从早期的 CyanogenMod 主题引擎到现在的原生 RRO 和 OMS API，Android 主题化已经走过了漫长的道路。凭借 [Android 12](https://www.xda-developers.com/android-12/) ，谷歌可能会将 Android 的主题引擎推向一个新的高度，这要归功于[新的基于壁纸的主题系统](https://www.xda-developers.com/android-12-theming-system/)代号为“monet”[当“莫奈”被启用](https://www.xda-developers.com/android-12-wallpaper-theming-system-leak/)时，用户的壁纸决定了整个设置和 SystemUI 的背景色和强调色，使其成为真正的动态主题化解决方案。然而，开发者和修改者还不能检查谷歌增强的主题化系统的代码库。这是因为 Android 12 仍处于“开发者预览”阶段，软件巨头将在稳定发布后才开始将 Android 12 源代码上传到 Android 开源项目(AOSP)网站。

DotOS 项目的人们现在正在尝试移植这一功能，他们受 Android 12 的启发，创建了自己版本的基于壁纸的主题化系统。对于那些不熟悉 DotOS 的人来说，它代表“DroidOnTime ”,是由 XDA 公认的贡献者 [mohancm](https://forum.xda-developers.com/m/mohancm.7471004/) 在 AOSP 基础上创建的定制 ROM，增加了几个功能，使使用 ROM 比普通的 AOSP 更愉快。新的主题引擎只是即将到来的 DotOS 5.1 版本中计划的功能之一。

DotOS 5.1 中的主题化系统被称为“MonetWannabe”，允许用户选择他们希望从壁纸中生成的调色板类型，并控制颜色生成过程的准确性。Iacob Ionut，又名 XDA 高级成员 [IacobIonut-DW](https://forum.xda-developers.com/m/iacobionut-dw.7481761/) ，是 DotOS ROM 的核心 UI/UX 开发者，他在仔细逆转谷歌在 Android 12 中的实现并调整底层算法以获得更好的灵活性后，从头开始编写了整个框架。

*想赚钱的人在行动*

主题引擎本质上是相当模块化的。启用后，甚至可以对快速设置媒体控件重新着色(如下所示)。人们可以简单地关闭框架，坚持手动着色。

除了基于壁纸的主题系统，DotOS 团队还推出了一个改进的快速设置面板 UI——其中一部分已经在之前的截图中可见。更准确地说，UI 重新设计的灵感来自于 [Android 12 早期模型](https://www.xda-developers.com/android-12-first-look-screenshots/)，但你可以找到许多其他设计元素与之混合。首先，通知和媒体播放器的边角稍微有点圆。“编辑”和“设置”按钮也进行了类似的修改，使其更易于访问，并与面板中的其他元素相匹配。接下来是 QS 定制，它失去了旧的背景和工具栏，并获得了一层新的油漆。

*改进的快速设置面板 UI:亮模式与暗模式*

此外，开发者已经决定重新装饰 [PackageInstaller](https://developer.android.com/reference/android/content/pm/PackageInstaller) 模块，这是 Android 操作系统的基础部分。如果你认为 PackageInstaller 只不过是一个过时的浮动框，显示应用程序的安装进度，那么你应该在看一眼大修后的版本后感到惊讶。

DotOS 5.1 更新中还会有更多的 UI 革新。例如，黑暗模式设置页面将被重新制作以保持一致性。你可以先睹为快，看看下面的重新设计:

* * *

### 下载 DotOS 5

您可以从项目的官方下载门户下载以下设备的当前 DotOS 5 版本:

*   **华硕**
*   谷歌
*   **联想**
*   **一加**
*   **现实**
*   **小米**

一旦 DotOS 5.1 发布，我们会让你知道。您可以找到它们中每一个的 vanilla 和 Gapps 版本。后者已经包含了 Google apps，所以你不需要刷新一个单独的 ZIP 文件来获得谷歌 Play 商店。

* * *

如果你有兴趣帮助 DotOS 团队进行开发，那么就去看看他们的 GitHub 库。如果你想了解来自团队的最新消息和新发布，你应该考虑在[推特](https://twitter.com/dotosofficial)上关注他们。