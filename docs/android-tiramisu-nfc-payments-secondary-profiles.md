# Android 13“提拉米苏”可能会让二级配置文件进行 NFC 支付

> 原文：<https://www.xda-developers.com/android-tiramisu-nfc-payments-secondary-profiles/>

虽然谷歌尚未推出稳定的 Android 12 版本，但我们已经开始看到关于下一个 Android 大版本的信息——Android 13。昨天我们得知，谷歌[已经为 Android 13 确定了甜点名](https://www.xda-developers.com/google-android-13-t-tiramisu-dessert-name/)。我们现在发现的证据表明，下一个版本的 Android 可能最终会允许第二个人资料进行非接触式支付。

Android 已经支持多用户好几年了，但二级配置文件很长时间以来一直缺少一个功能——配置 NFC 支付的能力。然而，这可能会在下一个 Android 版本中发生变化。我们在 AOSP Gerrit 上发现了[新的承诺](https://android-review.googlesource.com/q/topic:multi_user)，一旦合并到 AOSP，可能会增加对二级用户非接触式支付的支持。

提交具有以下描述:

> 支持多用户 NFC 支付
> 
> 根据不同用户配置 nfc 支付设置。

这些提交会修改设置应用程序，以允许设备上的二级配置文件设置自己的非接触式支付服务。在当前的 Android 版本中，该设置仅适用于设备所有者，不会出现在二级用户或访客中。您可以在所有者档案中导航至*设置>连接设备>连接偏好设置> NFC >非接触式支付*来找到设置。一旦谷歌在 Android 13 中为二级配置文件启用该功能，它也将对其他配置文件可用。我们可以确认，Android 12 中的二级配置文件中缺少“非接触式支付”设置。

如果你与其他家庭成员共享你的设备，并设置了单独的配置文件，这将非常有用，因为每个成员都可以设置自己单独的支付方式，并进行 NFC 支付。

目前对 Android 13 提拉米苏还知之甚少，但我们会密切关注新的进展。如果我们发现有趣的东西，我们会确保让你知道。与此同时，请继续关注 XDA 的更多报道。

* * *

*感谢 XDA 公认的开发者 [luca020400](https://forum.xda-developers.com/m/luca020400.5778309/) 的提示！*