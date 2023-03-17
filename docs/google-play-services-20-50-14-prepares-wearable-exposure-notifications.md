# Google Play 服务准备添加可穿戴曝光通知

> 原文：<https://www.xda-developers.com/google-play-services-20-50-14-prepares-wearable-exposure-notifications/>

回到去年 8 月，我们得知蓝牙特别兴趣小组(SIG)正在制定新的 BLE 规范,该规范将使智能手表等可穿戴设备上的联系人追踪成为可能。为了开发这一新规范，130 多家蓝牙成员公司组成了蓝牙 SIG 暴露通知工作组(ENWG)。当时，蓝牙 SIG 还宣布，它将在未来几个月内发布新蓝牙规范的初步草案，以供审查。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

正如承诺的那样，标准机构[上个月公布了可穿戴暴露通知服务(WENS)规范的草案](https://www.bluetooth.com/wp-content/uploads/2020/12/WENS_Wearable_Exposure_Notification_Service_Draft_Specification.pdf)。该草案强调了新的蓝牙规范，这将使*“一个非互联网连接的可穿戴设备能够以一种与一个或多个部署的基于客户端的暴露通知系统(ENSs)互补的方式运行，从而使更多的人能够参与 ENSs。”*尽管蓝牙 SIG 尚未最终确定这一新规范，但最新的 Google Play 服务更新的拆解显示，谷歌已经开始致力于为该应用程序添加可穿戴暴露通知支持。

Google Play 服务 v20.50.14 最近开始在 Play Store 上推出。它包括以下新字符串，揭示了即将推出的可穿戴式曝光通知支持的一些细节:

```
 <string name="exposure_notification_pair">Pair</string>
<string name="exposure_notification_pair_fail_dialog">Pair failed! Please try again.</string>
<string name="exposure_notification_pair_new_device">Pair new device</string>
<string name="exposure_notification_paired_devices">Paired devices</string>
<string name="exposure_notification_pairing">Pairing…</string>

<string name="exposure_notification_wearable_available_devices">Available devices</string>
<string name="exposure_notification_wearable_device_list">Get notified on paired devices</string>
<string name="exposure_notification_wearable_device_name">Device name</string>
<string name="exposure_notification_wearable_pair_dialog_message">"Your phone will use this device to securely collect and share random IDs with other devices that are nearby.

You can be notified if you’ve been near someone who reported having COVID-19.

The date, duration, and signal strength associated with an exposure will be shared with the app.
"</string>
<string name="exposure_notification_wearable_pair_dialog_title">Pair %s for COVID-19 Exposure Notification?</string> 
```

前面提到的字符串包括几个对话框，突出显示了配对过程，这将帮助用户连接支持的可穿戴设备以接收暴露通知。与新设备配对后，用户将看到一个对话框，显示:*“您的手机将使用此设备安全地收集随机 id，并与附近的其他设备共享。* *如果你身边有人报告患有新冠肺炎，你会收到通知。* *与曝光相关的日期、持续时间和信号强度将与应用程序共享。”*

截至目前，谷歌尚未就此事发布任何官方信息。但由于该公司已经开始致力于为 Google Play 服务添加可穿戴曝光通知支持，我们预计将在未来几周内看到正式声明。