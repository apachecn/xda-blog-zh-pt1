# Google Play 服务现在允许您删除您的广告 ID

> 原文：<https://www.xda-developers.com/google-play-services-delete-ad-id-opt-out-personalization/>

**更新 2 (09/16/2021 @美国东部时间下午 1:44):**您现在可以在 Google Play 服务中删除您的广告 ID。[点击这里了解更多信息。](#update2)文章发表于 2021 年 6 月 3 日，下面保留。

### 以前的更新

**更新 1 (07/28/2021 @美国东部时间下午 4:49):**谷歌分享了一张图片，展示了在 Android 12 的 Google Play 服务设置中删除你的广告 ID 的样子，他们还为开发者透露了一个新的应用集 ID SDK。[点击这里了解更多信息。](#update1)

Google Play 服务为所有选择广告个性化的用户生成一个广告 ID。这个 ID 不仅可以帮助谷歌向用户推送相关广告，还可以方便地用于分析和欺诈防范。当你关闭你的账户上的广告个性化时，谷歌停止使用你的广告 ID 来推送个性化广告，但它仍然保留它用于其他目的。然而，这种情况很快就会改变。

目前，你可以在 Android 设备上进入设置>谷歌>广告或设置>隐私>高级>广告，退出个性化广告。一旦你这样做了，Google Play 服务将停止向你的设备推送个性化广告推荐，但你手机上的应用程序仍然可以看到广告 ID。但是 Play 控制台帮助页面上的[最近更新显示，当你选择退出基于兴趣的广告时，Google Play 服务将很快删除广告 ID。更新声明:*“从 2021 年末开始，当用户选择退出基于兴趣的广告或广告个性化时，广告标识符将不可用。您将收到一串零来代替标识符。*](https://support.google.com/googleplay/android-developer/answer/6048248)

这一改变生效后，如果你禁用个性化广告，你手机上的应用程序将看到一串零，而不是你的广告 ID。Google Play 服务还会提醒所有可以访问您的广告 ID 和相关数据的应用程序，以便删除任何现有数据。在开发者 *kdrag0n* 分享的[通知](https://notifications.google.com/g/vib/AD-FnExHmpB-dOD5WpYWCKq4qIWOm8zGkEhuk06EURxvFoOM2g4jONDr4Y6oQwMqqJQN_UtNgJzrUiXa202OKzpM-ImnD4MfFErVIkQC3CMAVnrx65z367fCCv9IdyZwu0R67Vf3EWvTPaCxjeKnf0Q7MlNCJMbZI3YDqkp9R4KbPQWA7ji2DJjrHqvaX7Ii_HcM4Y1HRltRpbQ)中，谷歌进一步透露*“这一 Google Play 服务分阶段推出将影响 2021 年末开始在 [Android 12](https://www.xda-developers.com/android-12/) 设备上运行的应用，并将在 2022 年初扩展到支持 Google Play 的设备上运行的应用。7 月，我们将提供更多细节和替代解决方案，以支持分析和欺诈防范等基本使用情形。”*

目前，我们没有任何关于谷歌将推出的分析和欺诈防范替代解决方案的信息。我们会尽快更新这篇文章。

*感谢开发者 [kdrag0n](https://twitter.com/kdrag0n) 的提示！*

* * *

## 更新 1:2021 年 7 月政策更新期间分享的更多详细信息

在该公司最新的 PolicyBytes 视频中，概述了 Google Play 即将到来的政策变化，谷歌分享了更多关于广告 ID 及其分析和欺诈防范替代物的细节。

首先，谷歌展示了删除广告 ID 的选项会是什么样子，这项功能将通过今年晚些时候的 Google Play 服务更新推广到 Android 12 设备。

该公司还用一些新信息更新了其广告 ID 上的支持页面。对于任何需要在用户删除广告 ID 时得到通知的开发者，谷歌让你在这里注册通知系统。Google 还表示，将目标 API 级别更新为 31 的应用程序需要在其清单中声明以下权限来查询广告 ID:

```
 <uses-permission android:name="com.google.android.gms.permission.AD_ID"/> 
```

一些 SDK 可能已经声明了这种许可，但是应该注意的是，家族策略禁止使用广告 ID。在这种情况下，您必须通过在清单中包含以下元素来防止权限合并到您的应用程序中:

```
 <uses-permission android:name="com.google.android.gms.permission.AD_ID" tools:node="remove"/> 
```

接下来，谷歌分享了一些基本用例替代解决方案的细节，如分析和欺诈防范。称为[应用集 ID](https://developer.android.com/training/articles/app-set-id) ，这个 ID 是设备上同一开发者的所有应用的唯一标识符。谷歌称这是一个“隐私友好的选项”，可以将您组织拥有的一系列应用程序的使用或操作关联起来，它**不得**用于广告个性化或广告测量，不得出于广告目的连接到任何 Android 标识符或任何个人和敏感数据，并且其收集必须以“合法充分的隐私通知，包括您的隐私政策”向用户披露

如果应用程序是从 Google Play 以外的来源安装的，如果 Google Play 服务无法确定应用程序的开发人员帐户，或者如果应用程序安装在没有安装 Play 服务的设备上，则应用程序集 ID SDK 将返回调用应用程序本身的唯一 ID。如果共享相同 ID 的应用程序组超过 13 个月未访问 API，如果给定应用程序集中的最后一个应用程序被卸载，或者如果用户工厂重置设备，则应用程序集 ID 会自动清除。该功能的开发者预览版现已上线，尽管谷歌警告称，由于可能会发生变化，应用集 ID API 不应用于生产应用。

有关更多信息，请阅读今天发布的[完整开发者计划政策更新](https://support.google.com/googleplay/android-developer/answer/10808976?hl=en&ref_topic=9877065)或观看下面嵌入的“PolicyBytes”视频，该视频总结了最重要的变化。

* * *

## 更新 2:现在推出

Google Play 服务现在推出了删除设备广告 ID 的功能，前提是你的设备运行的是 Android 12。我们的一个线人@panduu221 在 Twitter 上告诉我们，他们现在有这个功能了。我们检查了我们自己的 Android 12 设备，并确认新的“删除广告 id”页面现在可见。这项功能的推出很可能是由服务器端的标志控制的，但值得一提的是，我们的设备有 21.36.14 版本的 Google Play 服务应用程序。