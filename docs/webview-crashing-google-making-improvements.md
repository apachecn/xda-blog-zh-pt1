# 谷歌解释了为什么 WebView 上个月一直崩溃；详细介绍即将推出的改进

> 原文：<https://www.xda-developers.com/webview-crashing-google-making-improvements/>

# 以下是 WebView 上个月持续崩溃的原因，以及谷歌是如何改进的

谷歌解释了为什么 Android 系统 WebView 上个月导致应用崩溃，以及该公司计划如何在未来避免此类问题。

上个月末，谷歌发布了一个错误的 Android 系统 WebView 更新，导致许多 Android 应用程序崩溃。这个问题非常普遍，Reddit 和 Twitter 上的大量用户都报告了这个问题。谢天谢地，谷歌通过 Play Store 及时推出了 Android 系统 WebView 和谷歌 Chrome 的更新来解决这个问题，一切都很好。该公司现在分享了一些关于问题实际原因的见解，以及它计划如何进行改进以防止任何未来的灾难。

根据 Google Workspace 团队最近的更新(T1)，这个问题是由“Chrome WebView 的实验配置技术(T7)中的一个*错误造成的。”*它影响了几个流行的安卓应用，包括 Gmail 和亚马逊，这些应用整合了 WebView 来显示网页内容。为了解决这个问题，谷歌通过 Google Play 发布了 Chrome 和 WebView 的更新二进制文件。该公司还在 Android 帮助中心社区论坛上发布了一个[的详细帖子](https://support.google.com/android/thread/103561027)，以帮助受该问题影响的用户。

现在，为了防止未来发生任何类似的事故，谷歌计划改进其对 WebView 系统组件及其依赖项的变更管理和部署政策。为此，公司将采取以下措施:

*   审核 WebView 及其相关依赖项的生产准备情况。
*   实施 WebView“安全模式”,该模式将处理此类配置错误并恢复到已知良好的状态。
*   改进实验的可测试性和推广过程。
*   通过 Play Store 加速 Chrome 和 WebView 的更新机制。
*   在整个事件过程中与我们的用户更好地沟通，并与我们的合作伙伴一起提供关于影响和解决状态的评论。

如果你的 Android 手机仍然面临随机的应用程序崩溃，并且你还没有安装最新的 Chrome 和 Android 系统 WebView 更新，请点击下面的链接立即下载最新的更新。