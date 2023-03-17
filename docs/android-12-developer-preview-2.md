# Android 12 开发者预览版 2 带来了更好的通知安全性和画中画增强功能

> 原文：<https://www.xda-developers.com/android-12-developer-preview-2/>

随着每一天的过去，我们离下一个主要 Android 操作系统的最终发布越来越近: [Android 12](https://www.xda-developers.com/android-12/) 。如果你渴望看到即将到来的 Android 版本的未来，谷歌已经为你准备好了今天的内容。该公司刚刚宣布了一个适用于合格像素设备的新开发者预览版。Android 12 开发者预览版 2，像[第一个开发者预览版](https://www.xda-developers.com/android-12-developer-preview-1/)一样，仍然只面向开发者，博文中提到的变化列表专注于开发者将不得不适应的新 API 和平台行为变化。以下是发生的变化。

## Android 12 开发者预览版 2 的新功能

### 信任和安全

*   允许一个应用程序在其他应用程序上覆盖窗口会带来明显的安全风险。为此，开发者预览版 2 中引入的新的 [HIDE_OVERLAY_WINDOWS](https://developer.android.com/reference/android/Manifest.permission#HIDE_OVERLAY_WINDOWS) 权限确保了应用程序可以调用[Window # sethideoverlywindows()](https://developer.android.com/reference/android/view/Window#setHideOverlayWindows(boolean))来指示当应用程序的窗口可见时，所有 [TYPE_APPLICATION_OVERLAY](https://developer.android.com/reference/android/view/WindowManager.LayoutParams#TYPE_APPLICATION_OVERLAY) 窗口应该隐藏。
*   在此新的预览版中，通知可见性控件已得到更新。现在，您可以配置通知操作，以便当从锁屏触发时，它们将始终生成验证质询。例如，一个消息应用程序现在要求在删除消息或将其标记为已读之前进行身份验证。
*   Android 12 开发者预览版 2 增加了对一种更简单、更有效的方式来获取已安装应用的校验和的支持。开发人员可以从 SHA256、SHA512、Merkle Root 等几种标准摘要算法中进行选择。这个特性的向后兼容版本正在开发中，在不久的将来会以 Jetpack 库的形式出现。

### Android 12 API 的新变化

*   **圆角:**在 Android 12 开发者预览版 2 中，开发者可以检查设备是否有带[圆角](https://developer.android.com/reference/android/view/RoundedCorner?hl=en)的屏幕，并获得他们的详细信息。从 UI 设计的角度来看，人们现在可以利用每个圆角的绝对细节以及相对于应用程序边界的角细节。
*   **画中画(PIP)改进:**应用程序现在可以[启用无缝调整大小](https://developer.android.com/reference/android/app/PictureInPictureParams.Builder#setSeamlessResizeEnabled(boolean))让系统在需要时调整 PIP 活动的大小。此外，启用 auto-PIP 现在可以使系统直接将应用程序转换到 PIP 模式，而无需等待 up-to-home 动画完成。最后，Android 现在支持[通过将画中画窗口](https://www.xda-developers.com/android-12-brings-pinch-to-resize-and-stashing-for-picture-in-picture-windows/)拖动到屏幕的左边缘或右边缘来隐藏它。
*   **配套设备应用程序 API 的更新:**智能手表和健身追踪器等可穿戴设备通常需要专门的应用程序来管理它们。谷歌希望只要有相关的配套设备在附近，这类应用程序就能更容易地运行和连接。为此，Android 12 开发者预览版 2 引入了一个新的[公司设备服务](https://developer.android.com/reference/android/companion/CompanionDeviceService) API。此外，新的[配套设备配置文件](https://developer.android.com/reference/android/companion/AssociationRequest.Builder#setDeviceProfile(java.lang.String))大大简化了配套设备注册流程。
*   **带宽估算改进:** Google 对现有的带宽估算 API 进行了大幅增强。开发人员现在可以获得设备上所有用户的每个运营商或 Wi-Fi SSID、网络类型和信号水平的总吞吐量估计值。
*   视觉效果:在 Android 12 中，使用 [RenderEffect](https://developer.android.com/reference/android/graphics/RenderEffect) 类来应用普通的图形效果比以往更加容易。现在，您可以单独应用模糊和颜色过滤器，或者将这些效果作为一个整体组合成连锁效果。

你可以[去这里](https://developer.android.com/sdk/api_diff/s-dp2/changes)看看 Android 12 DP1 和 DP2 之间的完整 API 差异。由于谷歌已经修改了几个 API，请确保通过[行为改变开关](https://developer.android.com/about/versions/12/reference/compat-framework-changes)来运行和调试你的应用程序，为面向 Android 12 做准备。反馈可以在这里[给出。](https://developer.android.com/about/versions/12/feedback)

建议在下载和刷新更新之前阅读[发行说明](https://developer.android.com/preview/release-notes)。请务必[到这里](https://issuetracker.google.com/issues/new?component=190602&template=1407746)提交任何错误报告，[到这里](https://www.reddit.com/r/android_beta/)讨论最新版本。

## 下载 Android 12 开发者预览版 2

要在 Pixel 设备上安装 Android 12 开发者预览版 2，您必须拥有 Pixel 3、Pixel 3 XL、Pixel 3a、Pixel 3a XL、Pixel 4、Pixel 4 XL、Pixel 4a、Pixel 4a 5G 或 Pixel 5。我们在这个页面上有链接可以下载这些谷歌 Pixel 设备[的最新系统映像。你可以选择增量 OTA 更新或者](https://www.xda-developers.com/how-to-download-android-12/)[手动刷新版本](https://www.xda-developers.com/how-to-install-android-12)。如果您没有兼容的设备，可以在 Android Studio 的 Android 模拟器中运行构建。

第二个 Android 12 开发者预览版也适用于 [Android TV](https://www.xda-developers.com/android-12-preview-android-tv-google-tv-experience/) ，其中 [ADT-3 开发者套件](https://store.askey.com/adt-3.html)是唯一兼容的设备。

* * *

四月份应该会有一个更大的开发者预览版，然后是几个测试版。如果一切按计划进行，稳定的 Android 12 版本将于 2021 年第三季度推出。

对于所有最新的 Android 12 新闻，请标记以下标签:

**[安卓 12 XDA 新闻](https://www.xda-developers.com/tag/android-12/)**