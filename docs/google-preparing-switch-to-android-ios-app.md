# 谷歌似乎正在为 iOS 开发一款“切换到安卓”应用

> 原文：<https://www.xda-developers.com/google-preparing-switch-to-android-ios-app/>

**更新 1 (07/28/2021 @ 00:22 AM ET):** 我们已经添加了数据恢复工具应用中提到的功能的截图。[点击这里了解更多信息。](#update1)这篇文章发表于美国东部时间 2021 年 7 月 27 日上午 08:20，保存如下。

如果你正在从安卓系统转移到 iOS 系统，苹果在谷歌 Play 商店提供了一款名为 Move to iOS 的应用，让你可以无缝地将安卓系统的数据转移到 iPhone 上。但是如果你想反其道而行之——从 iOS 转到 Android——谷歌目前在苹果的应用商店没有类似的工具。但最终，谷歌似乎准备好了一个竞争对手。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

随着 Android 12 Beta 3 的发布，谷歌[修改了 SetupWizard](https://www.xda-developers.com/android-12-beta-3-features/#android12beta3_revampedsetup) UI，以更好地适应 Material You 指南。在设置过程中，SetupWizard 会启动一个系统应用程序，负责帮助用户从旧手机中恢复数据。这款名为数据恢复工具的应用程序[最近发布到了 Google Play](https://play.google.com/store/apps/details?id=com.google.android.apps.restore) ，并且 1.0.382048734 版本的更新包含暗示谷歌希望帮助 iPhone 用户转向 Android 的字符串。

```
 <string name="ios_wifi_hotspot_instructions_first_step">Step 1:</string>
<string name="ios_wifi_hotspot_instructions_first_step_message">Get the <b>Switch to Android</b> app from the App Store®</string>
<string name="ios_wifi_hotspot_instructions_second_step">Step 2:</string>
<string name="ios_wifi_hotspot_instructions_second_step_message">Go to your Wi-Fi settings</string>
<string name="ios_wifi_hotspot_instructions_third_step">Step 3:</string>
<string name="ios_wifi_hotspot_instructions_third_step_message">Connect to network <b>^1</b> and enter password <b>^2</b></string>
<string name="ios_wifi_hotspot_instructions_title">Follow these steps on your iPhone</string> 
```

这些字符串告诉用户从 App Store 下载一个“切换到 Android”应用程序，然后进入 iPhone 上的 Wi-Fi 设置，使用 Wi-Fi 热点连接到 Android 手机。这类似于移动到 iOS 应用程序的工作方式。

尚不清楚用户将能够传输何种数据，但我们发现了额外的字符串，表明该工具将帮助您传输 WhatsApp 聊天等内容。

```
 <string name="ios_whatsapp_description">Scan the QR code with your iPhone to open WhatsApp, then tap <b>Start</b></string>
<string name="ios_whatsapp_export_description">Keep your iPhone unlocked and WhatsApp open</string>
<string name="ios_whatsapp_export_title">Getting chats ready…</string>
<string name="ios_whatsapp_message">Trouble scanning? On your iPhone, open WhatsApp, then go to <b>Settings > Chats > Move Chats to Android</b></string>
<string name="ios_whatsapp_title">Transfer WhatsApp chats</string> 
```

据我们所知，看起来你不太可能使用开关将你的 WhatsApp 聊天转移到 Android 应用程序本身。相反，该应用程序只会提供有用的指导，说明如何使用 WhatsApp 的[即将推出的“将聊天转移到 Android”](https://www.xda-developers.com/whatsapp-phone-number-transfer-chats/)功能来迁移 WhatsApp 的数据。

最后，一些字符串指向支持迁移支持的应用程序，但似乎只有在你的 iPhone 没有加密的情况下才有效。我们推测，谷歌会将发布在 Google Play 上的应用程序与安装在用户 iPhone 上的应用程序相匹配，因此尽管这将有助于迁移两个平台上最受欢迎的应用程序，但它不会迁移所有应用程序。

```
 <string name="fragment_ios_decryption_description">To transfer apps, SMS messages, and contacts, enter your iTunes® backup password</string>
<string name="fragment_ios_device_management_detected_description">"Your iPhone® is managed by your organization and has encrypted content. To transfer apps, iCloud® contacts, device contacts, and iMessage® messages, you’ll need to remove device management on your iPhone®."</string>
<string name="fragment_ios_skip_encrypted_data_dialog_description">Your apps, iCloud® contacts, device contacts, and iMessage® messages won’t transfer</string> 
```

谷歌目前[维护着一个名为“切换到 Android”](https://www.android.com/switch/)的页面，该页面解释了 iPhone 用户如何使用 Google Drive 应用程序备份他们的联系人、照片、视频和日历事件。这不像苹果为那些转向 iOS 的用户提供的那样方便或无缝，所以转向 Android 应用程序可能最终会弥合这一差距。在应用商店搜索谷歌公司的“切换到安卓”应用没有结果，查看该公司的[完整应用列表](https://apps.apple.com/us/developer/google-llc/id281956209#see-all/i-phonei-pad-apps)也没有结果，所以这款应用似乎还没有推出。

* * *

## 更新 1:截图

Android 应用程序开发人员和逆向工程师 Alessandro Paluzzi 分享了一些包含我们在数据恢复工具应用程序中发现的字符串的片段截图。这些片段要求用户在 App Store 上安装尚未发布的 Switch to Android 应用程序，并告诉用户输入他们的 iCloud 密码来解密他们的数据。

在另一条推特上，WABetaInfo 分享了数据恢复工具 WhatsApp 聊天传输部分的图像。