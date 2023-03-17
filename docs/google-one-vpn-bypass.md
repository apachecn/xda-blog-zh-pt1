# Google One 准备让你选择哪些应用应该绕过它的 VPN

> 原文：<https://www.xda-developers.com/google-one-vpn-bypass/>

# Google One 准备让你选择哪些应用应该绕过它的 VPN

谷歌正在测试 Android 版 Google One 应用的一项新功能，该功能将允许用户绕过其内置 VPN 的某些应用。

Google One 是谷歌不太知名的服务之一。首先，它是谷歌的付费云存储服务，计划从 100GB 到 30TB 不等。随着 Google Photos 从 6 月 1 日开始设置为[免费无限制备份](https://www.xda-developers.com/psa-google-photos-will-no-longer-offer-free-unlimited-storage-next-year/)，人们对 Google One 及其各种计划重新产生了兴趣。从 Google One plan 购买的存储空间可用于 Google 相册和各种 Google 服务，包括 Drive、Gmail 和 Docs。此外，谷歌还在更高层次的 [Google One 计划](https://one.google.com/about/plans)中加入了一些赠品，比如在谷歌商店购物最高可获得 10%的返现。去年 10 月，谷歌为顶级计划的用户增加了另一项漂亮的额外待遇:接入虚拟专用网[。该 VPN 服务适用于 2TB 及以上计划的 Google One Android 用户。自首次亮相以来，VPN 服务没有获得任何新功能或改进。但看起来这种情况很快就会改变。](https://www.xda-developers.com/google-one-2tb-plan-vpn-perk-online-privacy/)

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

在最新版本的谷歌 Android One 应用程序中，我们发现有证据表明，该应用程序将很快允许用户绕过 VPN 的某些应用程序。目前，谷歌 One 应用程序中的 VPN 服务不允许你将特定的应用程序列入白名单。如果由于 VPN 的原因，某个应用程序不能正常工作或表现异常，你唯一的选择就是完全关闭该服务。

以下字符串表示用户可以将特定应用程序添加到绕过列表中。添加到绕过列表的应用将忽略 VPN，并从您的手机网络路由其流量。

```
 <string name="app_bypass">Bypass VPN</string>
<string name="app_bypass_card_description">Your changes will take effect once the VPN is enabled</string>
<string name="app_bypass_dialog_message">This will restart the VPN</string>
<string name="app_bypass_save_description">&lt;b> Save changes. &lt;/b> This will restart the VPN.</string>
<string name="app_bypass_title">Allow apps to bypass VPN</string>
<string name="apps_bypassed_description">Allow specific apps to bypass the VPN when it is connected</string>
<string name="apps_bypassed_header">Apps bypassing VPN</string>
<string name="no_apps_bypass">No apps</string>
<string name="ppn_add_app_content_description">Add %1$s to the bypass list</string>
<string name="ppn_app_bypass_card_description">"You can allow specific apps to ignore the VPN and use your phone's network"</string>
<string name="ppn_app_bypass_card_title">"Using your phone's network"</string>
<string name="ppn_remove_app_content_description">Remove %1$s from the bypass list</string> 
```

这项功能并没有在最新版本的谷歌安卓应用中使用。如果它上线了，我们会让你知道的。请注意，Google One 中的 VPN 服务目前仅在美国可用。