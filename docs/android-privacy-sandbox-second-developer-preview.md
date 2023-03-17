# 谷歌发布第二个安卓隐私沙盒开发者预览版

> 原文：<https://www.xda-developers.com/android-privacy-sandbox-second-developer-preview/>

# 谷歌发布 Android 隐私沙盒的第二个开发者预览版

Android Privacy Sandbox 的第二个预览版在这里，它包括 MeasurementManager 属性报告 API 的早期预览。

谷歌的隐私沙箱是一项多年的倡议，旨在使用户的网络浏览更加隐私，同时为广告商提供更有效的个性化广告的新工具。4 月下旬，谷歌将这一计划扩展到了 Android，推出了 Android 隐私沙盒的[首个开发者预览版。](https://www.xda-developers.com/android-privacy-sandbox-preview/)第一个预览版允许开发者测试主题 API 和 SDK 运行时。现在谷歌发布了第二个开发者预览版。

Android Privacy Sandbox 的第二个预览版在这里，它包括 MeasurementManager 属性报告 API 的早期预览。Google 的发行说明解释了您可以在测试设备上使用新 API 做什么:

*   您可以调用 *registerSource()* 和 *registerTrigger()* 来注册应用广告事件，并接收事件级报告数据以进行应用到应用的归属。我们当前的实现使用最后接触属性。根据报告窗口的定义，计划发送报告。有关更多信息，请参考 MeasurementManager API 参考。
*   实际的报告上传发生在固定的时间间隔结束时，而不是在确切的计划时间。报告上传间隔默认为 4 小时，但可以使用以下 adb 命令覆盖:*ADB shell device _ config put adservices measurement _ main _ reporting _ job _ period _ ms<持续时间(毫秒)>*

谷歌表示，MeasurementManager API 的其他功能，如汇总报告、安装后属性和重定向，将在稍后添加。此外，用于测试 API 的示例应用和参考广告服务器将在未来版本中提供。

开发者可以通过 Android 模拟器尝试新的 Android 隐私沙盒预览。此外，谷歌还[为 Pixel 6、Pixel 6 Pro、Pixel 5、Pixel 5a、Pixel 4、Pixel 4a 提供了 64 位系统映像](https://developer.android.com/design-for-safety/privacy-sandbox/download#device)。

Android 隐私沙盒预览计划将贯穿 2022 年。在接下来的几个月里将会有更多的开发者预览版，并计划在今年年底发布测试版。

* * *

**来源** : [安卓开发者](https://developer.android.com/design-for-safety/privacy-sandbox/reference/adservices/measurement/MeasurementManager)