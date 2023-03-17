# 谷歌成立 Android Ready SE 联盟，推动数字钥匙和身份证

> 原文：<https://www.xda-developers.com/android-ready-se-alliance-digital-car-keys-drivers-licenses/>

智能手机已经取代了从数码相机到专用音乐播放器的所有东西。当我们还在等待设备完全取代钱包时，谷歌已经宣布成立 Android Ready SE 联盟，这是一项旨在推动数字钥匙和驾照采用的新举措。

[Android 11 引入了](https://www.xda-developers.com/google-android-digital-drivers-license/)身份凭证 API，可以使用手机安全存储手机驾照或其他凭证。虽然 Android APIs 和支持库已经存在，但谷歌现在正致力于标准化如何在安全、防篡改的硬件上存储和访问这些凭证，顺便说一下，谷歌表示，“大多数现代手机”都有这种功能。

[据谷歌](https://security.googleblog.com/2021/03/announcing-android-ready-se-alliance.html)称，Android Ready SE 联盟的成立是为了“创建一套开源的、经过验证的、随时可用的 SE[安全元素]小程序。”谷歌首先优先开发小程序，旨在实现身份凭证(如移动驾照)和数字汽车钥匙的使用。

*图片:谷歌*

谷歌之前开发了自己的防篡改硬件 enclave，名为 Titan M，它也可以使用 StrongBox 为 Android 应用程序提供防篡改密钥存储。现在，谷歌推出了面向 SE 的 StrongBox 的通用(GA)版本，这是一个合格的小程序，可供 OEM 合作伙伴使用。供应商包括 Giesecke+Devrient、Kigen、恩智浦、意法半导体和泰雷兹。作为 Android Ready SE 联盟成员的原始设备制造商必须满足以下要求:

1.  从 SE 供应商处挑选合适的、[经过验证的硬件部件](https://developers.google.com/android/security/android-ready-se/supported-chipsets)
2.  支持从引导加载程序初始化 SE，并通过 SPI 接口或加密绑定提供信任根(RoT)参数
3.  与 Google 合作，在 SE 工厂中提供证明密钥/证书
4.  为 se 小程序使用 GA 版本的 StrongBox，以适应您的 SE
5.  集成 HAL 代码
6.  启用 SE 升级机制
7.  对 StrongBox 运行 CTS/VTS 测试，以验证集成是否正确完成

苹果、三星和少数汽车制造商等公司已经在研发自己的数字汽车关键技术。事实上，在 [Galaxy S21 系列宣布](https://www.xda-developers.com/galaxy-s21-digital-key-audi-bmw-ford-genesis/)后不久，就有消息称三星的设备将能够找到并解锁奥迪、宝马、福特和 Genesis 的汽车。但谷歌的努力更多地是针对运行 Android 的设备，这可能会扩大可以与我们的汽车互动或持有我们的 id 的设备的数量。

不过，谷歌表示，这一联盟不仅仅针对手机和平板电脑。它还面向 Wear OS、Android Auto Embedded 和 Android TV 等平台。据谷歌称，几家 Android OEMs 厂商已经在未来的设备中采用 Android Ready SE，但这家搜索巨头没有透露任何公司的名称。欲了解更多信息，[请访问 developers.google.com Android 安全和隐私版块下的该计划专用页面](https://developers.google.com/android/security/android-ready-se)。