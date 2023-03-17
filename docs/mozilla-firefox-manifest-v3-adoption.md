# Mozilla 分享了它计划如何在 Firefox 中实现清单 V3

> 原文：<https://www.xda-developers.com/mozilla-firefox-manifest-v3-adoption/>

Mozilla 透露了它计划如何在 Firefox 中采用 Manifest V3。该公司表示，到 2022 年底，Firefox 将全面拥抱下一代网络扩展平台，在此之前，它将推出一个新的开发者预览计划，以收集网络开发者的反馈。

## 什么是清单 V3？

Manifest V3 是 web 扩展平台的最新变化，使扩展更加安全、快速和隐私友好。它是由谷歌在 2019 年首次宣布的，我们已经详细讨论了新版本中提出的各种[大变化和围绕它的争议](https://www.xda-developers.com/google-chrome-manifest-v3-ad-blocker-extension-api/)。清单 V3 中最有争议的变化之一是移除了 Web 请求 API，而支持新的声明性 Net 请求 API。开发人员社区广泛批评了这一变化，因为它剥夺了许多有用的扩展功能，使它们效率更低。谷歌 Chrome 已经[停止接受基于 V2 清单](https://www.xda-developers.com/chrome-99-beta-features/#:~:text=Chrome%2099%20beta%20also%20introduces%20changes%20related%20to%20ad%20blockers.%20Starting%20with%20Chrome%2099%2C%20Google%20no%20longer%20allows%20new%20ad%20blocker%20extensions%20to%20use%20Manifest%20V2.)的新扩展，而现有的 V2 清单扩展[将在 2023 年 1 月](https://www.xda-developers.com/google-chrome-manifest-v3-transition-details/)后停止工作。

## Mozilla 希望以不同的方式做事

Mozilla 表示，它意识到了 Manifest V3 中提出的一些有争议的变化及其对广告拦截器和其他扩展的严重影响。为此，Mozilla 表示，它将采用与谷歌 Chrome 不同的方法来实现 Manifest V3。Mozilla 认为新的声明式网络请求 API 并不是 WebRequest API 的完美替代品，限制了广告拦截器和隐私扩展的范围。因此，Firefox 将在清单 V3 中保留对“阻止 WebRequest”的支持，同时还支持 *DeclarativeNetRequest* 。

“Mozilla 将继续支持在 MV3 屏蔽 WebRequest。为了最大限度地兼容其他浏览器，我们还将提供对 declarativeNetRequest 的支持。Mozilla 高级软件工程师 Rob Wu 写道:“我们将继续与内容拦截器和该 API 的其他主要消费者合作，以确定当前和未来合适的替代方案。

Mozilla 也不喜欢 Chrome 使用的*后台服务工人*，因为它不支持许多用例，并且要求开发人员重写大部分扩展代码。Mozilla 去年提出了事件页面来解决这些缺点，它说这已经得到了社区的好评，并将在 Firefox 的 Manifest V3 实现中得到完全支持。Mozilla 表示，出于兼容性原因，它也将支持*服务人员*，因为“我们喜欢他们是一个事件驱动的环境，具有定义的生命周期，已经是具有良好跨浏览器支持的网络平台的一部分。”

“在 Firefox 中，我们已经决定在 MV3 支持事件页面，我们的开发者预览版将不包括服务人员(我们将继续努力在未来的版本中支持这些)。这将有助于开发人员更轻松地迁移现有的持久后台页面，以支持 MV3，同时保留对 MV2 中所有 DOM 相关功能的访问。”

* * *

**来源** : [Mozilla 博客](https://blog.mozilla.org/addons/2022/05/18/manifest-v3-in-firefox-recap-next-steps/)