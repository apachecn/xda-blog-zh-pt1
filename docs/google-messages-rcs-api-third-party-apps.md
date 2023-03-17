# Google Messages 为第三方应用程序隐藏了一个 RCS API

> 原文：<https://www.xda-developers.com/google-messages-rcs-api-third-party-apps/>

**更新 2 (07/09/2021 @美国东部时间下午 4:49):**我们了解到该 RCS API 目前不打算由第三方应用程序使用。[点击这里了解更多信息。](#update2)

### 以前的更新

**更新 1 (07/09/2021 @ 02:53 PM ET):** 我们已经更新了这篇文章，说明该 API 只能在三星独家版的谷歌消息应用程序中找到。[点击这里了解更多信息。](#update1)

RCS 代表丰富的通信服务，通常被视为 SMS 的继任者。它支持群聊管理、更高质量的文件共享、阅读回执、打字指示器和端到端加密等功能。为了使用 RCS 协议进行聊天，它必须通过 API 得到网络、手机操作系统和手机消息应用程序的支持。美国运营商在采用 RCS 方面拖了太长时间，所以谷歌完全绕过他们，将他们自己的 RCS 后端添加到谷歌消息应用程序中。然而，在 Android 上，*只有*Google Messages 应用程序可以访问 Android 的 RCS API。如果谷歌开放其“安卓信息应用编程接口”，这种情况可能会改变。

回到 2019 年，[我们了解到](https://www.xda-developers.com/google-rcs-api-3rd-party-apps/)谷歌正在致力于增加一个 RCS API。可悲的是，这些 API 对开发者是隐藏的，只能由隐藏的允许列表上的应用程序使用，包括谷歌消息应用程序。虽然谷歌消息应用程序最近变得更好，但它仍在更新基本功能，你会发现许多其他[安卓短信应用程序](https://www.xda-developers.com/best-text-messaging-apps-android/)。切换到其他应用程序的问题是，你将无法通过 RCS 发送消息，因此你将失去我们上面谈到的所有功能。然而，我们发现有证据表明，谷歌有一个未公开的“Android Messages API”，可以让任何第三方短信应用程序使用谷歌消息发送 SMS/MMS/RCS 消息。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

当 Google Messages 今天在 Google Play 上发布时，我们解码了 APK，并在其资源中发现了以下字符串:

```
 <string name="external_messaging_api_description">With this permission the app will be allowed to send SMS/MMS/RCS using Android Messages. It will have an access to send messages without any extra approvals.</string>
<string name="external_messaging_api_label">Permission to send SMS/MMS/RCS messages using Android Messages API</string> 
```

这些字符串清楚地描述了第三方消息应用程序可以请求的权限，以便能够通过 Google Messages 应用程序发送 SMS、MMS 或 RCS 消息。在 Google Messages 应用程序的清单文件中，我们还发现了消息应用程序必须声明的权限:

```
 <permission android:description="@string/external_messaging_api_description" android:label="@string/external_messaging_api_label" android:name="com.google.android.apps.messaging.EXTERNAL_MESSAGING_API" android:permissionGroup="android.permission-group.SMS" android:protectionLevel="dangerous"/> 
```

权限类型被列为“危险”，这意味着在没有向用户显示确认信息的情况下，它不会被授予请求应用程序。上面嵌入的字符串也暗示了这一点，其中声明拥有权限的应用程序可以“发送消息而无需任何额外的批准”，这意味着最初必须获得批准。该权限被分组在短信类别下，这是有意义的，因为它只打算由消息应用程序使用。

虽然我们希望看到 Google 开放 Android 平台的 RCS API，但是让 Google Messages 处理消息路由有一个潜在的巨大优势。这可能意味着所有通过第三方消息应用程序发送的 RCS 消息将使用谷歌的聊天服务，这是迄今为止使用最广泛的 RCS 实现，因为没有一个运营商的版本已经起飞。

我们还没有发现谷歌关于这个 Android 消息 API 的声明，但我们希望它能很快开放。第三方短信应用目前处于劣势，因为它们缺乏 RCS 支持，但这个 API 将意味着你可以使用你最喜欢的短信应用，并享受 RCS 的好处。当然，第三方短信应用程序必须实际实现新的 API，但看起来实现起来不会太难。

* * *

## 更新 1: API 仅在三星版本的应用程序中发现

在我们发表这篇文章后不久，我们了解到 Android Messages API 的字符串和清单条目只能在三星 Galaxy 手机的 [Google Messages 应用程序](https://www.xda-developers.com/google-messages-galaxy-s21-one-ui-design/)中找到。这是相同的应用程序和包名称，但 Google Play 动态地向三星 Galaxy 手机推出这一版本的应用程序。这些条目是在几个版本之前添加的，所以 API 本身似乎并不新鲜。我们不确定为什么这些条目只出现在三星手机的应用程序版本中，但有可能谷歌制作了这个 API，以便三星的消息应用程序可以使用谷歌的聊天服务，而用户无需切换应用程序。然而，我们不明白为什么这个 API 不能对其他应用开放，我们也没有看到三星 Messages 应用本身使用这个 API 的任何证据。希望谷歌将 API 开放给所有第三方消息应用程序，将其包含在应用程序的主版本中。

* * *

## 更新 2: API 仅限于三星应用

深入挖掘谷歌消息应用程序(h/t[*9 到 5 谷歌*](https://9to5google.com/2021/07/09/google-messages-permission-samsung-message-continuity/) )，我们发现有证据表明，这种 Android 消息 API 目前仅限于部分三星应用程序使用。具体来说，这项功能似乎旨在让三星可穿戴设备和联网平板电脑通过谷歌消息发送短信、彩信和 RCS 消息。这是三星呼叫&消息连续性功能的一部分。

当前的允许列表包括呼叫和消息连续性的包，即。“com . Samsung . Android . mdec service”，以及其他应用程序。该代码在授予对 API 的访问权限之前检查请求应用程序的包名和签名。一个标志允许任何应用程序访问 API，但是这个值显然不打算公开使用。(该标志被恰当地命名为“allow _ any _ app _ to _ connect _ do _ not _ use _ in _ public _ builds”。)

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*