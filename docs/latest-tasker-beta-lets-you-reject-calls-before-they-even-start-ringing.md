# 最新的 Tasker 测试版可以让你在电话铃响之前就拒绝接听

> 原文：<https://www.xda-developers.com/latest-tasker-beta-lets-you-reject-calls-before-they-even-start-ringing/>

广受欢迎的自动化应用程序 [Tasker](https://www.xda-developers.com/tasker-5-10-rolls-out-stable-android-11-controls-support/) 的开发者若昂·迪亚斯(joo Dias)已经[发布了新的测试版](https://www.reddit.com/r/tasker/comments/jemaxl/dev_tasker_5113beta_call_screening_and_a_bunch_of/)，这使得筛选那些机器人电话(或者你的父母，如果那是你的事情)变得更加容易。Tasker 5.11.3 beta 目前正在推出测试版，它增加了一个功能，可以在你的电话开始响铃之前阻止来电者与你联系。

该功能利用了 [CallScreeningService](https://developer.android.com/reference/kotlin/android/telecom/CallScreeningService) ，这是一种最初在 API level 24 (Android 7.0 Nougat)中提供的 API，但在 API level 29 (Android 10)中进行了更改，不再要求将呼叫筛选应用程序设置为默认拨号器。因此，Tasker 对该功能的实现适用于 Android 10 及以上版本的用户。安装最新的测试版后，用户可以将 Tasker 设置为他们的来电显示&垃圾邮件应用程序，从而能够根据他们在应用程序中设置的配置文件来设置筛选或阻止来电。

joo Dias 分享了新功能的视频演示:

新的来电过滤事件和来电过滤动作是该版本中唯一重要的新功能(但请记住，这只是一个测试版)，因为开发人员主要专注于让 Tasker 为 Google Play 即将于 11 月 2 日发布的 API level 29 要求做好准备。提醒一下，所有提交到 Google Play 的新应用已经被要求以 API 29 级为目标，而从 11 月 2 日开始，现有应用的更新将被要求以 API 29 级为目标。

这个 Tasker beta 版本中的其他调整包括将传感器方向坐标转换为角度的能力，对相机动作的修复，以及许多其他错误的修复。它还为因 API 问题而暂时取消的操作添加了警告。

如前所述，谷歌 Play 商店的稳定版 Tasker 还没有这个功能。如果你正在进行测试程序，但你实在等不及了，这里有一个下载 APK 的直接链接。如果你想加入 Tasker Beta 计划，你可以在[这里](https://joaoapps.com/beta-testing/)加入。别忘了，XDA 有一个[的完整论坛](https://forum.xda-developers.com/u/tasker-tips-tricks)，里面满是如何充分利用这个最强大的应用程序的提示和技巧。

### Tasker 5.11.3.beta 完整变更日志

*   Android 10+新增**来电屏蔽**动作和**来电屏蔽**事件。允许您在来电开始响铃之前拒绝来电。这里演示:【https://youtu.be/JxwfwkeffMk 
*   增加了在**测试传感器**动作和**任何传感器**条件下将方位坐标转换为度数的选项
*   修正了 Android 10+上的**相机**动作
*   修正了当编辑元素视频控制动作时视频值被重置的问题
*   修正了上一个测试版在一些手机相关操作上的问题
*   修复了**任何传感器**事件和状态，当其他电池强度较低的条件为假时，不会停止传感器监控
*   修正了有时当你在 Tasker 中接受一个新设置时**任何传感器事件**都会触发的问题
*   暂时不要使用管理外部存储权限，因为 Google Play 还不支持它，但已经做好了准备
*   如果需要，使 **Wifi 连接**状态中的 SSID 字段为多行
*   修复了向插件发送文字变量名(如\%variable)的问题
*   添加了**移动网络类型**动作在 Android 10+上不再有效的警告。
*   **结束通话**由于 Android 限制，Android 10+上的操作不再像以前一样有效