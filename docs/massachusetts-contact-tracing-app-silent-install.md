# 谷歌悄悄地在用户手机上安装了马萨诸塞州的联系人追踪应用程序

> 原文：<https://www.xda-developers.com/massachusetts-contact-tracing-app-silent-install/>

# 谷歌悄悄地在用户手机上安装了马萨诸塞州的联系人追踪应用程序

谷歌已经悄悄地在用户的智能手机上安装了马萨诸塞州的联系人追踪应用程序，引起了轩然大波。

谷歌似乎已经悄悄地在用户的智能手机上安装了马萨诸塞州新冠肺炎联系人追踪应用程序。“MassNotify”应用程序被发现自动安装在用户的设备上，在主屏幕或可搜索的 Play Store 列表上没有应用程序图标。虽然一些人推测它会自动安装在打开了 [Android 暴露通知](https://www.xda-developers.com/google-apple-exposure-notifications-express-covid-19-contact-tracing/)的设备上，但许多用户报告说他们没有启用该功能，并且该应用程序仍然安装在他们的智能手机上。

MassNotify 的帮助台联系了一个 [YCombinator 的黑客新闻阅读器](https://news.ycombinator.com/item?id=27563203)(通过 [*传呼电脑*](https://www.bleepingcomputer.com/news/security/google-force-installs-massachusetts-massnotify-android-covid-app/) )，他们告诉这个人，安装这个应用程序并不意味着这个应用程序是活跃的或在后台运行。

> #### “应用程序列表中出现 MassNotify 并不意味着您的电话启用了 MassNotify。该应用程序的出现仅仅意味着，如果您希望启用 MassNotify，它已经成为您手机设置中的一个选项。有关这方面的更多信息，请参见谷歌帮助中心的文章:[https://support.google.com/android/answer/10775533](https://support.google.com/android/answer/10775533)。你可以通过进入设置- >谷歌- >新冠肺炎暴露通知来查看 MassNotify 是否激活。页面顶部的“使用暴露通知”开关将显示 MassNotify 是否处于活动状态。在该屏幕上，您还可以随时启用或禁用 MassNotify。”

用户反映该应用不容易卸载，除非他们可以通过应用的包名找到 Play Store 列表[。许多用户第一次发现，当他们被提示更新应用程序时，他们甚至已经安装了应用程序。这款应用的评论目前充斥着用户，他们说这款应用未经他们同意就被安装到了他们的智能手机上，而且这款应用不容易卸载。](https://play.google.com/store/apps/details?id=gov.ma.covid19.exposurenotifications.v3)

MassNotify 是马萨诸塞州的官方应用程序，它使用暴露通知 API 来检测您何时被视为自报新冠肺炎阳性诊断的另一人的“密切接触者”。该 API 在 Android 和 iOS 之间跨平台工作，并已在全球一些国家成功部署和使用。然而，未经设备所有者同意，不应安装应用程序，尤其是收集设备数据的应用程序。它为谷歌强制在设备上安装应用程序开了一个坏先例，即使没有恶意内容和数据是匿名的。

*哔哔作响的电脑*联系谷歌询问了许多关于 MassNotify 的问题，并收到了以下回复:

> #### “我们一直在与马萨诸塞州公共卫生部合作，允许用户直接从他们的 Android 手机设置中激活暴露通知系统。该功能内置于设备设置中，并由谷歌 Play 商店自动分发，因此用户不必下载单独的应用程序。新冠肺炎暴露通知只有在用户主动打开时才会启用。用户决定是否启用该功能，以及是否通过系统共享信息，以帮助警告其他人可能的暴露。”