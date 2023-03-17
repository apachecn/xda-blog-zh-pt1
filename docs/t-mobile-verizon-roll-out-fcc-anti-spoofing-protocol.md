# T-Mobile、美国电话电报公司和威瑞森已经推出了 FCC 的反电子欺骗协议

> 原文：<https://www.xda-developers.com/t-mobile-verizon-roll-out-fcc-anti-spoofing-protocol/>

为了打击美国的垃圾电话和机器人电话，联邦通信委员会(FCC)在去年 3 月为强制采用 STIR/shake 协议设定了最后期限。该命令要求主要运营商在 2021 年 6 月 30 日前遵守 IP 呼叫的反欺骗系统，并使用加密证书验证所有呼叫。该地区所有的三大运营商，T-Mobile，AT & T，和威瑞森，现在已经确认他们完全符合该协议。

根据最近来自[*【The Verge】*](https://www.theverge.com/2021/6/30/22557539/t-mobile-verizon-carriers-fcc-stir-shaken-certification-deadline-spam-calls)的报道，T-Mobile 已经[宣布](https://www.t-mobile.com/news/press/t-mobile-calls-are-100-stir-shaken-compliant)它现在证明来自其网络的呼叫受到保护，不会被使用 STIR/shake 协议的诈骗呼叫者冒充。威瑞森还[证实](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU3583/https://www.verizon.com/about/news/over-78-million-verizon-customers-protected-over-13-billion-unwanted-calls)它正在使用反欺骗协议来验证显示在来电显示上的号码实际上就是正在呼叫的那个号码。同样，AT & T 的发言人透露，该运营商也满足了最后期限，现在它确保*“所有源自[其]无线网络的 LTE 和 5G 呼叫都符合 STIR/shake 标准。”*

对于不知情的人来说，STIR/shake 代表“使用令牌重新访问安全电话身份/基于签名处理断言信息”这是抵御 robocalls 的最佳防线之一，因为它要求运营商使用加密证书来验证和签署来自其网络的呼叫。然后，目的地网络会再次验证该证书，防止骗子和机器人呼叫者假冒他们的电话号码。

值得注意的是，2021 年 6 月 30 日的截止日期仅针对主要运营商。在 2023 年 6 月 30 日之前，订户少于 100，000 人的较小运营商可以免税。然而，联邦通信委员会正在考虑缩短这一期限。

为了跟踪运营商的机器人呼叫缓解工作，FCC 还建立了机器人呼叫缓解数据库。该机构要求语音服务提供商在数据库中提交其缓解工作的证明，包括其 STIR/shake 实施状态。FCC 在新闻发布会上透露，到目前为止，已经有超过 1500 家语音服务提供商在数据库中备案。超过 200 家语音服务提供商已获得全面 STIR/shake 实施认证，还有*“数百家已获得部分实施认证。”*FCC 进一步补充道，如果服务提供商的认证在 2021 年 9 月 28 日之后没有出现在 Robocall 缓解数据库中，它将禁止中间和其他语音服务提供商直接接受该提供商的流量。