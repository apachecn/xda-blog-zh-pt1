# 谷歌二人组可能在 4 月因未经认证的安卓设备而关闭

> 原文：<https://www.xda-developers.com/google-duo-shut-down-april-2021-uncertified-android-devices/>

我们最近报道了在 [Google Messages 应用程序中发现的新字符串，表明该应用程序将从 2021 年 4 月](https://www.xda-developers.com/google-messages-stop-working-uncertified-android-phones-april-2021/)起停止在未经认证的 Android 设备上运行。Google Duo 似乎也加入了这个名单，因为该应用程序最新更新中的新字符串表明，4 月份视频通话服务也将关闭。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Google Duo v123 正在谷歌 Play 商店上推出，它包含以下新字符串:

```
 <string name="grace_period_notification_body">"Because you're using an unsupported device, Duo will unregister your account on this device soon. Download your Clips and call history to avoid losing them."</string>
<string name="grace_period_notification_title">Duo is going away soon</string> 
```

虽然 Google Messages 中的字符串很简单，但是 Google Duo 中的字符串引用了“不支持的”设备。在这些不受支持的设备上，您的帐户将被注销，但在被踢出之前，您将有机会下载剪辑和通话记录。

然而，到底什么是“不受支持”的设备呢？深入挖掘反编译后的代码，我们可以确认“不受支持的”设备在此上下文中是指不符合 GMS，本质上与未经认证的设备意思相同。反编译的代码还表明，谷歌已经将最终强制执行日期定为 2021 年 3 月 31 日，在此之后，谷歌 Duo 将完全停止为未经认证的设备工作。但稍微松了口气的是，有 14 天的宽限期，因此未经认证的 Android 设备上的用户在应用和服务为他们关闭之前，将有足够的时间下载他们的数据。

人们可以把 [RCS 端到端加密的推出](https://www.xda-developers.com/google-rcs-e2ee-messages/)看作是谷歌放弃支持谷歌消息上未经认证的设备的一个看似合理的理由。但是对于 Gooogle Duo 来说，这个观点站不住脚。Google Duo 在网上[是免费的](https://duo.google.com/)，没有设备限制。因此，在经过认证或未经认证的设备上使用相同的功能并不重要。正如 Mishaal 确认的那样，你可以在华为 P40 Pro 上安装和使用 Google Duo，而不需要谷歌移动服务。当然，网络也是如此。因此，只将其中一个排除在外，而让另一个存在，似乎是不合理的。我们希望谷歌在实施改变时澄清其理由。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*