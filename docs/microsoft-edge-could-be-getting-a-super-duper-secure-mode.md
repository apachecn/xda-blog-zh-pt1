# 微软 Edge 可能会获得一种超级安全模式

> 原文：<https://www.xda-developers.com/microsoft-edge-could-be-getting-a-super-duper-secure-mode/>

是的，你没看错标题。微软正在为其 Edge 浏览器测试一项新的安全功能，至少目前为止，它被称为[超级安全模式](https://microsoftedge.github.io/edgevr/posts/Super-Duper-Secure-Mode/)。SDSM 的目标是通过禁用 JavaScript 的实时(JIT)编译来提高浏览网页的安全性。不过，SDSM 还有其他特色。

JavaScript 是 web 的基础部分，但它也带来了自己的问题，JIT 引擎是其中的一大部分。根据最初发现 SDSM 信息的 [*哔哔声计算机*](https://www.bleepingcomputer.com/news/microsoft/microsoft-edge-just-got-a-super-duper-secure-mode-upgrade/) ，V8 JavaScript 中大约 45%的漏洞与 JIT 引擎有关。微软的 Jonathan Norman 也指出，禁用 JIT 编译“杀死了一半的错误”,攻击者可以利用这些错误在 JavaScript 中进行安全攻击。此外，对于其余的漏洞，这种更小的攻击面至少会使攻击更难实施。

当然，如果禁用 JIT 编译器是所有的好处，这可能已经完成了。JIT 编译存在的原因是它可以显著提高 JavaScript 的性能。然而，微软研究团队表示，当禁用该功能时，实际上并没有看到明显的性能影响。在微软运行的数百个测试中，只有不到十个测试显示禁用 JIT 编译时性能下降。在某些情况下，性能甚至有所提高。然而，在有性能退化的测试中，它们是非常显著的。尽管如此，这使得 Edge 的超级安全模式看起来相当有吸引力。

但这还不是全部。根据微软的说法，让 JIT 保持启用状态，就不可能实现其他有助于安全性的功能。例如，英特尔的控制流执行技术(CET)是一种基于硬件的漏洞缓解技术，必须禁用。在 Edge 的 Super Duper 安全模式下，微软不仅禁用了 JIT 编译器，还启用了 CEF 以获得额外的安全性。微软还计划在未来启用任意代码保护(ACG)——另一件在启用 JIT 编译器的情况下不可行的事情。

微软很清楚这只是一个测试，所以不要期望它会很快成为一个功能。然而，如果你觉得这个想法很有趣，你可以试一试。您可以通过进入 *edge://flags* 在 Edge Beta、Dev 或 Canary 中启用 SDSM。各自的标志被简单地称为*超级骗子安全模式*。