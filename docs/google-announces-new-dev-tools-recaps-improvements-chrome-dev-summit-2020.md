# 谷歌宣布新的开发工具，并在 2020 年 Chrome 开发峰会上概述 Chrome 的改进

> 原文：<https://www.xda-developers.com/google-announces-new-dev-tools-recaps-improvements-chrome-dev-summit-2020/>

谷歌正在举办 2020 年 Chrome Dev 峰会，详细介绍这个星球上绝大多数用户选择的互联网浏览器的变化。谷歌对 Chrome 的愿景是让它成为一个安全、强大、快速的互联网接入工具。这篇文章汇集了明年最流行的网络浏览器的愿景中的一些零碎内容。

## 隐私

早在 2019 年，谷歌就宣布了 Privacy Sandbox，这是一项旨在开发一套开放标准的倡议，旨在改善网络隐私。这项工作还在继续，因为谷歌正朝着建立新的隐私保护替代第三方 cookies 和其他跨网站跟踪机制的方向前进。为此，客户机提示 API 是降低用户代理字符串粒度的第一步，以后还会有更多。

Chrome 稳定版的两个新解决方案是点击转化测量 API 和信任令牌 API。前者在不使用跨站点标识符的情况下测量广告转换，而[信任令牌](https://www.xda-developers.com/google-details-trust-tokens-api-alternative-third-party-cookies-web-browsers-chrome/)有助于将信任从一个上下文传递到另一个上下文，而无需被动跟踪。

清单 V3 也在向 Chrome 前进，首先是测试版，然后是稳定分支，从 2021 年 1 月 19 日起，Chrome 网络商店允许更新提交内容。

## 特征

浏览器需要增强网络功能，Chrome 计划通过给网络浏览器添加新功能来做到这一点。Chrome 86 让开发者能够使用可信网络活动在 Play Store 上列出他们的渐进式网络应用(PWA)。现在，开发者可以开始使用 Chrome 88 中新的[标准化数字商品 API 接受支付。](https://www.xda-developers.com/chrome-88-beta/)

## Chrome 和性能

谷歌 Chrome 一直是几个迷因的接收端，经常取笑网络浏览器的资源密集型特性。在这方面，谷歌已经通过今年早些时候披露的[档案引导优化&标签节流](https://www.xda-developers.com/google-chrome-faster-new-tab-pdf-url-sharing-features/)对速度进行了一些关键的改进。

现在，谷歌宣布减少 V8 的内存占用。V8 指针压缩有助于节省内存，它还允许 Google 通过并行加载网页的 JavaScript 文件来完全消除解析暂停，因此脚本可以被解析和编译，并在页面需要时立即执行。

接下来，谷歌在今年早些时候宣布了 [Web Vitals initiative](https://www.xda-developers.com/google-announces-web-vitals-initiative/) ，提出了代表理想用户体验的指标。[谷歌搜索还宣布](https://www.xda-developers.com/google-search-page-experience-ranking/)从 2021 年 5 月开始，搜索排名的新信号将包括核心网站生命体征。很明显，网页活力现在是网页性能指标的一个重要方面。

现在，谷歌宣布推出 Web Vitals Report，这是一个开源网站，是一个让你可以在谷歌分析中查询和可视化 Web Vitals 指标数据的工具，让网络开发人员可以轻松地比较不同细分市场的性能数据。

对于未来，Gooogle 将会把更多的注意力放在弥补构建网络界面的困难上。该公司戏弄了 Houdini.how，这是一组将使 CSS 更容易扩展的 API。

* * *

这概括了今年在线举行的谷歌 Chrome Dev Summit 2020 的所有主要公告。你可以注册 [wed.dev 简讯](http://web.dev/)，而[可以在 YouTube 频道](https://www.youtube.com/watch?v=NkIi7h8NnS4)上观看会议以了解更多细节。