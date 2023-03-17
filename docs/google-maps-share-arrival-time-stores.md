# 谷歌地图准备让你与商店分享你的到达时间

> 原文：<https://www.xda-developers.com/google-maps-share-arrival-time-stores/>

# 谷歌地图准备让你与商店分享你的到达时间

谷歌地图正在开发一项名为“辅助取件”的新功能，它可以让你与商店分享你的到达时间，以便更快地取件。

谷歌地图正在开发一项新功能，可以让你与商店分享你的到达时间，以加快提货速度。我们在谷歌地图 10.72 版本的拆解中发现了即将推出的功能，该版本最近开始通过 Play Store 推出。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

正如您在附加字符串中看到的，辅助提货功能将为您提供一个选项，将您的订单添加到谷歌地图，并与商店共享您的到达时间，以便更快地提货。该应用程序将自动与商店分享您的预计到达时间，直到您到达商店。

```
 <string name="ASSISTIVE_PICKUP_ACTIVATION_SIGN_IN_PAGE_SUBTITLE">Sign in to add your order to Maps, for a faster pickup later</string>
<string name="ASSISTIVE_PICKUP_ACTIVATION_SIGN_IN_PAGE_TITLE">Save time at pickup</string>
<string name="ASSISTIVE_PICKUP_ARRIVAL_CHECK_IN_BUTTON_TEXT">Check in</string>
<string name="ASSISTIVE_PICKUP_ARRIVAL_CHECK_IN_SUBTITLE">Check in with the store so they can bring your order directly to you</string>
<string name="ASSISTIVE_PICKUP_ARRIVAL_CHECK_IN_TITLE">Pick up your order</string>
<string name="ASSISTIVE_PICKUP_ETA_PROMPT_OK">OK</string>
<string name="ASSISTIVE_PICKUP_ETA_SHARE_BUTTON">Share arrival time</string>
<string name="ASSISTIVE_PICKUP_ETA_SHARING_CONFIRMATION_PROMPT_TEXT">Sharing arrival time until you get to the store</string>
<string name="ASSISTIVE_PICKUP_ETA_SHARING_EXIT_PROMPT_EXIT_BUTTON">Exit</string>
<string name="ASSISTIVE_PICKUP_ETA_SHARING_EXIT_PROMPT_TEXT">"You'll also stop sharing your arrival time with the store"</string>
<string name="ASSISTIVE_PICKUP_ETA_SHARING_EXIT_PROMPT_TITLE">Exit navigation?</string>
<string name="ASSISTIVE_PICKUP_ETA_SHARING_IN_PROGRESS">Sharing estimated time of arrival</string>
<string name="ASSISTIVE_PICKUP_ETA_UNSHARE_BUTTON">Stop sharing arrival time</string>
<string name="ASSISTIVE_PICKUP_MORE_INFORMATION_DIALOG_BODY">Pickup orders are created from confirmations sent to your Gmail. You can turn this off in settings any time.</string>
<string name="ASSISTIVE_PICKUP_MORE_INFORMATION_DIALOG_BUTTON_TEXT">OK</string>
<string name="ASSISTIVE_PICKUP_MORE_INFORMATION_DIALOG_LEARN_MORE">Learn more about orders on Maps</string>
<string name="ASSISTIVE_PICKUP_MORE_INFORMATION_DIALOG_SETTINGS">Go to settings</string>
<string name="ASSISTIVE_PICKUP_MORE_INFORMATION_DIALOG_TITLE">Pickup orders on Maps</string>
<string name="ASSISTIVE_PICKUP_NAVIGATION_SHARING_NOTICE_PROMPT_ANOTHER_DEVICE_SUBTITLE">On another device</string>
<string name="ASSISTIVE_PICKUP_NAVIGATION_SHARING_NOTICE_PROMPT_CANCELED_SUBTITLE">Not available for pickup</string>
<string name="ASSISTIVE_PICKUP_NAVIGATION_SHARING_NOTICE_PROMPT_CANCELED_TITLE">Order canceled</string>
<string name="ASSISTIVE_PICKUP_NAVIGATION_SHARING_NOTICE_PROMPT_CHECKED_IN_TITLE">Already checked in</string>
<string name="ASSISTIVE_PICKUP_NAVIGATION_SHARING_NOTICE_PROMPT_PICKED_UP_TITLE">Order picked up</string>
<string name="ASSISTIVE_PICKUP_NAVIGATION_SHARING_NOTICE_PROMPT_UNKNOWN_SUBTITLE">Continue and check in at the store</string>
<string name="ASSISTIVE_PICKUP_NAVIGATION_SHARING_NOTICE_PROMPT_UNKNOWN_TITLE">"Can't share arrival time"</string>
<string name="ASSISTIVE_PICKUP_SHARE_DIALOG_BODY">Share your arrival with %s while you drive, and get your order even faster. Your real-time location is never shared.</string>
<string name="ASSISTIVE_PICKUP_SHARE_DIALOG_CANCEL_BUTTON_TEXT">Not now</string>
<string name="ASSISTIVE_PICKUP_SHARE_DIALOG_LEARN_MORE">Learn more about sharing arrival time</string>
<string name="ASSISTIVE_PICKUP_SHARE_DIALOG_SHARE_BUTTON_TEXT">Share arrival time</string>
<string name="ASSISTIVE_PICKUP_SHARE_DIALOG_TITLE">Ready to go?</string> 
```

一旦该功能启用，您将能够根据发送到您 Gmail ID 的确认创建收件订单，并且您还可以随时在“设置”中选择关闭该功能。此外，该功能还将包括一个“签到”选项，帮助您在商店*签到，“这样他们就可以直接把您的订单送到您这里。”*字符串还指出，该功能不会在任何给定时间与商店共享您的实时位置。我们还发现了一个描述拆卸过程中辅助拾取功能的图像，如下所示:

一旦 Assistive Pickup 在稳定频道推出，谷歌地图将向您展示一张卡，突出显示新功能。它将包括帮助您开始使用新功能的快速说明。目前，该功能尚未在最新的谷歌地图版本中上线。我们会尽快更新这篇文章，只要它开始推出未来的更新。

谷歌地图在过去几周内获得了大量新功能。其中包括[改进的实时视图](https://www.xda-developers.com/googles-improved-live-view-allows-people-to-explore-the-city-better-than-before-via-ar/)、[新的环保和安全功能](https://www.xda-developers.com/google-maps-is-adding-new-eco-friendly-and-safety-features/)，以及[提供更丰富信息的定制体验](https://www.xda-developers.com/google-maps-gets-tailored-experience-richer-info-and-more/)。您可以通过上面的链接了解更多关于这些功能的信息。