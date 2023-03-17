# 如何安装带有空间音频的 tvOS 15 开发者测试版

> 原文：<https://www.xda-developers.com/how-to-install-tvos-beta/>

# 如何安装带有空间音频的 tvOS 15 开发者测试版

苹果新的 tvOS 15 更新带有空间音频，苹果还没有真正说还有什么，但你现在可以开始测试测试版。

在苹果的 [WWDC](https://www.xda-developers.com/tag/wwdc-2021/) 主题演讲中，苹果没有谈到的一件事是 tvOS。它确实简要提到了 tvOS 15 将包括空间音频，但仅此而已。当然，这并不罕见。毕竟，你能添加到内容消费平台的东西是有限的。

不过，你现在就可以拿到 tvOS 15 开发者测试版。

## 与 tvOS 15 兼容的 Apple TV 设备列表

*   Apple TV HD(也称为 Apple TV 第四代)
*   苹果电视 4K(两种型号)

## 如何安装 tvOS 15

在苹果电视上安装测试软件的棘手之处在于:它没有网络浏览器。这意味着，如果不将设备连接到 Mac，就无法在设备上获取配置描述文件。注意，如果你在等待公测，你可以通过设置打开测试版。

### 使用配置描述文件

1.  进入[苹果开发者](https://developer.apple.com/) - >开发- >下载，点击 tvOS 15 旁边的“安装配置文件”。
2.  请确定您已经安装了 Xcode 你可以从 Mac App Store 免费获得，也可以从 Apple Developer 获得新的测试版。你还需要苹果配置器。
3.  确定您的 Apple TV 已打开，并且与 Mac 连接在同一个 Wi-Fi 网络上。
4.  在 Xcode 中，进入 Windows ->设备和模拟器->设备。
5.  在 Apple TV 上，进入设置->遥控器和设备->远程应用程序和设备，这将启动 Apple TV 搜索要配对的设备的过程。
6.  回到 Xcode，您会看到一个发现区，您可以在这里选择您的 Apple TV。
7.  您将看到一个验证码，您需要输入该验证码。
8.  打开 Apple Configurator 并按照说明来设置 Apple TV(如果尚未完成)。
9.  单击添加->描述文件，然后添加配置描述文件。
10.  像往常一样检查 Apple TV 上的更新。

### 使用恢复映像

就像 iOS 15 一样，你可以将图像闪存到你的 Apple TV 中。奇怪的是，苹果只在苹果电视(第四代)上提供这种功能。这可能是因为 Apple TV 4K 实际上没有 USB 端口。

1.  前往[Apple Developer](https://developer.apple.com/)->Develop->Downloads，下载 Apple TV HD 的恢复映像。
2.  使用 USB Type-C 电缆将 Apple TV 连接到 Mac。
3.  在 Finder 中，选择您的 Apple TV。
4.  按住 Option 键，点按“恢复 Apple TV”。与 iOS 不同，没有检查更新的选项，所以这将进行工厂重置。
5.  导航到您下载的图像并打开它。

公开测试版也是可用的，所以每个人都更容易得到它们。这也是在向公众发布之前测试候选版本的一种简单方法。