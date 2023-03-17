# iOS 版 Chrome 现在可以用人脸或触控 ID 锁定匿名标签

> 原文：<https://www.xda-developers.com/chrome-ios-incognito-tabs-face-touch-id-security/>

# iOS 版 Chrome 将为匿名标签带来人脸和触控 ID 安全功能

最新的 iOS 版谷歌 Chrome 测试版包括锁定匿名标签的选项，以及用 Face ID 或触控 ID 解锁的选项。请继续阅读了解更多信息！

如果你想访问敏感网站，同时避免在浏览器历史中留下痕迹，Chrome 上的匿名模式是一个很好的选择。然而，如果你忘记关闭这些标签，就有可能有人拿起你解锁的手机并访问这些匿名标签。为了避免这种情况，谷歌的 Chrome 团队正在为 iOS 用户开发新的隐私功能。在新的测试版更新中，Chrome 现在可以通过 iPhone 的 Face ID 或触控 ID 认证锁定匿名标签。

根据 iOS 89 版谷歌浏览器测试版的发布说明，“你可以通过触控 ID 或 Face ID 为你的匿名标签添加更多的安全性。当你返回应用程序时，你的匿名标签将被模糊化，直到你确认是你。”一旦用户启用了基于 Face ID 或触控 ID 的锁定，Chrome for iOS 将不再让你在没有解锁的情况下看到任何打开的匿名标签。一旦隐姓埋名模式解锁，你将不再需要通过面部或触控 ID 认证，直到浏览器关闭并再次打开。

### 如何在 iOS 版 Chrome 上启用匿名标签隐私认证

新功能仅在最新测试版的 iOS 版 Chrome 上提供。这意味着你需要首先安装测试版来替换你设备上现有的 Chrome 版本。

*   要获得 Chrome 测试版，请在你的 iOS 设备上安装[苹果的 TestFlight iOS 应用](https://apps.apple.com/us/app/testflight/id899247664)。
*   访问 Chrome Beta 版的[试飞邀请](https://testflight.apple.com/join/LPQmtkUs) URL
*   同意许可协议并安装测试版。
    *   如果你收到通知说测试版已经满了，你可能要等到谷歌的 Chrome 测试网站有新的邀请。
*   iOS 89 应用安装测试版后，在地址栏输入 *chrome://flags* ，搜索‘隐姓埋名的设备认证’并启用标志。

*   关闭并重新打开应用程序
*   进入“设置”>“隐私”,启用“关闭 Chrome 时锁定匿名标签”
*   如果您想禁用此功能，请返回到 *chrome://flags* 并禁用设置。

截至目前，Android 用户还没有这种安全功能。但考虑到该功能正在测试中，我们应该很快就会看到它在 Android 版本的 Chrome 浏览器中出现。

Chromium 开发者还在桌面版 Chrome 上试验[不同宽度的标签，当标签滚动功能(也在测试中)开启时。这个特性使得当你一次打开多个标签时，你的标签栏看起来不那么拥挤。Firefox 和 Safari 有类似的功能，所以很高兴看到谷歌在其浏览器上效仿。](https://www.xda-developers.com/google-chrome-tab-width-tab-scrolling/)