# 高通调制解调器缺陷影响 30%的手机；让攻击者记录电话

> 原文：<https://www.xda-developers.com/qualcomm-modem-flaw-record-phone-calls/>

以色列安全公司 Check Point Research 发现了高通移动站调制解调器的一个缺陷，该缺陷影响了全球数百万部安卓手机。该公司声称，黑客可以利用这一漏洞，获取你的短信，电话，在某些情况下，甚至解锁你的 SIM 卡。

Check Point 的[报告](https://research.checkpoint.com/2021/security-probe-of-qualcomm-msm/)显示，移动站调制解调器是高通芯片不可或缺的一部分，可以追溯到 20 世纪 90 年代初。它仍然是该公司一些最新 5G 芯片组的一部分，并且可以在三星、谷歌、小米、LG、一加等公司的一些最新型号中找到。因此，该漏洞影响了全球很大一部分 Android 智能手机。Check Point 估计，多达 30%的安卓手机安装了包含该漏洞的高通调制解调器软件。

该报告进一步揭示，黑客可以利用该漏洞从 Android 向调制解调器注入恶意代码。这使得攻击者能够访问用户的通话记录和短信，并能够监听用户的对话。”攻击者还可以利用该漏洞解锁 SIM 卡，并克服服务提供商设置的任何限制。

高通意识到了这个漏洞，并且公司已经发布了一个补丁。在给 [*Tom's Guide*](https://www.tomsguide.com/news/qualcomm-modem-flaw) 的一份声明中，*的一名高通代表表示，“高通科技已经在 2020 年 12 月向原始设备制造商提供了补丁，我们鼓励最终用户在补丁可用时更新他们的设备。”*值得一提的是，自 2020 年 12 月以来发布的任何 [Android 安全公告](https://www.xda-developers.com/tag/android-security-bulletin/)中都没有包含分配给该漏洞的目录号(CVE-2020-11292)。但谷歌可能在之前的安全更新中包含了它，而没有在公告中提及。据高通发言人称，该公司将在 2021 年 6 月的安全更新中公开解决这一问题。

目前，还不清楚是否所有受影响的设备都被打了补丁。“根据我们的经验，实施这些修复需要时间，所以许多手机很可能仍然容易受到威胁，”一位 Check Point 代表告诉 Tom's Guide。如果你使用的高通骁龙设备自 2020 年 11 月以来没有收到安全更新，你的设备很可能仍然容易受到攻击。但是，如果您有，您的 OEM 可能已经修补了该漏洞。

有关漏洞的更多细节，请点击[此链接](https://www.tomsguide.com/news/qualcomm-modem-flaw)查看 Check Point 的报告。