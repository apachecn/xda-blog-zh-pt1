# 英特尔从 Arc 和 Xe 图形中撤销对 DirectX 9 的原生支持

> 原文：<https://www.xda-developers.com/intel-withdraws-native-support-for-directx-9-from-arc-and-xe-graphics/>

英特尔期待已久的 Arc GPU 终于来了，但同时也给老游戏的粉丝带来了一些消息。看起来英特尔将不再支持 Arc 和 Xe 专用 GPU 上的 DirectX 9 (DX9)和第 12 代处理器上的集成显卡。

据 *The Verge、* [报道，英特尔已经悄悄宣布](https://www.intel.com/content/www/us/en/support/articles/000091238/graphics.html)它将从 Arc 和 Xe 上对 DX9 的硬件支持切换到 DirectX 12 (DX12)的模拟支持。

> 第 12 代英特尔处理器的集成 GPU 和 Arc 离散 GPU 不再原生支持 D3D9。基于 DirectX 9 的应用和游戏仍然可以通过 Microsoft* D3D9On12 接口工作。

这到底意味着什么？理论上什么都没有，至少目前是这样。它所做的是立即将 DX9 支持的责任从英特尔转移到微软，因此，任何支持问题。 [D3D9On12 在 GitHub](https://github.com/microsoft/D3D9On12) 上列出，供想了解更多的人参考。不会有专门的驱动程序支持剩下的流行 DX9 游戏，其中有[相当多的](https://www.pcgamingwiki.com/wiki/List_of_DirectX_9_games)，虽然没有大量完全依赖 DX9。但是英特尔目前并不认为人们使用 Arc 或 Xe 图形玩这些游戏会有任何问题。

还需要指出的是，这只会影响 GPU 和第 12 代 Xe 集成显卡处理器的弧线。第 11 代英特尔芯片拥有对 DX9 的原生支持，这种支持不会消失。不过，英特尔确实指出，当与 Arc GPU 配对时，除非你告诉你的系统改用集成显卡，否则你将失去这种支持。

> 第 11 代和更老的英特尔处理器上的集成 GPU 原生支持 DX9，但它们可以与 Arc 显卡结合使用。如果是这样，渲染很可能由卡而不是 iGPU 来处理(除非卡被禁用)。因此，系统将使用 DX9On12 而不是 DX9。

所有人都祈祷事情继续按计划进行。

via **[濒临](https://www.theverge.com/2022/8/15/23306160/intel-directx-9-support-emulation-direct-x-12)**