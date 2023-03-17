# Chrome 将增加性能覆盖以帮助网站开发者建立更快的网站

> 原文：<https://www.xda-developers.com/google-chrome-performance-heads-up-display/>

当谷歌今年晚些时候推出 Chrome 90 时，该浏览器将提供一个可选的新覆盖，为开发者提供网站表现的重要统计数据。

谷歌工程经理[Addy Osmani](https://addyosmani.com/blog/performance-hud/)(via[*AndroidPolice*](https://www.androidpolice.com/2021/01/22/chrome-90-will-get-a-performance-overlay-helping-developers-create-faster-websites/))详细介绍了 Chrome 的新性能平视显示器(HUD)。新的覆盖层将成为 Chrome DevTools 的一部分，将为开发者提供核心网站活力和平滑度指标。HUD 启用后，它将持续显示在每个标签上。

新的性能叠加是在[谷歌推出 Web Vitals](https://www.xda-developers.com/google-announces-web-vitals-initiative/) 之后推出的，这是一项旨在“为质量信号提供统一指导的举措，这些信号对于在网络上提供出色的用户体验至关重要。”

以下是我们在 2020 年 5 月对核心网络重要指标的描述:

> 核心网站生命是适用于所有网页的所有网站生命的子集，应该由所有网站所有者来衡量，并将在所有谷歌工具中出现。目前，这些核心 Web 要素关注用户体验的三个方面——加载、交互性和视觉稳定性——并包括以下指标(及其各自的阈值):
> 
> *   最大含量涂料(LCP):测量装载性能。为了提供良好的用户体验，LCP 应该在页面首次开始加载后的 2.5 秒内发生。
> *   第一输入延迟(FID):测量交互性。为了提供良好的用户体验，页面的 FID 应该小于 100 毫秒。
> *   累积布局偏移(CLS):测量视觉稳定性。为了提供良好的用户体验，页面应该保持小于 0.1 的 CLS

开发人员最感兴趣的是创建一个快速流畅的网站。这是因为从 2021 年 5 月开始，谷歌将根据“页面体验”对网站进行排名。去年 8 月，谷歌开始将网站标记为符合核心网络指标，告诉 Chrome 85 用户某个链接是否会导致“快速页面”。

据 Osmani 称，HUD 仍在打磨中，因此稳定性和性能等问题将随着时间的推移而出现。你可以前往[crbug.com](https://crbug.com/new)并在内部> GPU >度量组件下报告任何错误或反馈。