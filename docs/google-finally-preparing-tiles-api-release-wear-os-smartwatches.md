# 谷歌正准备为 Wear OS 发布官方 Tiles API

> 原文：<https://www.xda-developers.com/google-finally-preparing-tiles-api-release-wear-os-smartwatches/>

**更新 1(01/26/2021 @ 06:10PM ET):**Google 已经合并了实现 Wear OS Tiles API 的提交。[点击这里了解更多信息。](#update1)文章发表于 2020 年 12 月 18 日，下面保留。

2019 年，[谷歌发布了“Tiles”](https://www.xda-developers.com/google-wear-os-tiles-feature/)，这是一个新功能，可以让你在 Wear OS 智能手表上显示小的、信息丰富的应用程序 widget 卡片。谷歌为一些事情添加了磁贴，包括目标、下一场比赛、预测、心率、头条和计时器，允许用户通过在表盘上向左滑动来轻松访问重要信息。在发布时，你只能添加 5 个磁贴，但在 Wear OS 应用 v2.40 中，谷歌提高了限制，允许用户在智能手表上添加多达 10 个磁贴。自从 Tiles 发布以来，像 Mobvoi 这样的智能手表 OEM 厂商也建立了自己的 Tiles。

然而，时至今日，谷歌从未发布官方的磁贴 API，让第三方 Wear OS 应用开发者提供自己的磁贴。受够了这种延迟，一些开发人员[对谷歌在 Wear OS 应用中使用的内部 Tiles API](https://www.xda-developers.com/wear-os-unofficial-tiles-api/) 进行了逆向工程，以创建一个非官方的 leAPI。虽然这已经导致一些第三方应用程序开发人员成功地创建了磁贴，但不建议依赖未记录的 API，因为它们可能随时发生变化，从而导致破损。但在不久的将来，开发商似乎将不必诉诸非官方的方式来建造瓷砖。

最后，在 Tiles 首次亮相近一年半之后，看起来 Google 正准备推出一个官方的 Tiles API。一个名为[“磨损瓦片 API 的初始提交”](https://android-review.googlesource.com/c/platform/frameworks/support/+/1531917)的 AOSP 提交将瓦片 API 添加到 AndroidX 支持库。

*耐磨砖 API 的初始提交。*

*这将检查耐磨瓷砖 API 的应用程序端。测试(和测试库)还没有被添加，但是会在未来的 CL 中出现。这个版本的存在实际上是为了开始 API 审查。*

一旦这个提交被合并，开发者将能够在更新到最新的 AndroidX 版本后调用这个 API。

随着官方 Tiles API 的发布，我们应该会看到更多的开发者加入进来，为 Wear OS 驱动的智能手表带来令人兴奋的新 Tiles。我们不知道谷歌计划何时公开发布该 API。但是我们会密切关注事态的发展，如果有新的消息，一定会让你知道。

* * *

## 更新 Wear OS Tiles API 的初始提交已合并

现在，实现 Wear OS Tiles API 的初始[提交](https://android-review.googlesource.com/c/platform/frameworks/support/+/1550775)已经合并(h/t @[kevinlife 2](https://twitter.com/kevinslife2))，用不了多久，开发者就可以正式将 Tiles 添加到他们的 Wear OS 应用中了。然而，谷歌尚未进行 API 测试，因此该公司可能不会在 [Wear AndroidX Jetpack 库](https://developer.android.com/jetpack/androidx/releases/wear)中立即提供该 API。一旦这篇文章正式发布，我们会及时更新。