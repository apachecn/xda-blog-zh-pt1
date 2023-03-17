# “查找我的设备”应用程序泄露了谷歌众包追踪网络的信息

> 原文：<https://www.xda-developers.com/find-my-device-network-new-info/>

6 月中旬，我们首先报道了谷歌正在开发一个“ [Find My Device Network](https://www.xda-developers.com/google-find-my-device-network/) ”，本质上是苹果“Find My network”的安卓版本。我们在 Google Play 服务应用程序中发现的字符串表明，该网络将允许您的手机帮助定位您和其他人的设备。除了字符串和一些名为“Spot”的 API 的代码引用，Play Services 应用程序中没有太多其他细节。然而现在，谷歌“查找我的设备”应用程序的新更新包含大量引用该功能的字符串，揭示了谷歌即将推出的众包跟踪网络的更多信息。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

今天早些时候， [Google Find My Device app](https://play.google.com/store/apps/details?id=com.google.android.apps.adm) 的 2.4.043_df 版本发布。解码 APK 后，我们发现了多个引用“查找我的设备网络”和“点”的字符串字符串揭示了用户如何将设备标记为丢失或找到；添加还可以跟踪您的设备的“共同所有者”；导出、导入和扫描加密密钥以共享您的设备，等等。

“查找我的设备”应用程序不仅会显示设备最后一次被发现的时间，还会显示它是否就在附近。

```
 <string name="spot_device_status_in_range">Near you right now</string>
<string name="spot_device_status_located_lately_not_in_range">Last seen: %1$s. Does not seem to be near you now.</string>
<string name="spot_device_status_located_now_not_in_range">Last seen just now. Does not seem to be near you.</string> 
```

如果您丢失了设备，您可以在“查找我的设备”应用程序中将它标记为丢失。找到后，您可以将其标记为已找到。

```
 <string name="mark_lost">Mark as Lost</string>
<string name="unmark_lost">Mark as Found</string> 
```

当然，一旦您的设备失去互联网连接或退出任何其他登录设备的蓝牙范围，它就不能仅由您自己的设备跟踪。这就是众包查找我的设备网络的用武之地。当你将设备标记为丢失时，你将获得“众包协助寻找”据推测，附近其他启用了 Google Play 服务的 Android 手机——即。几乎所有的安卓手机都可以在谷歌的“查找我的设备”网络上默默标记丢失设备的位置。

然后，当你标记为丢失的设备被发现时，你会收到来自“查找我的设备”应用程序的通知，谷歌将尝试在发现该设备时给该设备打电话。找到丢失设备的人不会收到有关该设备所有者的任何信息，从而保护了所有者的隐私。

```
 <string name="spot_mark_as_lost_explanation_header">You are about to mark this device as lost. This will have the following effects:</string>
<string name="spot_mark_as_lost_suggestion">Try marking the device as lost to get crowdsourced assistance in finding it.</string>
<string name="spot_lost_device_owner_notifications_explanation">You will get notifications when this device is sighted by another member of the Find My Device Network.</string>
<string name="spot_lost_device_ringing_explanation">We will attempt to ring the device at the time of the sighting.</string>
<string name="spot_lost_device_sighter_notifications_explanation">When this happens, the sighting user will be notified that they helped a fellow member of the network, without exposing your identity.</string>
<string name="spot_alerts_channel_description">Shown when a device you have marked as lost is sighted.</string>
<string name="spot_alerts_channel_name">Alerts</string> 
```

一旦丢失的设备被找到，拥有者可以通过导航到最后发现它的位置(或通过与找到它的人见面)来捡起它。然而，设备的所有者不一定是唯一能够捡起丢失设备的人。“查找我的设备”应用程序提示您可以添加设备的“共同所有者”，这些共同所有者将能够看到您标记为丢失的任何设备的位置。

不过，添加共有人需要事先做一些设置。你必须生成一个嵌入在二维码或文件中的加密密钥，你需要将它存储在设备之外，如外部存储驱动器、云或纸上。

```
 <string name="spot_device_sync">Sync encryption key</string>
<string name="spot_device_sync_needed">Location and other functionality not available. You need to synchronize encryption key for it to work.</string>
<string name="spot_export_owner_key_button_text">Export</string>
<string name="spot_export_owner_key_data_format">"Find My Device Network encryption key #%1$s for %2$s generated on %3$s on %4$s.
Please store this key for future use."</string>
<string name="spot_export_owner_key_description">Press the button to store the encryption key. We recommend storing the encryption key for future use in a safe place separately from this device, on a removable storage, on a cloud storage, or printed.</string> 
```

为了添加共同所有者，您需要向他们发送二维码或包含加密密钥的文件。潜在的共同所有者需要扫描 QR 码或导入加密密钥文件。

```
 <string name="spot_display_one_time_sharing_key_qr_code_description">To complete the sharing process of %1$s, please let %2$s scan the QR code below, which contains a cryptographic key required for sharing.</string>
<string name="spot_import_owner_key_camera_scan">"Import encryption key by scanning QR code with camera.
Choose this option if the encryption key is displayed on another device or printed."</string>
<string name="spot_import_owner_key_done">Encryption key import completed</string>
<string name="spot_import_owner_key_failed">Failed to import encryption key</string>
<string name="spot_import_owner_key_for_a_device_method_title">%1$s require(s) encryption key 
<string name="spot_import_owner_key_method_title">Please select import method</string>
<string name="spot_import_owner_key_open_file">"Import encryption key from file.
Choose this option if you have a stored backup file of the encryption key."</string> 
```

为了防止滥用或意外的共享请求，其他用户需要接受所有者的共享邀请。其他用户可以拒绝邀请，或者在接受邀请后放弃访问。

```
 <string name="spot_pending_owner_explanatory_text_async_message">This user has yet to accept or reject your sharing invitation. If something went wrong, e.g. they not received or have lost your message, you can re-issue the invitation using the ⟳ button.</string>
<string name="spot_pending_owner_explanatory_text_qr_code">This user has yet to accept or reject your sharing invitation. If something went wrong, e.g. they have yet to scan the QR code, you can re-issue the invitation using the ⟳ button.</string>
<string name="spot_relinquish_device_dialog_content">"Are you sure you want to relinquish this shared device?
To share this device again, you will need to get a new invitation."</string>
<string name="spot_relinquish_device_dialog_title">Relinquish Shared Device</string> 
```

当您与他人共享对设备的访问权限时，他们可以通过“查找我的设备”应用程序跟踪您手机的位置。如果你的手机在身边，这意味着他们可以看到你的位置。每个共同所有者还可以看到所有其他共同所有者(以及所有者)的电子邮件地址，因此您应该只与您信任的人共享设备。

```
 <string name="spot_share_device_info_note">Note: when the device is with you, you implicitly share your location with its co-owners (the users listed above).</string>
<string name="spot_share_device_info_note_owner_suffix">"Only invite people you trust to share a device.
Each co-owner can see the email addresses of all the others."</string> 
```

如果您选择远程抹掉设备，该设备将从“查找我的设备”网络中移除，并将重置为出厂状态。

```
 <string name="spot_erase_device_dialog_content">"Are you sure you want to erase this device?
This will remove it from Find My Device and the device tracking services it provides.
The device should be in range with your Android, in order to reset the device to its factory state. If the device is not in range, use the \"force delete\" button."</string>
<string name="spot_erase_device_dialog_title">Erase Device</string>
<string name="spot_erase_device_force_delete_button">Force delete</string>
<string name="spot_erase_device_with_shared_owners_dialog_content">"Are you sure you want to erase this device for yourself and the co-owners?
This will remove it from Find My Device and the device tracking services it provides.
The device should be in range with your Android, in order to reset the device to its factory state. If the device is not in range, use the \"force delete\" button."</string> 
```

谷歌尚未证实其 Find My Device 网络的任何细节，但有传言称 [Pixel 6](https://www.xda-developers.com/google-pixel-6/) 系列将支持超宽带(UWB)，我们预计很快就会听到这一消息。