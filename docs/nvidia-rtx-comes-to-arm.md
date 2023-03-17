# 英伟达 RTX 包括实时光线跟踪和 DLSS 即将推出 ARM

> 原文：<https://www.xda-developers.com/nvidia-rtx-comes-to-arm/>

# NVIDIA 将 RTX 实时光线追踪和 DLSS 引入 ARM

NVIDIA 宣布，它已经成功地将实时光线跟踪和 DLSS 技术移植到 ARM 平台上。

游戏开发者大会 2021 已经正式拉开帷幕，英伟达正在发布一堆公告。该公司刚刚证实，其广受欢迎的 RTX 技术将进入 ARM 平台。英伟达还公布了新的技术演示，展示其 GeForce RTX 技术公司与基于 ARM 的联发科处理器的配对。这也是自从有报道称 [NVIDIA 将接管 ARM](https://www.xda-developers.com/nvidia-officially-buying-arm-promise-maintain-neutral-open-licensing-model/) 以来，我们听到的两者之间的第一次进展。

两个演示包括流行的 Wolfenstein: Youngblood 和来自开放研究内容存档的 Bistro，它们在配备 GeForce RTX 3060 的联发科 Kompanio 1200 处理器上实时运行。Wolfenstein: Youngblood 演示使用了光线跟踪反射，所有这些都由英伟达 DLSS 加速，该公司使用 GPU 加速的深度学习算法来提高帧速率。同样，NVIDIA 展示了 Bistro 演示，该演示描绘了一个详细的光线跟踪的法国城市场景，启用了 RTX 直接照明(RTXDI)和 NVIDIA Optix AI-Acceleration Denoiser(NRD)。

NVIDIA 通过移植几个 SDK 成功将其 RTX 技术引入 ARM，包括:

*   深度学习超级采样(DLSS)，它使用人工智能来提高帧速率，为游戏生成清晰的图像
*   RTX 直接照明(RTXDI)，允许开发人员将动态照明添加到他们的游戏环境中。
*   NVIDIA Optix AI-Acceleration Denoiser(NRD)，使用 AI 更快地渲染高保真图像。
*   RTX 内存实用程序(RTXMU)，它优化了应用程序使用图形内存的方式。
*   RTX 全局照明(RTXGI)，有助于在真实世界环境中重现光线反弹的方式。

“在过去的二十年里，RTX 是电脑游戏领域最具突破性的技术。联发科和英伟达正在为基于 Arm 的高性能个人电脑的新类别奠定基础，”联发科智能多媒体业务部总经理 PC Tseng 表示。

您可以查看以下在 GDC 2021 上展示的 RTX on ARM 演示:

NVIDIA 还宣布发布了最新版本的工作室驱动程序 T1，它正式支持两个最受欢迎的游戏引擎——Unity 和 Unreal Engine——以及 Toolbag、Omniverse 等。