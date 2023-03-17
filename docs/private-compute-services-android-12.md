# 私有计算服务安全更新 Android 12 中的人工智能功能

> 原文：<https://www.xda-developers.com/private-compute-services-android-12/>

在 [Android 12](https://www.xda-developers.com/android-12/) 中引入的[新隐私功能](https://www.xda-developers.com/android-12-privacy-private-compute-core-privacy-dashboard/)之一是私有计算核心，这是操作系统中存储和处理机器学习数据的安全分区。

目前，Android 12 中的 Private Compute Core 保存了三个机器学习功能的数据:实时字幕、正在播放和智能回复。Private Compute Core 内部的功能不能直接访问互联网，但许多机器学习和人工智能功能需要不时地更新新的和改进的模型，这就是 Android 新的私人计算服务将发挥作用的地方。今天，谷歌宣布了一套新的私人计算核心服务，将使存储在沙盒中的人工智能功能能够安全更新。

私有计算服务将在私有计算核心和云之间提供一个保护隐私的桥梁，使通过安全路径提供新的人工智能模型和沙盒机器学习功能的其他更新成为可能。谷歌表示，功能和私人计算服务之间的通信通过一套有目的的开源 API 进行，这些 API 从数据中删除识别信息，并应用隐私技术，如[联合学习](https://www.xda-developers.com/google-federated-learning-hey-google-accuracy/)，联合分析和私人信息检索。

谷歌表示，他们将开放私人计算服务的代码，以便独立的安全研究人员可以对其进行审计。然而，代码何时公开发布还没有时间表。

私有计算核心是一个安全的环境，与操作系统和应用程序的其余部分相隔离。除非用户有意，否则在这个沙箱中存储和处理的数据不会向其他应用程序公开。例如，智能回复建议将一直隐藏在你的键盘和你正在输入的应用程序中，直到你点击它。

除了隐私沙箱，Android 12 还增加了一个隐私仪表盘，显示手机上的应用程序何时访问位置、麦克风和摄像头等敏感权限的时间线。