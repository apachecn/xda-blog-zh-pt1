# 这个应用程序可以让你调整 Android 13 设备上的手电筒亮度

> 原文：<https://www.xda-developers.com/adjust-flashlight-brightness-android-13-devices/>

# 这个应用程序可以让你调整一些 Android 13 设备上的闪光灯亮度

现在，您可以使用手电筒-提拉米苏应用程序来调整 Android 13 设备上的手电筒亮度。从帖子里的链接下载。

在谷歌向用户推出第一个开发者预览版 Android 13 后不久，我们得知它包括了两个新的 API 来帮助用户控制手机上的闪光灯亮度。这一发现让我们相信，Android 13 将推出一种新的开关，帮助用户轻松调节手电筒的亮度。遗憾的是，在本月早些时候[向 Pixel 设备](https://www.xda-developers.com/android-13-launched/)推出的 Android 13 稳定版中没有这种功能。

虽然谷歌没有在 Android 13 中添加原生选项来帮助用户控制手电筒亮度，但你现在可以使用第三方应用程序来实现这一目的。polodarb 的手电筒-提拉米苏是一个方便的应用程序，可以让你控制 Android 13 设备上的手电筒亮度。正如你在附上的截图中看到的，该应用程序有一个准系统界面，只有一个滑块，让你调整手电筒的亮度。

该应用程序可以在运行 Android 13 的 Pixel 6、Pixel 6 Pro 和 Pixel 6a 上正常工作，也可以在运行 One UI 5.0 测试版的 Galaxy S22 Ultra 上使用。在像素上，该应用程序提供了对亮度的精细控制，而在 Galaxy S22 Ultra 上，你只能获得五个亮度级别。手电筒-提拉米苏并不能在所有运行 Android 13 的设备上工作。在我们的测试中，我们发现它在运行 [ColorOS 13 beta](https://www.xda-developers.com/oppo-coloros-13-beta-hands-on/) 的 Oppo Find X5 Pro 上无法工作，而 *9to5Google* 的 Max Weinbach 报告称，它在运行 [OxygenOS 13 beta](https://www.xda-developers.com/oneplus-oxygenos-13-open-beta-hands-on/) 的一加 10 Pro 上也无法工作。

正如*斯珀*的米莎尔·拉赫曼在他们[之前对新 API](https://blog.esper.io/android-13-flashlight-brightness-control/)的报道中指出的，该应用在一些设备上无法工作，因为它需要更新相机硬件抽象层(HAL)。 *"* *【因为】谷歌已经冻结了其新的 HAL 要求，以确保针对版本 N 构建的供应商实现将可认证到版本 N+3...拉赫曼写道:“设备制造商可以将他们的设备升级到 Android 13，同时重用为旧版本 Android 设计的供应商实现，该版本不包括新的相机设备 HAL 及其对 LED 亮度控制的支持。*

这可能是该应用程序在 Oppo Find X5 Pro 和一加 10 Pro 上不工作的原因。如果您拥有任何其他受支持的设备，您可以通过从下面提供的链接下载 APK 来尝试一下。

**[下载手电筒-提拉米苏](https://github.com/polodarb/Flashlight-Tiramisu)**