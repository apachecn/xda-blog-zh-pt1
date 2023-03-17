# NVIDIA 广播 1.3 版带来了巨大的性能改进

> 原文：<https://www.xda-developers.com/nvidia-broadcast-13-brings-performance-improvements/>

NVIDIA 发布了 NVIDIA Broadcast 应用程序的最新更新，使其版本达到 1.3。对于那些不知道的人，NVIDIA Broadcast 是一款为 NVIDIA RTX 卡所有者设计的应用程序，允许他们将音频和视频效果添加到他们的流媒体设置中。这包括背景噪音消除或虚拟视频背景，这在之前的 [RTX 之声](https://www.xda-developers.com/nvidia-rtx-voice-available-on-gtx-cards/)应用中是可用的。

1.3 版本的更新为 NVIDIA Broadcast 带来了几项关键改进。首先，如果您使用背景噪音消除功能，您可能已经注意到，在过去，高音调的声音和尖叫声可能会导致音频中断。NVIDIA 表示，这种情况很少见，但因为它通常发生在流的高峰兴奋期间，所以仍然是一个大问题。现在，该公司使用新的训练声音配置文件来解释这些场景，以便在消除背景噪音的同时仍然可以听到声音。

该版本还降低了堆叠不同效果对性能的影响。以前，同时使用多个音频和视频效果可能会很快耗尽 GPU 的 VRAM。在 NVIDIA Broadcast 1.3 中，在堆叠基于 AI 的效果时，VRAM 的使用量减少了 40%以上，保持游戏在流传输时流畅运行。

最后，NVIDIA 增加了对更多应用程序的支持，以便与 NVIDIA Broadcast 配合使用。你现在可以使用佳能、尼康和索尼的网络摄像头工具以及 OBS 虚拟相机来使用该应用程序。更重要的是，为了让应用程序更好地工作，我们还在这里和那里做了一些 UI 调整和修复。

提醒一下，由于与其他开发商的合作，NVIDIA Broadcast 的许多功能也可以在其他应用程序中使用。音频噪声消除功能可以在 OBS Studio 和 streamers 的 Streamlabs 等应用程序中找到，而视频编辑可以在 Adobe Premiere Pro 和 Audacity 等工具中使用。不过，你需要安装 [NVIDIA Broadcast 可再发行软件包](http://www.nvidia.com/broadcast-sdk-resources)才能使用这些功能。

如果只是想要单机版 app，现在就可以下载[英伟达广播 1.3 版](https://www.nvidia.com/en-us/geforce/broadcasting/broadcast-app/)。