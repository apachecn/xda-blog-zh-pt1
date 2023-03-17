# ARM 宣布推出用于笔记本电脑的 Cortex-A78C CPU，最高可配 8 个大内核

> 原文：<https://www.xda-developers.com/arm-cortex-a78c-cpu-core-announcement/>

5 月，ARM 宣布了其最新的移动 IP，包括 Cortex-A78 CPU、Mali-G78 GPU 和 Ethos-N78 NPU。该公司还宣布了其 [Cortex-X 定制(CXC)计划](https://www.xda-developers.com/arm-announces-cortex-x-custom-cpu-program/)，Cortex-X1 是该计划下的第一个 CPU 核心。该计划允许在 ARM Cortex 产品的传统路线图之外进行定制和差异化。该公司表示，这一代基于 ARM 的处理器取得了巨大成功，并迅速扩展到传统手机以外的市场。现在，该公司正在寻求通过其最新的 CPU 产品 Cortex-A78C 来解决其中一些市场。

ARM Cortex-A78C CPU 是在常规 Cortex-A78 的基础上构建的新 CPU。 [ARM 表示](https://community.arm.com/developer/ip-products/processors/b/processors-ip-blog/posts/arm-cortex-a78c)它是专为下一代移动设备(如始终在线的笔记本电脑)打造的可扩展且安全的计算解决方案的一部分。Cortex-A78 系列包括用于智能手机的常规 Cortex-A78，用于复杂自主应用的 Cortex-A78AE，以及现在用于笔记本电脑的 Cortex-A78C。Cortex-A 系列的价值在于 PPA(性能、功耗和面积)。Cortex-A78C 以这些设计为基础，采用最新的架构更新来增强计算性能、可扩展性和安全性。

Cortex-A78C 的主要特点是支持多达八个大 CPU 核心集群，从而实现更同质的多大核心计算。与常规 Cortex-A78 相比，八核(多达八个大 CPU 内核)可带来更可扩展的多线程性能提升，常规 Cortex-A78 在 DynamIQ 共享单元(DSU)中仅支持四个大 CPU 内核和四个小 CPU 内核(以 Cortex-A55 的形式)。手臂纸币那么大。在移动领域，几乎没有什么事实上的标准，未来也将如此。Cortex-A78C 的八核配置将带来更高的多线程性能，这对于要求苛刻的工作负载来说是一个优势。Cortex-A78C 还将 L3 缓存增加到 8MB，以进一步提高性能，尤其是对于具有大型数据集的工作负载。

ARM 表示，这些增强功能非常适合支持高性能、多线程工作负载，例如游戏中的物理和专业生产力应用。根据 ARM 的说法，八个核心配置在与 Mali GPUs 结合时进一步扩展和增强了全天游戏功能，Mali-G78 提供了图形性能和电池续航时间的改进，以获得更加身临其境的移动游戏体验。另一方面，增加的三级高速缓存将使开发人员能够为下一代设备带来增强的游戏体验，如 AAA 游戏。

Cortex-A78C 还提供数据和设备安全更新。ARM 指出了指针认证(PAC)功能，该功能可以最大限度地减少攻击面，以确保设备上的数据安全。该公司指出，复杂的计算机攻击利用了面向返回编程(ROP)和面向跳转编程(JOP)中的小工具。PAC 显著减少了漏洞利用，并防止攻击者控制软件控制流，从而使 ROP 漏洞利用减少了 60%以上，JOP 漏洞利用减少了 40%以上。ARM 表示，减少这些潜在的漏洞是必要的，以确保用户的数据在设备上保持安全，即使安装了第三方应用程序。

总之，ARM 表示，虽然 Cortex-A78 是下一代手机的移动核心，但 Cortex-A78C 的新功能提供了下一代移动设备所需的性能、可扩展性和安全性

ARM 发布 Cortex-A78C 非常及时，因为据传苹果硅动力 MAC 电脑将于 11 月 10 日在苹果的在线活动上发布。对于高通来说，这一声明可能来得正是时候。在 12 月的技术峰会上，该公司可能会宣布用于永远在线个人电脑的[骁龙 8cx](https://www.xda-developers.com/qualcomm-snapdragon-8cx-always-on-always-connected-pc/) SoC 的继任者，该 SoC 是近两年前推出的，配有四个 ARM Cortex-A76 大内核。迁移到八个 Cortex-A78C 内核以及 Adreno 680 的继任者将提供相当大的性能提升。