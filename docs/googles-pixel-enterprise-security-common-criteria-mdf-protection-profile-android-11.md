# 谷歌 Pixel 手机首先在 Android 11 上满足通用标准的 MDF 保护配置文件

> 原文：<https://www.xda-developers.com/googles-pixel-enterprise-security-common-criteria-mdf-protection-profile-android-11/>

# 谷歌的 Pixel 手机是第一批符合通用标准的 Android 11 保护配置文件的手机

采用 Android 11 的谷歌 Pixel 设备现已通过通用标准的严格 MDF 保护配置文件认证，可实现强大的企业安全性。

除了摄像头，谷歌 Pixel 智能手机可能在整体硬件方面有所欠缺，但最快的软件更新使它们非常受欢迎。Pixel 设备不仅比其他设备先获得最好的 Android 功能，还通过每月的安全更新获得顶级的安全性。除了这些更新，专用的 [Titan M 安全芯片](https://www.xda-developers.com/google-pixel-3-titan-m-security/)据称可以提供企业级隐私保护。现在，运行 [Android 11](https://www.xda-developers.com/android-11-stable-google-pixel-oneplus-xiaomi-realme-oppo/) 的 Pixel 设备也是第一批符合 Common Criteria 的 MDF 安全标准的设备。

[移动设备基础(MDF)保护简介](https://commoncriteriaportal.org/files/ppfiles/pp_md_v3.1.pdf)由[通用标准](https://commoncriteriaportal.org/ccra/index.cfm)制定，概述了全球 31 个国家的 IT 公司必须遵守的准则。谷歌在[博客文章](https://security.googleblog.com/2021/03/continuing-to-raise-bar-for-verifiable.html#Blog1:~:text=strongest%20possible%20protections)中指出，这些指导方针确保企业用户数据受到*最强有力的保护*。这一认证允许谷歌为其运行 Android 11 的 Pixel 设备(即 Pixel 3 及以上版本)背书，这些设备最适合需要保护大量敏感数据的企业用户。

使 Common Criteria 的 MDF 指南更具说服力的是，评估是在实验室中进行的，专家们在实验室中测试设备对消费者和企业面临的各种"*现实世界威胁的弹性*。进行这些测试是为了保证“*每一个如广告所宣传的缓解工程*为了验证 Pixel 设备面临不同威胁时的缓解措施，实验室评估了以下功能:

*   **受保护的通信** -确保所有通信和网络(包括 Wi-Fi)的流量都经过加密。
*   **受保护的存储** -确保存储加密和防篡改机制，如 Titan M 芯片。
*   **授权和认证** -检查欺骗和虚假接受
*   **移动设备完整性**——验证 Android 对[验证启动](https://source.android.com/security/verifiedboot)、 [Google Play 系统更新](https://source.android.com/devices/architecture/modular-system)、[无缝 OS 更新](https://source.android.com/devices/tech/ota/ab)的实现。
*   **可审计性** -供用户报告或 IT 管理员检查事件，如设备启动和关闭、数据加密、数据解密和密钥管理。
*   **移动设备配置** -供企业管理员执行 Android Enterprise 针对摄像头、位置或应用程序安装的安全策略。

除了对企业而言，这些安全功能还可确保用户免受窥探和/或一般或有针对性的攻击。例如，如果你的 Pixel 手机丢失或被盗，由于这些保护措施，你的个人数据被访问的几率会降低。

谷歌补充道，“*满足必要的安全需求所需的特性被直接嵌入到 Android 开源项目中。*“这些工具已经发布在 [GitHub](https://github.com/android/security-certification-resources) 上，供原始设备制造商用于类似的认证。除了 MDF 保护配置文件，谷歌还将帮助原始设备制造商获得[国家技术研究所的](https://www.nist.gov/) [加密算法](https://csrc.nist.gov/projects/cryptographic-algorithm-validation-program)和[模块验证程序](https://csrc.nist.gov/projects/cryptographic-module-validation-program)以及[美国国防部的安全技术实施指南](https://public.cyber.mil/stigs/)的认证。