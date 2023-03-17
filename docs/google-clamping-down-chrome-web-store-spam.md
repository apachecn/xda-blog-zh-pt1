# 谷歌取缔 Chrome 网上商店的垃圾邮件和安全问题

> 原文：<https://www.xda-developers.com/google-clamping-down-chrome-web-store-spam/>

# 谷歌正在打击 Chrome 网络商店的垃圾邮件和安全问题

谷歌正在为 Chrome 网络商店制定新规则，这可能会减少来自扩展的垃圾邮件，并保护开发者的账户。

谷歌在 Chrome 网络商店和 Play 商店上遇到的问题几乎一样多。这家商店既有 Chrome 网络浏览器的扩展，也有传统的 Chrome“应用”(其中一些比书签好不了多少)，多年来一直存在许多与恶意软件和不可信任的开发者有关的问题。谷歌现在开始对 Chrome 网上商店开发者实施一些额外的规则，这应该会减少垃圾邮件和一些安全问题。

谷歌在给 Chrome 网络商店开发者的一封电子邮件中表示，“多年来，我们对产品和政策进行了大量改进，以帮助确保人们在 Chrome 网络商店上安装扩展时感到安全。作为这项工作的一部分，我们更新了最佳实践，并命名了安全和信任等关键领域的不良行为。今天，我们进一步澄清了三项政策，以保持高质量的扩展，并为开发人员提供一致的体验。”

新政策主要是为了减少欺骗性策略。不允许在同一个安装流程中提供多个扩展，并且扩展不能追加销售其他扩展或应用。例如，有害的扩展可能会提示您安装不同的扩展，因此如果您删除了第一个扩展，您可能不会想到也删除第二个扩展(这可能会继续收集数据或其他有害的做法)。谷歌还禁止开发者发布“功能、内容和用户体验高度相似”的多个扩展。

最后，Chrome 网络商店开发者需要在他们的谷歌账户上启用两步验证。这应该会减少开发者账户被黑客攻击的情况，这反过来会允许黑客提交对现有扩展的恶意更新(或将扩展的控制权转移到另一个谷歌账户)。谷歌刚刚[为 Google Play 开发者](https://www.zdnet.com/article/google-play-developer-accounts-to-require-2fa-and-a-physical-address/)制定了同样的规则，Mozilla 在今年三月开始要求 Firefox 插件开发者使用双因素认证[。](https://blog.mozilla.org/addons/2021/03/11/two-factor-authentication-required-for-extension-developers/)

### 原始电子邮件

亲爱的开发者:

我们宣布了一系列政策说明，旨在更好地定义现有政策并解决新形式的滥用。

多年来，我们已经对产品和政策进行了大量改进，以帮助确保人们在 Chrome 网上商店安装扩展时感到安全。作为这项工作的一部分，我们更新了最佳实践，并命名了安全和信任等关键领域的不良行为。今天，我们将进一步阐明三项政策，以保持高质量的扩展，并为开发人员提供一致的体验:

**欺骗性安装策略更新:**

1.  不允许在同一个安装流程中提供多个扩展。同样，扩展不能中断其他扩展或应用的追加销售。此类行为违反了我们的欺骗性安装策略和通知滥用政策。
2.  扩展承诺的功能集必须以透明的方式清楚地陈述。你的扩展的所有主要的和重要的特征必须对用户是清楚的，而不是隐藏在不相关的文本中。
3.  任何用户交互的结果都应该符合用户设定的合理预期。
4.  不允许要求不相关的用户操作来访问广告功能。

**垃圾邮件和重复内容:**

1.  具有高度相似的功能、内容和用户体验的多个扩展被认为是重复的。如果这些扩展的内容量都很小，并且提供相同的单一目的，开发人员应该创建一个聚合所有内容的扩展。例如，禁止发布多个壁纸扩展，而这些扩展作为单个扩展会更好。

**两步验证:**

1.  为了发布新的扩展或更新现有的扩展，开发者需要为他们的 Google 帐户启用两步验证。关于如何启用两步验证的说明可在[这里](https://notifications.google.com/g/p/AD-FnEy2SxTQLXgMeuro0CLAIaEGyqsYTeEOT5P7AiSVilp74OyI4Pp5MFJeGoM7V4cQih-iOjpLZEzScuVcPgn9_LD3xLdrOHGtPsDdG0MXw52RAtQqtl-dSbKSp4ILAesyx0GIO5A9c2-FW5iPMRHeHZw6BbvdlwhK8m36)找到。

开发者还可以在我们的[计划政策](https://notifications.google.com/g/p/AD-FnEwRLAgbzl5Gu09AlSI6dVlO82FdbFkakE_qrAQpEB78etbfZGPlJ75yS5jp9VI_TIxrhPqv2vWG827fccXzM4J2MSR6SS-gH_Grq0jsUkE7wKsQX_dNJReJrfJ9IfbSbWw)和我们的[常见问题](https://notifications.google.com/g/p/AD-FnEwE1Nwz30mNWxCF4s2ZSCV8o-advysp2oQ2d2A72GKBX9_ZrVZHfd-fmCWYQYyC9EXSzsBj0WooWhkN2Livb8RlK-dRMkBg31Sj6Pa3E24riVv6fWVsDftF)中了解更多关于今天的指南。这些政策说明将于 2021 年 8 月 2 日生效。在该日期之后，开发者将无法发布新的或更新现有的扩展，除非启用两步验证，并且违反这些新政策的扩展可能会从 Chrome 网络商店中删除并禁用。

如有任何疑问，可[联系开发者支持](https://notifications.google.com/g/p/AD-FnEwuu8HCw223ZpeyylSggBaqFa63tXlOgLLvOFREIw3nxLXXQUfrTfdpSKDd12MpF5hmBtrfj78v8FftY7txJW5u2IFuk3M_S3DN_4HNyBM0xp2ZlUYRGeNE8gxXS4_YdDAAQtFycRLWi03DTgkh1BQ)。

感谢您的合作以及您对 Chrome 扩展生态系统的参与！

-谷歌 Chrome 网络商店团队