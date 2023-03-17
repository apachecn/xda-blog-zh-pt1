# 苹果发布 iOS 14.8 修复新的据称被 NSO 集团使用的零点击漏洞

> 原文：<https://www.xda-developers.com/ios-14-8-security-patches/>

# 苹果发布 iOS 14.8 修复新的据称被 NSO 集团使用的零点击漏洞

苹果发布了带有一些重要安全补丁的 iOS 14.8。随着 iOS 15 版本的临近，这次更新可能是 iOS 14 收到的最后一次更新。

苹果发布了带有一些重要安全补丁的 iOS 14.8。这次更新可能是 iOS 14 收到的最后一次更新，因为随着新的 [iPhone 13](https://www.xda-developers.com/iphone-13/) 的发布，iOS 15 的发布也将临近。然而，苹果可能会允许用户安装未来的安全更新，而不必更新到下一个主要的操作系统版本。

一周前，公民实验室(Citizen Lab)通过 iMessage 通知苹果(Apple)一个针对 iOS、iPadOS、watchOS 和 macOS 用户的[新零日零点击漏洞利用](https://citizenlab.ca/2021/09/forcedentry-nso-group-imessage-zero-click-exploit-captured-in-the-wild/)。除了设备的摄像头和麦克风之外，攻击者还可以获得敏感信息，包括受害者的消息、通话记录和电子邮件。这个名为 FORCEDENTRY 的漏洞源于以色列，由 NSO 集团分发给世界各国政府。苹果花了一周时间修复，建议所有用户尽快更新设备。

除了 iOS 14.8，苹果还发布了跨 iPadOS、watchOS 和 macOS 的安全更新。在一份[支持文档](https://support.apple.com/en-us/HT212807)中，苹果列出了以下修复:

*   核心图形
    *   适用于:iPhone 6s 和新款机型、iPad Pro(所有型号)、iPad Air 2 和新款机型、iPad 第 5 代和新款机型、iPad mini 4 和新款机型以及 iPod touch(第 7 代)
    *   影响:处理恶意制作的 PDF 可能导致任意代码执行。苹果意识到有报道称该问题可能已被积极利用。
    *   描述:通过改进输入验证解决了整数溢出问题。
    *   CVE-2021-30860:公民实验室
*   网络工具包
    *   适用于:iPhone 6s 和新款机型、iPad Pro(所有型号)、iPad Air 2 和新款机型、iPad 第 5 代和新款机型、iPad mini 4 和新款机型以及 iPod touch(第 7 代)
    *   影响:处理恶意制作的 web 内容可能会导致任意代码执行。苹果意识到有报道称该问题可能已被积极利用。
    *   描述:内存管理的改进解决了释放后使用的问题。
    *   CVE-2021-30858:一位匿名研究者

要更新你的 iPhone，你可以查看我们的教程[如何在你的 iPhone](https://www.xda-developers.com/how-to-check-update-ios-iphone/) 上检查和更新 iOS。我们强烈建议所有用户尽快在其设备上更新到最新版本的 Apple 软件。