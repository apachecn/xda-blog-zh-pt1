# Android 12 不再需要你的位置来扫描附近的蓝牙设备

> 原文：<https://www.xda-developers.com/android-12-location-scan-nearby-bluetooth-devices/>

谷歌在每个 Android 版本中不断改善隐私并规范应用程序使用权限的方式，Android 12 也带来了健康的变化。昨天，在主要的 [Google I/O 2021](https://www.xda-developers.com/google-io-2021-recap/) 主题演讲中，展示了隐私仪表盘、通知栏中的摄像头/麦克风使用图标等功能。但也有一些较小的变化，以确保应用程序只使用他们需要的权限，无论何时他们需要使用它们，而不是访问他们不需要的任何东西。其中一个变化非常小，但却是重要的一步:现在，应用程序不再需要请求位置许可来跟踪附近的蓝牙设备。

这可能是一个奇怪的问题，你可能会问自己:为什么扫描附近的蓝牙设备需要位置权限？基本上，在 Android 12 之前，扫描附近蓝牙或 Wi-Fi 设备的能力是与 Android 更广泛的“位置”权限捆绑在一起的。这种情况的原因是有道理的:你可以通过推断附近或当前连接的蓝牙设备或 Wi-Fi 网络来跟踪设备。因此，即使一个应用程序只是扫描蓝牙设备，而没有利用 GPS 或其他跟踪技术，它仍然需要相同的位置权限。

然而，由于用户的误解，这导致了不可预见的后果。当基于蓝牙的新冠肺炎联系人追踪应用程序被开发出来时，这些位置权限提示导致许多用户指责这些应用程序跟踪你的位置，这就是为什么谷歌[在 Android 11 中为这些应用程序破例](https://www.xda-developers.com/android-11-beta-3-here-remove-location-requirement-covid-19-contact-tracing-apps-exposure-notification-system/)，这样他们就不再需要请求位置权限才能使用联系人追踪 API。

现在在 Android 12 中，[谷歌增加了](https://developer.android.com/about/versions/12/features/bluetooth-permissions)一个新的蓝牙 _ 扫描和蓝牙 _ 连接权限，这是与应用程序可以请求的位置权限不同的专用权限。获得这些权限后，应用程序可以扫描附近的设备，而无需请求位置权限。然而，只有针对 Android 12 的应用程序才能声明这些权限。

这很重要，因为不仅用户在授予应用程序权限时更有信心，而且还避免了这些应用程序获得定位你的手机的权限——如果位置权限被授予，他们就可以这样做。