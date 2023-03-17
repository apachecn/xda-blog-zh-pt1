# 小米正在开发超宽带供电的“魔控桥”

> 原文：<https://www.xda-developers.com/xiaomi-is-developing-uwb-powered-magic-control-bridge-for-controlling-mi-tvs/>

小米在过去几年中一直在建立其智能家居生态系统，特别是在电视领域。该公司长期以来一直销售机顶盒，现在提供一系列 Mi 电视型号，如我们今年早些时候评论的 QLED 4K 电视。根据小米之家新版应用的代码，小米正在开发一款新的“魔法控制桥”配件，如果你对拿起物理遥控器不够感兴趣，它将允许小米电视周围的任何人从兼容的手机或平板电脑上控制它。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

*感谢 PNF 软件为我们提供了使用* [*JEB 反编译*](https://www.pnfsoftware.com/?aid=xdadev) *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*

我们拆开了小米 Mi Home 应用的 v6.9.601 更新，其中包含引用“魔法控制桥”的文本字符串。该设备显然可以连接到任何 2.4GHz 的 Wi-Fi 网络(但不是 5GHz)，或使用 USB 连接直接连接到电视。一旦设置完成，它将允许范围内的任何人使用超宽带(UWB)连接来控制 Mi 电视产品。如果你愿意，你也可以把它限制在你家里的家庭成员之间。

```
 <string name="uwb_permission_group">Permissions</string>
<string name="uwb_permit_dialog_all_desc">When everyone comes close to the UWB device, the device can be found and controlled via Magic Control.</string>
<string name="uwb_permit_dialog_title">Permissions for Magic Control</string>
<string name="uwb_permit_group_all">Everyone</string>
<string name="uwb_permit_group_home">Family members in same home</string>
<string name="uwb_reset">Reset</string>
<string name="uwb_support_device_title">Magic Control Device</string>
<string name="uwb_tag_need_reset_stranger_msg">The device has already been connected to Magic Control Bridge. Please press and hold the device reset button for 7 seconds to reset the device and try to connect again.</string>
<string name="uwb_tmp_no_device">No equipment</string>
<string name="uwb_user_guide">"Go to view the Beginner's Guide >"</string>
<string name="uwb_wifi_not_enabled">Please turn on the Wi-Fi.</string>
<string name="uwb_wifi_not_valid_5g">Magic Control Bridge Mate does not support 5G network, please switch the network to 2.4G</string> 
```

这款设备听起来将提供与谷歌 Android TV 远程应用类似的功能，但可能不需要远程设备在同一个 Wi-Fi 网络上或连接到同一个小米账户。该功能反映了[小米去年为 UWB 技术创造的一个演示](https://blog.mi.com/en/2020/10/13/xiaomi-introduces-groundbreaking-uwb-technology/)，展示了如何将手机指向电视，可以在手机上调出遥控器。目前还没有证据表明 Magic Control 设备将允许远程控制其他设备，但也许以后可以通过软件更新添加这一功能。

这座桥似乎需要 UWB 硬件支持，小米目前没有出售任何带 UWB 的手机或平板电脑。小米的 Mi MIX 4 可能会在 8 月 10 日宣布[，据信它将拥有](https://m.weibo.cn/detail/4666853962815638)[所需的超宽带芯片](https://www.xda-developers.com/xiaomi-next-flagship-uwb-tracking-support/)，以及[折叠屏幕和下显示摄像头](https://www.xda-developers.com/xiaomi-mi-mix-4-flexible-screen-under-display-camera/)。在那之前，你将不得不坚持使用一个无聊的旧遥控器。