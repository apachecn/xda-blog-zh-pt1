# 谷歌可能正在开发苹果“查找我的”网络的安卓版本

> 原文：<https://www.xda-developers.com/google-find-my-device-network/>

因为苹果严格控制着 iOS 生态系统，他们能够建立一个巨大的众包设备网络，帮助定位其他设备。像许多其他公司一样，苹果公司最近发布了一款蓝牙追踪器，多亏了 Find My network， [AirTags](https://www.xda-developers.com/apple-airtags-review/) 可以说是市场上最有效的追踪器。由于几乎每台 Android 设备上都安装了 Google Play 服务应用程序，谷歌是唯一一家能够建立像苹果一样庞大的设备网络的公司。似乎谷歌认识到了这一事实，并准备建立自己的众包设备网络。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Google Play 服务版本 21.24.13 今天在测试频道推出，在我们解码后，我们发现添加了以下字符串:

```
 <string name="mdm_find_device_network_description">Allows your phone to help locate your and other people’s devices.</string>
<string name="mdm_find_device_network_title">Find My Device network</string> 
```

新字符串清楚地表明，谷歌正在开发一个“查找我的设备”网络，利用 Google Play 服务“[允许]你的手机定位你和其他人的设备。”谷歌已经在 Play Store 上提供了一个名为“查找我的设备”的应用程序，但它只能找到登录到你的谷歌帐户的设备。如果这个“查找我的设备”网络上线，那么你将能够帮助其他 Android 用户定位他们丢失或被盗的设备。

虽然 Android 可以在许多不同类型的设备中找到，但在全球超过 30 亿台运行该操作系统的设备中，很可能有很大一部分是智能手机。在中国以外销售的绝大多数 Android 智能手机都预装了 Play Services 应用程序，这可能意味着它们将有资格参与“查找我的设备”网络。作为背景，Google Play 服务是谷歌移动服务(GMS)的关键组成部分之一，GMS 是谷歌制造的一套应用和服务，该公司将其分发给寻求销售 Android 设备的智能手机制造商。GMS 还捆绑了 Android 生态系统中最大的应用商店 Play Store。寻求在 Android 设备上预装 Play Store 的设备制造商还必须包括谷歌移动服务的许多其他组件，包括谷歌 Play 服务和其他应用程序。

我们还没有这个“查找我的设备”网络的更多细节，但我们将继续挖掘最新的 Google Play 服务版本，如果我们了解到更多信息，将更新本文。我们特别有兴趣了解更多关于设备兼容性的信息，以及是否会选择加入或退出。