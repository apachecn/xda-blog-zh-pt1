# Android 12 可能会让设置 Google Home 设备变得更加无缝

> 原文：<https://www.xda-developers.com/android-12-concurrent-peer-to-peer-internet-connection/>

[Android 12](https://www.xda-developers.com/android-12/) 是一次大规模更新。它不仅给[带来了彻底的设计革新](https://www.xda-developers.com/material-you/)，还包含了大量的新功能和改进，将极大地改善我们与 Android 设备的交互方式。除了这些突出的功能，Android 12 还带来了许多较小的生活质量变化。

Andriod 12 带来的一个小而有用的改进是能够同时保持与对等设备和 Wi-Fi 路由器的 Wi-Fi 连接。如果你曾经试图用你的手机设置 Chromecast 或 Google Home 设备，你可能已经注意到，在设置过程中，你的手机需要首先断开与互联网的连接——提供 Wi-Fi 网络。然后，您的设备启动与物联网设备的对等 Wi-Fi 连接，并在完成设置后，重新连接到提供互联网的 Wi-Fi 网络。

例如，这里有一些截图展示了谷歌 Home 应用程序中谷歌 Nest Mini 的设置过程。正如你所看到的，Nest Mini 创建了一个“临时 Wi-Fi 网络”，手机在设置期间可以连接到这个网络。在此期间，主 Wi-Fi 网络断开，这意味着您的手机与互联网断开连接，除非您打开了移动数据。

发生这种情况的原因是 Android 目前不支持同时连接到对等设备和主要的互联网提供网络(您的 Wi-Fi)。但随着 Android 12 的推出，这种情况将会改变。

从 Android 12 开始，支持并发点对点和互联网连接的设备可以同时保持这两种连接。换句话说，在设置智能家居设备时，你的手机不应该与你的家庭 Wi-Fi 断开连接。但是有一个问题。只有针对 API 级别 31 及更高的应用程序才会启用此功能。针对早期版本 Android 的应用程序将无法利用并发连接，并将受到传统行为的影响，这意味着在连接到对等设备之前，您的设备将与 Wi-Fi 网络断开连接。

这对于 Google Home 和 Chromecast 设备来说不是问题，因为 Google Home 应用程序很可能会在 Android 12 公开发布后不久或之前进行更新，以利用这一功能。然而，如果你正在使用亚马逊或其他原始设备制造商的物联网产品，你可能需要等待他们更新他们的应用程序以支持 Android 12。

对于开发者来说，谷歌建议从[wifi manager . getconnectioninfo()](https://developer.android.com/reference/android/net/wifi/WifiManager#getConnectionInfo())API 迁移出来，转而使用[network callback . oncapabilities changed()](https://developer.android.com/reference/android/net/ConnectivityManager.NetworkCallback#onCapabilitiesChanged(android.net.Network,%20android.net.NetworkCapabilities))API。前者在 Android 12 中已被否决，该 API 将不支持屏蔽位置敏感数据等新功能。