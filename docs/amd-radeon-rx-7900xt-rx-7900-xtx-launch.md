# AMD 推出镭龙 RX 7900 XT 和镭龙 RX 7900 XTX，价格分别为 899 美元和 999 美元，这是世界上第一款小芯片游戏 GPU

> 原文：<https://www.xda-developers.com/amd-radeon-rx-7900xt-rx-7900-xtx-launch/>

经过几个月的泄露和热切的期待，它终于来了。今天早些时候，AMD 在拉斯维加斯的 RDNA 3 技术活动上发布了镭龙 RX 7900 XT 和镭龙 RX 7900 XTX 旗舰 GPU。RDNA 3 对世界各地的游戏玩家来说都是极其令人兴奋的，这不仅是因为持续的短缺和 Nvidia GeForce 4090 的安全问题，还因为 RDNA3 独特的硬件和软件功能组合被 7000 系列所利用。

请继续阅读，了解您需要了解的关于即将推出的镭龙 7900 txt 和镭龙 7900XT 的一切，包括定价、可用性、技术进步和性能。

## AMD 镭龙 RX 7900 XTX 价格，性能和可用性

让我们从与各地游戏玩家最相关的因素开始:价格和可用性。AMD 镭龙 RX 7900 XTX GPU 的价格为 999 美元，将于 2022 年 12 月 12 日上市。这包括第一方卡和 AMD 的插件板合作伙伴(AIB)的卡。

虽然花一千美元买一个新的显卡对于主流游戏玩家来说肯定是遥不可及的，但对于你所得到的东西来说，价格实际上是相当合理的。根据 AMD 的内部测试(我们将在即将到来的第一手审查中验证这一点)，镭龙 RX 7900 XTX 提供了真正的旗舰级速度，与即将推出的 6950 XT 相比，传统光栅工作负载的性能高达 1.7 倍，光线跟踪的性能高达 1.8 倍。

那么它是如何到达那里的呢？镭龙 7900 XTX 是一个大规模的基于小芯片的 GPU，具有 96 个计算单元，运行在 2.3 GHz 游戏时钟(去耦)，并由 384 位内存总线上的 24GB gddr 6 内存支持。由于 RDNA3 是基于小芯片的，AMD 能够将 TSMC 最先进的 5 纳米节点用于主图形计算芯片(GCD)，同时将 TSMC 更强大、更注重价值的 6 纳米节点用于 6x 内存高速缓存芯片(MCD)。GCD 包含传统的渲染管道组件，如 FP32 着色器和 ROP，而 MCD 负责无限缓存和 GDDR6 内存控制器。

这些规格和性能数据使镭龙 RX 7900 XTX 在原始光栅性能方面与英伟达的 GeForce RTX 4090 不相上下，但节省了 600 美元的成本。但从字里行间来看，一旦你考虑到实时光线跟踪性能，镭龙 RX 7900 XTX 的表现就没有英伟达的产品那么好了——这在今天的游戏生态系统中越来越重要。AMD 自己引用的数字“高达 1.8 倍”6950 XT 的光线跟踪性能意味着 7900 XTX 可能无法匹配英伟达的上一代 RTX 3090，更不用说当前一代 RTX 4090 了。

然而，如果你最关心电子竞技等传统光栅化游戏的高帧速率，7900 XTX 将是一个难以击败的包。换句话说，镭龙 RX 7900 XTX 正在成为价格低于 1000 美元的传统光栅工作负载最快的显卡。

## AMD 镭龙 RX 7900 XT 价格、性能和可用性

尽管 7900 XTX 令人印象深刻，但并不是每个人都有 999 美元来购买显卡。幸运的是，AMD 还推出了它的小弟弟，镭龙 RX 7900 XT。**镭龙 RX 7900 XT 售价 899 美元**，比 7900 XTX 便宜 100 美元，将于 2022 年 12 月 12 日上市。

镭龙 RX 7900 XT 缺少什么？不多。再往下一层，你得到 84 个计算单元而不是 96 个，在 320 位总线上得到 20GB 的 GDDR6 而不是 384 位总线上的 24GB。此外，时钟从 2.3GHz 降至 2.0GHz，但你显然可以使用第三方软件对你的卡进行超频，以弥补差异。考虑到内核数量和时钟数量的减少，当两者都处于库存速度时，XT 看起来只有 XTX 的大约 76%的原始计算能力。但这是否会转化为 24%的游戏性能差异还有待观察。然而，人们可以合理地假设，由于启用的 Cu 较少，当两者都被推到极限时，7900 XT 可能比 XTX 有更多的超频空间。

无论各部分之间的性能差异如何，镭龙 7900 XT 都将成为那些重视传统光栅工作负载高性能的用户的绝佳选择。但如果是给自己买，我会连续几周晚饭吃拉面(农心黑，拜托？)并节省额外的 100 美元来购买 XTX。

## 镭龙 RX 7900 XTX 不需要一个新的 PSU，它不会烧毁你的房子

镭龙 RX 7900 XTX 和镭龙 RX 7900 XT 准备提供非凡的性能和有吸引力的价格，但这还不是全部。它们都由两个传统的 8 针 PCI-Express 电源连接器供电。是的，你没看错，你不需要一个新的 PSU，你也不用担心那些目前困扰 GeForce RTX 4090 的 12VHPWR 适配器。由于这些卡仅由两个 8 针连接器供电，7900 XTX 和 7900 XT 的主板总功率分别仅为 355 瓦和 300 瓦。

还有很多要谈的，但我们今天只允许谈这么多。也就是说，我们将在未来的内容片段中为您提供所有关键细节，因此请关注 XDA 门户网站，了解所有最新的 RDNA3 新闻。

*哪款 RDNA3 GPU 最让你心动？如何看待 7900 txt 和 7900XT 叠加到英伟达的 RTX 4090 和 4080？AMD 配备了 2x 8 针电源连接器，而不是 12VHPWR 插头，您是否和我们一样松了一口气？请在下面的评论中发表意见！*