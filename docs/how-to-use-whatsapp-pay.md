# 如何设置 WhatsApp Pay 收发钱

> 原文：<https://www.xda-developers.com/how-to-use-whatsapp-pay/>

在经历了艰难的起步之后，WhatsApp 的支付功能现在已经在印度和其他受支持的市场广泛提供，这标志着这家脸书公司向前迈出了一大步，因为它希望扩展其通讯功能之外的领域，并准备利用电子商务机会。以下是你需要知道的关于 WhatsApp 雄心勃勃的支付功能的一切。

## 背景——漫长的探索

WhatsApp 寻求在印度推出支付服务可以追溯到 2018 年。2018 年 2 月，WhatsApp 获得了印度国家支付公司(NPCI)的批准，对其支付服务进行测试，该公司向 100 万用户推出了这项服务。

但看似一帆风顺的事情很快就戛然而止，因为该公司卷入了一场旷日持久的监管斗争，这场斗争持续了两年。监管机构提出的要求之一是遵守印度储备银行的[数据存储指南](https://m.rbi.org.in/Scripts/FAQView.aspx?Id=130)，该指南要求所有支付服务提供商(PSP)存储印度境内用户的财务数据。

RBI 要求 NPCI 暂停 WhatsApp Pay 的全面推广，直到该公司满足这些要求。WhatsApp 最初抵制合规性，但意识到没有其他办法，该公司同意遵守数据本地化要求，以获得推广的绿灯。

WhatsApp 任命第三方 CERT-In 审计师德勤(Deloitte)审计其合规性，德勤于 2020 年 5 月 29 日向 NPCI 提交了报告，称 WhatsApp 完全符合 RBI 的数据本地化规范。

NPCI 对这份报告感到满意，随后正式批准 WhatsApp 及其支付服务提供商 ICICI Bank 分阶段在 UPI 上上线，第一批用户最多可达 2000 万。2021 年 11 月，WhatsApp [获得了将服务](https://www.xda-developers.com/whatsapp-pay-approval-expand-40-million/)扩展到另外 2000 万用户的许可。这使得 WhatsApp Pay 的用户总数达到 4000 万，考虑到 WhatsApp 在中国拥有 4 亿多用户，这个数字微不足道。这就把我们带到了下一个问题。

## WhatsApp 的支付功能在我的国家可用吗？

与其他普遍可用的 WhatsApp 功能不同，支付功能目前仅在三个国家可用:印度、美国和巴西。在印度，WhatsApp Pay 使用统一支付接口(UPI)平台，而在巴西，该功能由脸书 Pay 提供支持，由信用卡和借记卡运营商 Cielo 处理支付处理。

在美国，WhatsApp 用户可以通过 Novi 钱包收发钱款[。到目前为止，它只对有限数量的用户开放。Novi 是 WhatsApp 母公司](https://www.xda-developers.com/whatsapp-novi-integration-live-some-users-us/) [Meta](https://www.xda-developers.com/facebook-meta-name/) 的数字钱包。它允许用户通过一种叫做 USDP 的稳定货币转账，这种货币由美元支持(例如 1 USDP 等于 1 美元)。)

WhatsApp 在它的 [FAQ 页面](https://faq.whatsapp.com/payments/set-up/learn-more-about-participating-countries-and-supported-banks/)上提到，它正在*“努力将这一功能带到其他国家”*，但是到目前为止，该公司还没有分享关于在其他市场进一步扩张的具体细节。

## 如何使用 WhatsApp Pay

使用 WhatsApp Pay 的要求非常基本——你只需要最新版本的 WhatsApp 。如果你符合这一要求，请按照以下步骤设置该功能，并开始在 WhatsApp 上发送和接收付款:

*   确保你的手机上安装了最新版本的 WhatsApp 稳定版还是测试版，都没关系。
*   在应用程序中，点击右上角的三点菜单，寻找*支付*选项。
*   即使你在菜单中看到了*支付*选项，也不能保证你的账户激活了该功能。你可能会看到*你现在不能在 WhatsApp 中设置支付*的错误，或者看到一个类似这样的屏幕(在这种情况下，恭喜你，你可以使用这个功能了)。

*   入职流程非常简单。点击*添加支付方式*并从列表中选择您的银行。

*   WhatsApp 将尝试查找并链接与您的手机号码相关联的银行账户。你可能会被要求通过短信验证你的电话号码——这是第一次设置账户时 UPI 应用程序中的一个常见程序。

*   如果链接过程顺利，您现在应该已经准备好通过 WhatsApp Pay 发送和接收资金了。

## WhatsApp 付费体验

使用 WhatsApp Pay 与使用任何其他 UPI 应用程序非常相似，但由于该服务被集成到 WhatsApp 应用程序中，因此它带来了更简化、更整洁的体验。UI 非常干净直观，主要强调对等交易。您还可以选择扫描二维码在商家和企业支付。

它不会取代像 Google Pay 这样的成熟应用程序——例如，你不能支付你的账单——但对于收发资金来说，它可以相当好地完成工作。

如果收款人已经设置了 WhatsApp Pay，汇款就像选择联系号码、输入金额和输入您的 UPI PIN 码一样简单。如果另一方还没有支付功能，你可以选择向他们的另一个 UPI ID 汇款——假设他们使用类似 Google Pay 或 PhonePe 或任何 UPI 的东西。只需要求他们分享他们的 UPI ID，看起来应该类似于 *91XXXXXXXX@okicici* 或< *用户名> @ < bankupi >，*并完成交易。

同样，您也可以通过提供自己的 ID，从其他服务提供商那里将钱存入自己的 WhatsApp Pay UPI ID。但是 WhatsApp 生成的 ID 看起来像是 *<你的电话号码> .wa.xes@icici* ，这不像其他基于用户名的 UPI IDs 那样直观。因此，对拥有 WhatsApp Pay 的发送者和接收者的软“要求”是简化用户名共享过程，并消除这种想法。

将来，在 WhatsApp 中使用一个出现在聊天栏内的专用支付按钮来支付款项会更加容易。

## 展望未来

印度有十几个 UPI 应用程序，WhatsApp 要说服人们一夜之间转向自己的 UPI 并不容易，不管它在易用性和简单性方面有什么优点。这也为脸书多年来一直关注的电子商务机会铺平了道路，也是即时通讯平台货币化的可行方式。

WhatsApp 在印度有着家喻户晓的天然优势。与其他合众国际社的应用程序不同，它不必去寻找新用户，也不必乞求人们在他们的手机上安装另一个合众国际社的应用程序。这款应用已经出现在超过 4 亿台设备上，因此该公司的任务被简化为找出如何推动这些用户养成使用 WhatsApp Pay 的习惯。

尽管有这些优势，WhatsApp Pay 在印度移动支付领域仍然是一个相对不为人知的名字。NPCI 发布的[最新数据显示，WhatsApp 在 2021 年 12 月仅进行了 225 万笔交易。相比之下，沃尔玛旗下的 PhonePe 和 Google Pay 分别处理了 20.7760 亿笔和 15.8743 亿笔交易，分别位居第一和第二。WhatsApp 是否能够扭转局面，成为头号玩家还有待观察。](https://www.npci.org.in/what-we-do/upi/upi-ecosystem-statistics)