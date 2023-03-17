# Google Pay 可以安全地存储你的新冠肺炎疫苗信息

> 原文：<https://www.xda-developers.com/google-pay-covid-19-vaccine-passport/>

谷歌已经更新了 [Passes API](https://developers.google.com/pay/passes) ，以便能够安全地在你的 Android 智能手机上存储你的新冠肺炎疫苗接种卡和/或测试状态，这标志着[谷歌试图帮助当局打击新冠肺炎疫情](https://www.xda-developers.com/google-apple-contact-tracing-coronavirus/)的又一种方式。

[通行证 API](https://developers.google.com/pay/passes) 允许第三方开发者创建登机牌、积分卡、数字门票等。用户可以保存到 Google Pay 以便于访问。多亏了 Passes API，可以在 Google Pay 应用程序中汇总[您的登机牌和积分卡](https://www.xda-developers.com/google-pay-boarding-passes-money-transfers/?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%3A+xda-developers%2FShsH+%28xda-developers%29)，从而快速轻松地登机或跟进您的订阅。现在，Passes API 已经更新，因此来自医疗保健组织、政府机构或公共卫生当局授权的组织的开发人员可以将用户的数字新冠肺炎疫苗卡/检测信息集成到 Google Pay 中。然后，可以从所有者的智能手机访问数字新冠肺炎疫苗接种卡或检测报告，并显示给可能需要查看它的相关人员。

任何拥有运行 Android 5 或更高版本的设备的人——只要他们的设备经过 Google Play 认证——都可以在他们的设备上数字化存储他们的新冠肺炎疫苗接种信息或测试状态。谷歌在其博客文章中表示，这项功能将首先在美国推出，随后在其他国家推出。

为了确保用户的私人医疗信息不被泄露，谷歌表示，API 将数字证书存储在智能手机上，不会上传到云。一旦存储在设备上，即使在离线或互联网连接微弱的情况下，也可以从所有者的主屏幕上访问该卡。用户可以将它存储在多个设备上，尽管他们需要手动这样做，因为它不是存储在谷歌服务的云中。卡上的信息不会与谷歌共享，也不会用于广告或其他服务。最后，为了保护用户信息，在设备上存储新冠肺炎卡需要一个锁定屏幕。甚至访问该卡也需要保存的密码、pin 或设备上使用的生物识别方法。

合格的供应商可以在这里让谷歌知道他们的兴趣。用户不需要实际安装 Google Pay 应用程序来访问他们的新冠肺炎疫苗接种或测试卡，因为通行证 API 和卡的添加/检索都是通过 Google Play 服务处理的，Google Play 服务预装在所有带有 Google 移动服务的手机上。