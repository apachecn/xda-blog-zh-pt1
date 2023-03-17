# 谷歌希望从开发者那里得到关于 OEM 软件如何干扰应用程序的反馈

> 原文：<https://www.xda-developers.com/google-developer-feedback-oem-software-affecting-android-apps/>

# 谷歌希望从开发者那里得到关于 OEM 软件如何干扰应用程序的反馈

谷歌邀请应用程序开发者就 OEM 软件如何影响他们的应用程序提供反馈。请继续阅读，了解更多信息。

在过去的几年里，谷歌已经大大改进了 Android 处理后台应用的方式。Doze 和[应用待机桶](https://developer.android.com/about/versions/pie/power)等优化有助于将系统资源分配给最需要它们的应用，同时确保滥用应用不会在后台猖獗运行。

虽然 Android 的节能措施相当有效，但许多智能手机原始设备制造商还会进一步实施额外的后台应用程序删除政策和电池节能选项。这些措施通常更具侵略性，并且[阻止第三方应用程序完成它们的工作](https://www.xda-developers.com/samsungs-one-ui-3-update-annoying-app-killing-behavior/)。一些原始设备制造商还保留了一份白名单，允许脸书和 WhatsApp 等应用程序不受限制地运行，这让小型应用程序开发者处于不利地位。谷歌很清楚这些[的粗制滥造的做法](https://www.xda-developers.com/phone-software-killing-apps-background/)，尽管它还没有采取决定性的行动，但它现在正在邀请开发者的反馈，以寻求一个可能的解决方案。

早在 2018 年，AOSP bug 追踪器上就出现了一个[问题，详细描述了一部分中国原始设备制造商如何滥用 Android 的核心功能，并禁止第三方应用程序在后台运行。这个问题充满了数百名应用程序开发人员的回应，他们重复了类似的经历，敦促谷歌阻止原始设备制造商违反 Android 合规性并实施如此激进的政策。](https://issuetracker.google.com/issues/122098785#comment155)

2021 年 6 月 8 日，一位用户评论说，小米和一加这样的 OEM 厂商甚至扼杀 AccessibilityService。作为回应，一名谷歌员工最近评论说，他们将研究这个问题，并邀请应用程序开发者提交他们的反馈。

谷歌要求开发者提供以下细节:

*   受影响的应用的名称
*   观察到问题的 OEM 和设备型号的名称
*   Android 操作系统版本
*   重现问题的步骤以及预期结果和观察到的结果
*   受影响的 API
*   他们是否能够在 Pixel 设备(或运行相同 Android 版本的其他设备)上重现相同的问题

如果你是一名应用开发者，你可以通过填写本页上的[表格向谷歌提交反馈。](https://docs.google.com/forms/d/e/1FAIpQLSd9P3gLKgMbVwQnAra6UhOjnCWtKpp55kYmigUKo8-ynmvdPg/viewform?resourcekey=0-e65sRbpisoGmtEe_zPZnMg)