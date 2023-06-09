# 自定义内核提高了 ROG 手机 2 和 ROG 手机 3 的刷新率

> 原文：<https://www.xda-developers.com/rog-phone-2-3-boosted-144-165hz-frame-rates-with-custom-kernel/>

华硕的 ROG 智能手机系列在手机游戏玩家中相当受欢迎。通过每一代 ROG 手机，华硕都在继续推进智能手机硬件的边界。最近发布的 ROG 手机 5 就是一个最好的例子，它提供了 6.78 英寸 144Hz AMOLED 显示屏，高通骁龙 888 芯片组，高达 18GB 的内存，总容量为 6,000mAh 的电池，65W 快速充电等等。尽管 ROG Phone 5 是该公司迄今为止最强大的智能手机，但之前的手机，如 ROG Phone II 和 ROG Phone 3，即使在 2021 年仍然保持领先。

这两款手机还享有少数开发商提供的可靠的售后社区支持，这些开发商带来了新的定制 rom、内核和 T2 模块，开启了新的可能性，让用户能够更好地控制他们的设备。例证:XDA 知名开发商 [Freak07](https://forum.xda-developers.com/m/freak07.3428502/) 刚刚发布了 Kirisakura 内核的新更新，允许 ROG Phone II 和 ROG Phone 3 超过其默认的最大显示刷新率。

**警告**:超频设备显示屏的刷新率总会有一些风险。不要将显示器的刷新率提高到超出其正常极限，除非您认为显示器可能会损坏。

对于 ROG 手机 II，开发商已经发布了 Kirisakura v3.2.0，将显示屏超频至 144Hz。120 赫兹是 ROG Phone 2 官方支持的最大刷新率，但看起来显示器能够处理更高的刷新率。从 120Hz 到 144Hz 不会在可感知的平滑度方面产生很大的差异，但那些喜欢从显示器中挤出最后一个 Hz 的人无疑会很高兴。

刷新最新内核版本后，从显示设置中选择 120Hz 模式会将显示设置为 144Hz——您不会看到单独列出的 144hz 模式。虽然将 120Hz 的显示器提升到 144Hz 听起来确实很酷，但开发者警告说，“存在一定的风险”，因为超频刷新率往往就是这样。如果你了解风险，仍然想尝试新的 144 赫兹模式，请点击下面的链接，在那里你会找到所有的说明和相关细节。

**[为你的 ROG 手机下载 Kirisakura 内核 v 3 . 2 . 0 II](https://forum.xda-developers.com/t/kernel-25-03-2021-android-10-kirisakura-3-2-0-for-asus-rog-phone-2-aka-yoda.4028237/page-24#post-84717691)**

**[ROG 手机二论坛](https://forum.xda-developers.com/c/asus-rog-phone-ii.9056/)**

与此同时，ROG 手机 3 的 Kirisakura kernel v2.1.1 将刷新率从默认的 144Hz 提高到 165Hz。我们已经知道华硕正在试验[一个隐藏的 160 赫兹模式](https://www.xda-developers.com/asus-rog-phone-3-hidden-160hz-refresh-rate-mode/?_ga=2.16284723.423813080.1616382540-555576961.1574762426)，它可以通过 ADB 命令激活。然而，Freak07 的定制内核支持略微超频的 165Hz 模式，与最近的[红色魔法 6](https://www.xda-developers.com/red-magic-6-series-china-launch/) 相匹配。不过，在你刷新新的内核 zip 之前，你首先需要使用 ADB 命令激活隐藏的 160Hz 模式——你可以通过遵循[我们的指南](https://www.xda-developers.com/asus-rog-phone-3-hidden-160hz-refresh-rate-mode/?_ga=2.16284723.423813080.1616382540-555576961.1574762426)来做到这一点。

如果你有兴趣在你的 ROG 手机 3 上尝试 165 赫兹的模式，看看下面的链接吧。不言而喻，你的智能手机必须有一个解锁的引导程序和一个定制的恢复像 TWRP 安装，以闪存这个定制的内核。

**[下载 Kirisakura 内核 v2.1.1 for ROG 手机 3](https://forum.xda-developers.com/t/kernel-25-03-2021-android-10-kirisakura-2-1-1-for-asus-rog-phone-3-aka-obiwan.4155505/page-10)**

**[【ROG 手机三论坛】](https://forum.xda-developers.com/c/asus-rog-phone-3.11025/)**

除了上述风险，超频显示器刷新率还有一个警告。由于 ROG Phone II 和 ROG Phone 3 支持的所有股票显示模式都是由华硕校准的，这意味着新的超频显示模式尚未经过该公司的专业校准。开发者一直在调整伽马曲线，以提高低亮度下黑暗场景的可见性，并使颜色看起来更自然，但这些变化对一些用户来说可能看起来很奇怪。尽管如此，开发人员表示，他们试图找到一个平衡，并让用户选择股票校准和他的。

*特色图片:以 160Hz 刷新率运行的华硕 ROG 手机 3*