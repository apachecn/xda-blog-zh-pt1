# 你现在可以直接从谷歌助手运行 Tasker 任务

> 原文：<https://www.xda-developers.com/run-tasker-tasks-from-google-assistant/>

对于我们的许多读者来说，Tasker 不需要介绍。这是 Android 上最好的自动化应用，自从最初的开发者[在近 3 年前把火炬传给 joo Dias](https://www.xda-developers.com/tasker-joao-dias-autoapps-development/)(!)，不断变得更好。随着版本 5.11.14 的更新，Tasker 任务现在可以直接从 Google Assistant 调用。

正如开发人员在 Reddit 上解释的那样，你可以说“好的，谷歌，在 Tasker 中运行我的任务”，其中“我的任务”与你的任何任务的名称相匹配。或者，如果你喜欢这些，你可以把“运行”换成“开始”、“执行”、“设置”或“发送”，开发人员正在考虑把“转动”加到组合中，这样你就可以说“打开我的电脑”或“关掉我的灯”之类的话了。你甚至可以通过语音运行一个任务，并同时设置几个变量，比如说“好的，谷歌，用一些东西和其他东西运行我的任务”，这将变量%par1 设置为“一些东西”，将%par2 设置为“其他”。然后，可以设置您的任务来解析%par1 和%par2 变量，做您想做的任何事情。

如果您想要更多的控制，您也可以使用新的“助理行动”事件创建一个配置文件。这将允许您接收可变输入。例如，您可以要求 Google Assistant“使用 Tasker 运行 5 分钟后关闭我的卧室灯”来触发 Assistant 操作配置文件，然后使用 [Tasker 的模式匹配](https://tasker.joaoapps.com/userguide/en/matching.html)解析查询的“等待 5 分钟”和“关闭我的卧室灯”部分，以正确的顺序执行您想要的操作。

下面嵌入的视频展示了 Tasker 新的谷歌助手集成可以做的几件事。开发者展示的许多东西都需要一两个额外的插件，但不是所有的都需要。这款应用总是有一点学习曲线，但回报可能会很大。在我看来，玩几十个不同的动作和插件也很有趣，但每个都有自己的风格。

虽然 Tasker 的新谷歌助手集成非常强大，但它目前只支持英语。不过，这显然是谷歌打造的[助手应用动作](https://developers.google.com/assistant/app/overview)功能的一个局限。Tasker dev 表示，一旦谷歌允许，他将增加对其他语言的支持。

如果你对用 Tasker 自动化你的生活感兴趣，那就从 Google Play 下载这个应用吧。它的价格为 3.49 美元，但订阅 Google Play Pass 是免费的。如果你从开发者网站下载 APK [，你可以免费试用该应用 7 天，但我们认为考虑到它提供的多少，它绝对值得购买。](https://tasker.joaoapps.com/)

### Tasker 5.11.14 完整变更日志

*   移除了“助理行动”事件不工作的警告，因为它现在工作了
*   添加了助手动作视频提示
*   修正了在某些情况下在某些设备上使用应用工厂构建应用的问题
*   固定链接到俄语翻译论坛
*   让 javascript 中的“alert()”函数返回哪个按钮被按下
*   使“蓝牙连接”事件能够在设置时选择蓝牙设备
*   在“Tasker 函数”操作中添加了“GenerateUUID()”函数
*   通过在“HTTP Auth”操作中直接指定自定义重定向 URL，使用户可以使用自定义重定向 URL
*   修正了有时通知显示 Tasker 没有被授权的问题
*   修正了 Tasker 在某些情况下的许可检查
*   如果确实需要，只在“测试网络”操作中使用位置权限
*   允许“执行任务”操作的参数输入字段有多行输入
*   修正了当复制文件到外部 SD 卡大写扩展名时，在目标文件中可能使用错误扩展名的错误
*   修复了在某些情况下使用 Javascript 中的项目/概要文件/任务变量
*   不允许在“可变状态”状态下使用不受监控的内置变量。错误地允许了它
*   修复在某些情况下插件中使用无效变量名的问题
*   修复某些设备上的“采取的步骤”事件
*   修正了小的崩溃