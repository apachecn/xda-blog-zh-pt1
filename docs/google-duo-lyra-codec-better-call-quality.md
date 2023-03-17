# Google Duo 使用了一种新的编解码器，在连接不良的情况下提供更好的通话质量

> 原文：<https://www.xda-developers.com/google-duo-lyra-codec-better-call-quality/>

**更新 1 (04/09/2021 @ 03:45 PM ET):** 谷歌发布了 Lyra 的源代码，这是谷歌二人组使用的新的低比特率语音编解码器。[点击这里了解更多信息。](#update1)文章发表于 2021 年 3 月 1 日，下面保留。

虽然美国运营商正忙于营销他们的新 5G 网络，但现实是，绝大多数人不会体验到宣传的速度。美国和世界各地仍有许多地方的数据速度很慢，因此为了弥补这一点，Google Duo 等服务使用压缩技术来有效地提供最佳的视频和音频体验。谷歌现在正在测试一种新的音频编解码器，旨在大幅改善恶劣网络连接的音频质量。

在一篇博文中，谷歌人工智能团队详细介绍了他们命名为“Lyra”的新的高质量、极低比特率语音编解码器。像传统的参数编解码器一样，Lyra 的基本架构包括以[log Mel spectrogram](https://medium.com/analytics-vidhya/understanding-the-mel-spectrogram-fca2afa2ce53)的形式提取独特的语音属性(也称为“特征”)，然后压缩，通过网络传输，并在另一端使用生成模型重新创建。然而，与更传统的参数编解码器不同，Lyra 使用了一种新的高质量音频生成模型，不仅能够从语音中提取关键参数，还能够使用最少量的数据重建语音。Lyra 中使用的新生成模型建立在谷歌[之前在 WaveNetEQ](https://www.xda-developers.com/google-duo-ai-waveneteq-machine-learning-model-audio-call-quality/) 上的工作基础上，WaveNetEQ 是目前在谷歌 Duo 中使用的基于生成模型的丢包隐藏系统。

 <picture>![Lyra architecture](img/407e7664281b977713625daea4eae6cf.png)</picture> 

Lyra's basic architecture. Source: Google

谷歌表示，其方法使 Lyra 与当今许多流媒体和通信平台中使用的最先进的波形编解码器不相上下。根据谷歌的说法，Lyra 优于这些最先进的波形编解码器的优势在于，Lyra 不会逐个样本地发送信号，这需要更高的比特率(因此需要更多的数据)。为了克服在设备上运行生成模型的计算复杂性问题，谷歌表示，Lyra 使用了一种“更便宜的递归生成模型”，它可以“以更低的速率”工作，但会并行生成不同频率范围的多个信号，这些信号随后会“以所需的采样率合并成一个输出信号”。在中端设备上实时运行这种生成模型会产生 90 毫秒的处理延迟，谷歌表示这“与其他传统语音编解码器一致”

与视频的 AV1 编解码器配合使用，谷歌表示，视频聊天甚至可以在一个古老的 56kbps 拨号调制解调器上进行。这是因为 Lyra 被设计为在带宽严重受限的环境中运行，如 3kbps。根据谷歌的说法，Lyra 在非常低的比特率下轻松胜过免版税的开源 Opus 编解码器以及 Speex、MELP 和 AMR 等其他编解码器。以下是谷歌提供的一些语音样本。除了在 Lyra 中编码的音频之外，每个语音样本在非常低的比特率下遭受音频质量下降。

**干净的演讲**

*原件*

https://www.gstatic.com/cmaudio/lyra/ai_blog/clean_p257_011_reference.wav

*Opus@6kbps*

https://www.gstatic.com/cmaudio/lyra/ai_blog/clean_p257_011_opus.wav

天琴座@3kbps

https://www.gstatic.com/cmaudio/lyra/ai_blog/clean_p257_011_lyra.wav

*Speex@3kbps*

https://www.gstatic.com/cmaudio/lyra/ai_blog/clean_p257_011_speex.wav

**嘈杂的环境**

*原件*

https://www.gstatic.com/cmaudio/lyra/ai_blog/noisy_p232_013_reference.wav

*Opus@6kbps*

https://www.gstatic.com/cmaudio/lyra/ai_blog/noisy_p232_013_opus.wav

天琴座@3kbps

https://www.gstatic.com/cmaudio/lyra/ai_blog/noisy_p232_013_lyra.wav

*Speex@3kbps*

https://www.gstatic.com/cmaudio/lyra/ai_blog/noisy_p232_013_speex.wav

谷歌表示，它“使用开源音频库，用超过 70 种语言的扬声器训练了莱拉数千小时的音频，然后用专家和众包听众验证音频质量。”因此，新的编解码器已经在 Google Duo 中推出，以提高极低带宽连接的通话质量。虽然 Lyra 目前针对的是语音用例，但谷歌正在探索如何将其转化为通用音频编解码器。

* * *

## 更新 1:谷歌开源 Lyra 编解码器用于谷歌二重奏

本周早些时候，谷歌[宣布](https://opensource.googleblog.com/2021/04/lyra-enabling-voice-calls-for-next-billion-users.html)已经开源了谷歌二人组使用的新音频编解码器 Lyra，因此其他开发者可以在自己的通信应用中使用它。该版本附带了使用 Lyra 编码和解码音频所需的工具，并针对在 Linux 上开发的 64 位 ARM Android 进行了优化。开源库专注于使用 Lyra 进行实时语音通信，但谷歌希望开发人员将该编解码器应用于其他编码和解码音频语音的应用程序。代码是用 C++编写的，核心 API、信号处理工具链和一个演示 Android 应用程序现在可以在 [GitHub](https://github.com/google/lyra) 上获得，作为 Apache 许可下的测试版。