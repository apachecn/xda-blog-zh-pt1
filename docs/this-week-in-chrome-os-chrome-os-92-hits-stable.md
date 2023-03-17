# 本周 Chrome OS: Chrome OS 92 稳定上市

> 原文：<https://www.xda-developers.com/this-week-in-chrome-os-chrome-os-92-hits-stable/>

对于 Chrome OS 和谷歌来说，这是相当忙碌的一周。谷歌通过正式预览即将推出的 Pixel 6 和 Pixel 6 Pro 智能手机拉开了本周的序幕。虽然这不是 Chrome OS 的直接新闻，但谷歌制造的张量芯片可能会对 Chromebooks 产生未来影响。在本周中期，Chrome OS 92 终于进入了稳定渠道，带来了一系列新功能。美国电话电报公司还在其网站上发布了 LTE 版本的 Galaxy Chromebook Go 进行销售。

除了所有的最新消息，即将推出的 Chrome OS 功能也有令人鼓舞的发展。Chromebooks 将很快在 dock 中获得原生谷歌日历支持。Debian 11“牛眼”即将推出 Chromebooks，现在可以在某些设备上使用。Chrome Unboxed 的人也能让 Vulkan 游戏在 Chrome OS Canary 94 上运行。让我们更详细地看一下所有的东西。

## Pixel 6 和 Pixel 6 Pro 采用了谷歌的张量芯片

周一，我们都被谷歌宣布 Pixel 6 和 Pixel 6 Pro 的惊喜惊醒。从谷歌获得关于 Pixel 手机的官方“泄露”是相当常见的，但我们没想到会这么早。我们已经知道 Pixel 6 系列将运行谷歌的新定制 SoC。现在[我们知道了这个 SoC 的名字，称为张量](https://www.xda-developers.com/google-pixel-6-teaser/)。

鉴于谷歌在他们的机器学习平台中使用张量这个词，这个名字很有意义。这些手机不是 Chrome OS 设备，但谷歌硅的潜力预示着内置张量芯片的 Pixelbook 的可能性。苹果已经开始将其 Macbook 系列过渡到所有内部芯片的过程，谷歌也可以轻松做到这一点。Pixelbook Go 已经是我最喜欢的 Chromebooks 之一了。续集中的谷歌张量芯片可能会使性能和与 Chrome OS 的集成更好。

## Chrome OS 92 冲击稳定通道

本周最大的 Chrome 新闻无疑是 [Chrome OS 92 冲击稳定频道](https://www.xda-developers.com/chrome-os-92-update/)。更新中的一些关键功能包括 Chrome OS 上更好的视频通话、eSim 支持和新的表情选择器。如果你像我一样喜欢生活在边缘，这些功能中的一些已经在 Canary、Developer 和 Beta 通道中提供了相当长的时间。仍然很高兴看到谷歌研究了很长时间的实验慢慢稳定下来。

显然，改进视频通话现在是一件大事，因为许多人仍然在家工作。eSim 支持的增加令人兴奋，或许这意味着我们将在不久的将来迎来 LTE 甚至 Chromebooks 的涌入。

Chrome OS 92 stable 还附带了一些其他漂亮的标志。其中最有用的是:

**chrome:flags # enable-input-noise-cancellation-ui**

如果你在 Chromebook 上使用外置麦克风，这可以消除输入噪音。对于我们这些制作教程视频或录制播客的人来说，这是添加到 Chrome OS 的一个很好的功能。

## Galaxy Chromebook 现已在美国电话电报公司上市

上周我们提到 Galaxy Chromebook Go LTE 即将推出，现在它已经上市。本周，美国电话电报公司将该设备放在他们的网上商店出售。据推测，这款设备不会在实体零售店出售，很可能只在网上销售。

在规格方面没有太多惊喜，但价格至少让我震惊。这款 Chromebook 的 LTE 版本售价为 349 美元，相当合理。我估计 WiFi 版本至少会涨价 100 美元。如果您从 AT & T 购买并捆绑一个合格的数据套餐，您还可以减去购买价格[的 50%。数据套餐每月 20 美元，但你仍然可以花 175 美元购买硬件，这很划算。](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU4003/https://www.att.com/buy/tablets/samsung-galaxy-chromebook-go-32gb-silver.html)

## Chromebooks 获得原生谷歌日历支持

认为 Google Calendar 没有从一开始就被直接烤进 Chrome OS 是很疯狂的。但是，我们都知道谷歌做出了一些奇怪的选择。令人欣慰的是，谷歌日历似乎终于要登陆 Chrome 操作系统了。

最初是在 Chrome Story 的 Chromium Gerrit 中发现的，[这一提交](https://chromium-review.googlesource.com/c/chromium/src/+/3072882)表明该功能将类似于 Windows 系统托盘中的日历集成。您还可以使用键盘快捷键 *Alt+Shift+C* 来启动日历视图小部件。启用日历小部件的实验标志要到 Chrome OS 103 才会过期，所以我们可能需要等待一段时间才能进入稳定通道。

## Debian 11 即将登陆 Chrome 操作系统

如果你在 Chromebook 上使用 Linux，你可能知道 Chrome OS 上的底层容器是基于 Debian 的。截至目前，Debian for Chrome OS 的最新版本是代号为“Buster”的 Debian 10。随着 Chrome OS 上 Debian 11“牛眼”的到来，这种情况似乎很快就会改变。

Chrome Unboxed 的 Gabriel Brangers 在 Canary channel 上玩着一台 Tiger Lake Chromebook(我猜是华硕 Chromebook CX9 ),注意到现在有一个标志可以在 Chromebook 上启用 Debian 11。这带来了一些内核改进，也带来了在 Chromebook 上运行 Vulkan 游戏的可能性，这恰好是我们的下一个主题。如果你不是一个 Linux 超级用户，你不会注意到从 Buster 到 Bullseye 的很大区别，但这对 Chrome OS 粉丝来说是令人兴奋的事情。

## 克洛斯蒂尼的 Vulkan 游戏现在是一件事了

正如我在本专栏中多次提到的，Steam gaming 可能会在今年晚些时候登陆 Chrome OS。让 Steam 游戏在 Chromebooks 上运行的最重要的一步是 Vulkan 支持。

在周五的一篇帖子中，Chrome Unboxed [的 Luke Short 详细描述了他在 Crostini](https://chromeunboxed.com/eureka-playing-vulkan-games-in-crostini/) 运行 Vulkan 游戏的努力。这样做的细节是相当技术性的，他显然欺骗了他的 Chromebook Pixel 2，使其认为这是华硕 CX9，以使事情正常工作。

这一发展的结果是，我们似乎离 Chrome OS 上的官方 Steam 支持越来越近了。Borealis 应该会彻底改变人们对 Chromebook 游戏的看法。很有可能 Chrome OS 94 上的 Vulkan 会有更广泛的公开测试标志，以及前面提到的 Debian 11 支持。

这星期就这些了。总的来说，对于 Chrome OS 或者整个谷歌的粉丝来说，这是非常棒的一周。我们即将推出游戏 Chromebooks、今年秋天的 Pixel 6 和 Pixel 6 Pro，以及更多有趣的东西值得期待。我的华硕 Chromebook CX9 评测完成并提交，期待下周上线。如果你想在这一周和我聊聊 Chrome OS 和 Android 的所有事情，[在 Twitter 上关注我](http://twitter.com/jspring86az)。