# 谷歌将开始在桌面浏览器中测试更快的页面导航

> 原文：<https://www.xda-developers.com/google-chrome-desktop-back-forward-cache/>

谷歌去年在 Android 平台的 Chrome 上推出了一项新功能，叫做后退-前进缓存，旨在提高使用后退和前进按钮时的性能。回退缓存在您返回后将页面保存在内存中一段时间，因此如果您需要返回到最近的页面，加载时间是即时的。这一改变似乎是成功的，因为谷歌已经开始在桌面平台上进行测试。

2020 年 10 月发布的谷歌 Chrome 86，[增加了一个在桌面平台手动启用后退-前进缓存的功能标志。在那之前，该功能只在 Android 上可用。谷歌现在已经在谷歌群组上](https://www.xda-developers.com/google-chrome-86-rolls-out-with-flags-for-menu-icons-back-forward-cache-and-more/)[发布了一个“意图实验”页面](https://groups.google.com/a/chromium.org/g/blink-dev/c/GJsdwulsGiI/m/7OauT6SjBQAJ?pli=1)(通过 *Windows 最新* 发布[)，解释说该功能现在将在少量桌面 Chrome 用户中进行测试。如果一切顺利，该功能最终将为所有人打开。](https://www.windowslatest.com/2021/05/13/google-chrome-load-pages-faster-on-desktop-using-back-forward-cache/)

“为了降低兼容性风险，”Chrome 的开发人员在帖子中说，“当面临不确定性时(例如，当页面使用 WebSocket 这样的非平凡 API 时)，我们将从不缓存页面的谨慎方法开始。对于存储在双向缓存中的页面，面向开发人员的唯一主要区别是 unload()处理程序不会触发。然而，这与 Safari 的行为是一致的，它应该会将 compat 风险降至最低。”

谷歌没有提到为什么这项功能这么长时间以来一直只在手机上使用，但延迟可能是由于内存使用。Chrome 经常因其在桌面平台上的高内存使用率而受到批评，冻结更多页面可能不会有所帮助。然而，谷歌和微软一直致力于其他的改变，以减少 Chromium 引擎的内存使用，所以回退缓存的成本在这一点上不太明显。谷歌去年还在 T2 表示，浏览器扩展会给桌面平台增加额外的复杂性，因为它们中的许多会对当前页面的变化做出反应。

谷歌将随着 Chrome 92 的发布开始测试，预计 Chrome 92 将于 6 月 3 日进入测试版，7 月 20 日稳定发布。