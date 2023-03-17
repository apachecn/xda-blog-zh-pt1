# 由于这些变化，Chrome 91 的性能提高了 23%

> 原文：<https://www.xda-developers.com/chrome-91-23-percent-faster-performance/>

# 由于这些变化，Chrome 91 的性能提高了 23%

谷歌最近在稳定频道推出了 Chrome 91，由于帖子中提到的变化，它的性能提高了 23%。

谷歌[最近在稳定频道推出了](https://www.xda-developers.com/google-chrome-91-stable-rollout/) Chrome 91。此次更新引入了大量更改，包括改进的表单控件、大屏幕设备上的默认桌面模式支持、文件系统访问 API 改进等等。此次更新还带来了大量的性能改进，谷歌现在透露，最新的更新使 Chrome 比以前的版本快了 23%。

在 *Chromium 博客*上的[最近的一篇帖子](https://blog.chromium.org/2021/05/chrome-is-faster-in-m91.html?m=1)中，Chrome 产品经理 Thomas Nattestad 透露，Chrome 91 *现在随着[新斯派克普拉编译器](https://v8.dev/blog/sparkplug)和[短内置调用](https://v8.dev/blog/short-builtin-calls)的推出，速度提高了 23%,每天为我们的用户节省了超过 17 年的 CPU 时间！这篇文章解释说，斯派克普拉是一个新的 JavaScript 编译器，它“填补了需要快速执行和优化代码以获得最高性能之间的空白”。"*另一方面，短的内置调用优化了*"我们将生成的代码放在内存中，以避免调用函数时的间接跳转。”*

Chrome 的 V8 引擎具有多个编译器，这些编译器在执行 JavaScript 的各个阶段做出不同的权衡。新的斯派克普拉编译器在发动机的双层编译器系统(点火和涡轮风扇)之间取得了平衡，以生成本机代码，而不依赖于执行 JavaScript 代码时收集的信息。因此，它*“开始快速执行，同时仍然生成相对较快的代码”*从而提高性能。

Short builtins 是一种新的机制，可以帮助 V8 引擎优化生成代码在内存中的位置。*“当 V8 从 JavaScript 生成特定于 CPU 的代码时，它会将这些代码放在内存中。这些生成的代码将频繁调用内置函数，内置函数是处理常见例程的小代码片段——从添加两个变量这样的基本操作，到 JavaScript 标准库中成熟的函数。对于某些 CPU，调用离生成的代码较远的函数会导致 CPU 内部优化(如分支预测逻辑)失败。解决这个问题的方法是将内置函数复制到与生成代码相同的内存区域。它进一步指出，这一变化应该会提高 Chrome 在苹果 M1 芯片上的性能。*

要了解这些性能升级的更多信息，请查看 Chrome [V8 博客文章](https://v8.dev/blog/sparkplug)。