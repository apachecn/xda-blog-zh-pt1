# Mobvoi 正在开发智能录音机和人工智能转录服务

> 原文：<https://www.xda-developers.com/mobvoi-working-smart-audio-recorder-ai-transcription-service/>

可穿戴设备制造商 Mobvoi 在今年推出了一系列智能手表和 [TWS 耳塞](https://www.xda-developers.com/ticpods-anc-review/)后，现在正在开发一款新的录音机产品。这款名为 Mobvoi AI Recorder 的设备最近在 FCC 的一份文件中被发现，这让我们很好地了解了它的设计和尺寸。

有问题的 [FCC 文件](https://gov.fccid.io/2AX5U-CXR-TNT)是由深圳天诺科技有限公司提交的，很可能是该设备的 ODM。根据提交的文件，Mobvoi AI 记录仪将有一个带圆形边缘的高矩形机身。这台录音机的左边有两个按钮，背面有一个皮带夹。它只有 11 毫米厚，60 毫米高，19 毫米宽。

虽然 FCC 的文件没有透露关于该设备的更多信息，但我们通过解码 Google Play 上最新版本的 [Mobvoi 应用程序，设法挖掘出了一些额外的细节。拆卸后显示了一个教程页面，解释了设备上各种按钮的作用及其工作原理。我们还设法从 APK 提取了一些高质量的设备渲染图。](https://play.google.com/store/apps/details?id=com.mobvoi.companion.aw)

### 在 Mobvoi 应用程序中发现新字符串

```
 <string name="ticrecorder">Mobvoi AI Recorder</string>
<string name="triton_battery_unknown">request…</string>
<string name="triton_blue_light_long_press">Long press Bluetooth until green indicator flickers</string>
<string name="triton_bluetooth_connect">Bluetooth connection</string>
<string name="triton_bluetooth_pair_text">Bluetooth pairing</string>
<string name="triton_confirm_to_finish">Press the boot button again to complete the pairing</string>
<string name="triton_connected">Connected</string>
<string name="triton_data_sync">Data transporting…</string>
<string name="triton_delete">Delete</string>
<string name="triton_deleting_file">File deleting…</string>
<string name="triton_device_number">Device number：%s</string>
<string name="triton_device_sync">Sync</string>
<string name="triton_device_title">Triton 会议盒子</string>
<string name="triton_disconnected">Disconnected</string>
<string name="triton_edit_hint">输入搜索词搜索相关内容</string>
<string name="triton_fail_upload_to_server">Upload fail.</string>
<string name="triton_file_already_synced">File already synchronized</string>
<string name="triton_file_delete">Delete</string>
<string name="triton_file_issync">synchronized</string>
<string name="triton_file_sync">Upload to the cloud</string>
<string name="triton_file_syncing">Synchronizing…</string>
<string name="triton_file_upload">Transfer to the phone</string>
<string name="triton_file_uploading">Uploading…</string>
<string name="triton_find">Search again</string>
<string name="triton_find_device">Discovery equipment</string>
<string name="triton_find_my_device">Find my device</string>
<string name="triton_finish_wifi_transport">Synchronizing succeeded</string>
<string name="triton_how_to_des">"1\. Click the Bluetooth button on the device, and the Bluetooth light is green, indicating that the Bluetooth connection is on.
2.If the device has been connected to the phone Bluetooth before, the device will automatically detect that the Bluetooth is on and make the connection automatically"</string>
<string name="triton_how_to_open">How to turn on/off</string>
<string name="triton_how_to_wifi">"1\. After the device Bluetooth is connected to the mobile phone, click the WiFi button, and the WiFi light is blue, indicating that the WiFi express has been turned on.
2.APP automatically detects WiFi, and automatically connects After
3.APP connects to the device, click below to enter the recording pen folder for data synchronization."</string>
<string name="triton_i_known">I known</string>
<string name="triton_make_sure_bluetooth_on">"Please make sure your device is powered on and your phone's Bluetooth is turned on."</string>
<string name="triton_memory_manager">Space management</string>
<string name="triton_more">more</string>
<string name="triton_my_device">My Device</string>
<string name="triton_no_server_file">No files</string>
<string name="triton_no_unsynced_file">No files</string>
<string name="triton_not_device">No available equipment found.</string>
<string name="triton_not_transfer">Unsynchronized recording</string>
<string name="triton_operation_guide">Operating instructions</string>
<string name="triton_pair_fail">Bind failed.</string>
<string name="triton_pair_success">Bind succeeded.</string>
<string name="triton_record_duration">%1$dm%2$ds</string>
<string name="triton_record_duration_with_hour">%1$dh%2$dm%3$dm</string>
<string name="triton_record_file_name">The recording on %3$s,%1$d/%2$d</string>
<string name="triton_record_list">Record List</string>
<string name="triton_record_list_synced">Synchronized recording list in the cloud</string>
<string name="triton_remain_duration">It is expected that it can also be transcribed: %1$s</string>
<string name="triton_remain_memory">Remaining: %1$s</string>
<string name="triton_serial_number">SN: %1$s</string>
<string name="triton_source_cloud">in cloud</string>
<string name="triton_source_device">in the device</string>
<string name="triton_storage_management">Space management</string>
<string name="triton_success_delete_file">Delete file succeeded.</string>
<string name="triton_success_upload_to_server">Upload succeeded.</string>
<string name="triton_sync_by_wifi">Audio data volume is large, WiFi transmission is recommended</string>
<string name="triton_transport_left_time">Please be patient and wait approximately %1$d minutes %2$d seconds.</string>
<string name="triton_tutorial_page1_1">Record key</string>
<string name="triton_tutorial_page1_2">On/WiFi fast transfer key</string>
<string name="triton_tutorial_page1_3">Microphone</string>
<string name="triton_tutorial_page1_title">Equipment composition description</string>
<string name="triton_tutorial_page2_1">Magnetic back clip</string>
<string name="triton_tutorial_page2_2">USB - C</string>
<string name="triton_tutorial_page2_3">USB Type - C data line</string>
<string name="triton_tutorial_page2_title">Equipment composition description</string>
<string name="triton_tutorial_page3_1">Long press Bluetooth until green indicator flickers</string>
<string name="triton_tutorial_page3_2">1\. Power on, start button is on in green, APP will detect device Bluetooth automatically for connection.</string>
<string name="triton_tutorial_page3_3">2\. If device has been connected to mobile phone Bluetooth, the device will have automatic connection when detect that Bluetooth is enabled.</string>
<string name="triton_tutorial_page3_title">Bluetooth pairing and APP connection</string>
<string name="triton_tutorial_page4_1">1\. Power on, click “Record” and it will shake; recording is started when red indicator flickers.</string>
<string name="triton_tutorial_page4_2">2\. Click “Record” key again to shake, red indicator is off and recording is stopped.</string>
<string name="triton_tutorial_page4_title">Start/stop recording</string>
<string name="triton_tutorial_page5_1">Turn on WiFi fast transfer to speed up transfer of record into mobile phone APP</string>
<string name="triton_tutorial_page5_2">1\. When Bluetooth is connected to mobile phone, click WiFi button again, WiFi blue indicator is on, which means WiFi fast transfer is enabled</string>
<string name="triton_tutorial_page5_3">2\. The APP will detect WiFi automatically for automatic connection</string>
<string name="triton_tutorial_page5_4">3\. When APP is connected, enter the device’s folder for data synchronization</string>
<string name="triton_tutorial_page5_title">WiFi fast transfer</string>
<string name="triton_tutorial_page6_1">Record Button</string>
<string name="triton_tutorial_page6_10">BLUE is on</string>
<string name="triton_tutorial_page6_10_1">Wifi enabled</string>
<string name="triton_tutorial_page6_11">BLUE flashing</string>
<string name="triton_tutorial_page6_11_1">Waiting for connection</string>
<string name="triton_tutorial_page6_12">BLUE always on</string>
<string name="triton_tutorial_page6_12_1">Wifi connected</string>
<string name="triton_tutorial_page6_13">YELLOW flashing</string>
<string name="triton_tutorial_page6_13_1">OTA upgrade</string>
<string name="triton_tutorial_page6_14">RED always on</string>
<string name="triton_tutorial_page6_14_1">Charging</string>
<string name="triton_tutorial_page6_15">BLUE always on</string>
<string name="triton_tutorial_page6_15_1">Fully charged</string>
<string name="triton_tutorial_page6_2">RED flashing</string>
<string name="triton_tutorial_page6_2_1">Recording</string>
<string name="triton_tutorial_page6_3">RED off</string>
<string name="triton_tutorial_page6_3_1">End of recording</string>
<string name="triton_tutorial_page6_4">WiFi Button</string>
<string name="triton_tutorial_page6_5">Green is on</string>
<string name="triton_tutorial_page6_5_1">Power on</string>
<string name="triton_tutorial_page6_6">Green flashing</string>
<string name="triton_tutorial_page6_6_1">Waiting for connection</string>
<string name="triton_tutorial_page6_7">Green always on</string>
<string name="triton_tutorial_page6_7_1">Bluetooth connected</string>
<string name="triton_tutorial_page6_8">RED is off</string>
<string name="triton_tutorial_page6_8_1">Power off</string>
<string name="triton_tutorial_page6_9">RED flashing</string>
<string name="triton_tutorial_page6_9_1">Insufficient power supply</string>
<string name="triton_tutorial_page6_title">Indicator light</string>
<string name="triton_tutorial_page7_1">rec.mobvoi.com</string>
<string name="triton_tutorial_page7_2">You can log on to the recording platform of Mobvoi and then edit and rewrite the recording files online.</string>
<string name="triton_tutorial_page7_title">Log in to WEB for online editing</string>
<string name="triton_tv_update_content">Updates</string>
<string name="triton_unbind_device">Unbind Device</string>
<string name="triton_unbind_fail">Unbinding failed.</string>
<string name="triton_update">Firmware upgrade</string>
<string name="triton_usb">USB data transport</string>
<string name="triton_version">Firmware version</string>
<string name="triton_week_fri">Fri</string>
<string name="triton_week_mon">Mon</string>
<string name="triton_week_sat">Sat</string>
<string name="triton_week_sun">Sun</string>
<string name="triton_week_thu">Thu</string>
<string name="triton_week_tue">Tue</string>
<string name="triton_week_wed">Wed</string>
<string name="triton_wifi">WiFi 配网</string>
<string name="triton_wifi_connect">WiFi connection being initiated</string>
<string name="triton_wifi_connect_fail">Wifi connect fail.</string>
<string name="triton_wifi_disconnected">Wifi disconnected</string>
<string name="triton_wifi_fast">WiFi Fast Forward</string>
<string name="triton_wifi_file_sync">File synchronize</string>
<string name="triton_wifi_transport">Wifi Synchronize</string> 
```

正如你在所附图片中看到的那样，Mobvoi AI 记录仪将在正面配备两个麦克风，在左侧边缘有一个录音按钮和电源开关/WiFi 快速传输键。正如在 FCC 文件中看到的那样，该录像机背面将有一个磁性皮带夹，底部边缘还将有一个 USB Type-C 端口。

该教程进一步透露，用户将能够通过按下电源按钮将 Mobvoi AI 记录器与智能手机配对，当设备处于配对模式时，电源按钮将显示绿色 LED。初始配对过程完成后，该设备将在每次开机时自动连接到智能手机。

要录制音频，用户必须按下录制按钮，Mobvoi AI 录音机将振动，以表明它已经开始录制。在录制过程中，录制按钮还会显示一个红色 LED 指示灯。当连接到智能手机时，用户可以通过按下电源/WiFi 快速传输按钮，将他们的录音快速传输到连接的设备。指示灯 LED 会变成蓝色，表示 WiFi 快速传输已启用。

当 WiFi 快速传输打开时，Mobvoi 应用程序会自动检测，并在智能手机上打开设备的根文件夹进行数据同步。本教程还包括一个方便的图表，突出所有的 LED 指示灯颜色及其含义。现在我们已经看了教程，这里有几个设备的高分辨率渲染:

尽管 Mobvoi 迄今为止尚未正式发布任何关于 Mobvoi AI 录音机的信息，但该公司已经[建立了一个新网站](https://rec.mobvoi.com/welcome)，介绍一种旨在帮助用户管理和转录他们的录音的人工智能转录服务。正如你在所附的截图中看到的那样，该网站强调了 Mobvoi AI 的转录功能，这将允许用户轻松地将他们的语音记录转换为文本文件。

人工智能还将标记关键音频，以帮助用户通过点击按钮跳回到他们记录的重要部分。此外，它将提供一个智能摘要，将所有重要内容分段显示。每个部分都有自己相应的关键字，使用户能够快速定位和跟踪以前会议的内容。

该公司的编辑套件还允许用户为他们的录音添加标签，以便于访问，即时编辑转录，并在各种平台上查看所有录音。最后，为了确保所有用户数据保持隐私，Mobvoi 将使用多种加密算法对上传到其服务的所有数据进行加密。

截至目前，我们还没有关于 Mobvoi AI 记录器的发布日期和定价的信息。我们联系了 Mobvoi，以获得关于即将推出的产品的更多细节，但该公司拒绝对我们的调查结果发表评论。