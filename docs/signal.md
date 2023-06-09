# 什么是 Signal 以及如何使用它:关于安全 IM 服务你需要知道的一切

> 原文：<https://www.xda-developers.com/signal/>

在企业和政府的大规模监控变得越来越普遍的时候，消费者正在寻找能够让他们的私人谈话免受窥探的消息应用。虽然有大量的[消息应用](https://www.xda-developers.com/best-chat-apps/)可供消费者使用，但并不是所有的应用都有相同的保护级别或消费者利益。这就是信号发挥作用的地方。

## 什么是信号？

Signal 是一款跨平台的消息应用，专注于隐私和安全。它是免费使用的，由非营利性信号技术基金会运营。此外，它是端到端加密的，所以你所有的聊天和电话都无法访问，除了你和预定的收件人。

由于其隐私保护，Signal 近年来变得更加突出，特别是在美国黑人的命也是命抗议和 WhatsApp 隐私政策混乱之后。它也得到了埃隆·马斯克(Elon Musk)等人的支持。根据一些估计，截至 2021 年 1 月，该应用程序拥有 4000 万月活跃用户。

* * *

## 如何下载和安装信号

Signal 适用于 Android、iPhone/ iPad、Windows、Mac 和 Linux 用户。安装非常简单——安卓用户可以从 [Google Play](https://play.google.com/store/apps/details?id=org.thoughtcrime.securesms) 下载消息应用，而 iPhone 和 iPad 用户可以通过[苹果应用商店](https://apps.apple.com/us/app/signal-private-messenger/id874139669)下载。Google Play 和 App Store 会自动处理安装过程。值得注意的是，Signal 只能在运行 Android 4.4 或更高版本的手机、运行 iOS 11.1 或更高版本的 iPhones 以及运行 iOS 11.1/ iPadOS 13 或更高版本的 iPads 上使用。

对于其他平台，如 Windows、Mac 和 Linux，你必须去其网站下载 Signal。如果您使用的是 Windows，运行下载的可执行文件(。exe)文件，然后按照屏幕上的说明进行操作。macOS 用户必须对下载的磁盘镜像文件进行同样的操作。dmg)。Signal 支持 64 位版本的 Windows 7 或更新版本，以及 macOS 10.11 或更新版本。

对于 Linux 用户来说，这个过程略有不同，这个应用程序只能安装在基于 64 位 Debian 的 Linux 发行版上，比如 Ubuntu、Linux Mint 和 Kali Linux。要在 Linux 上安装 Signal，请在终端中运行以下三个命令。

```
 wget -O- https:
cat signal-desktop-keyring.gpg | sudo tee -a /usr/share/keyrings/signal-desktop-keyring.gpg > /dev/null

echo 'deb [arch=amd64 signed-by=/usr/share/keyrings/signal-desktop-keyring.gpg] https://updates.signal.org/desktop/apt xenial main' |\
  sudo tee -a /etc/apt/sources.list.d/signal-xenial.list

sudo apt update && sudo apt install signal-desktop 
```

### 如何在 Android 手机或 iPhone 上设置信号

*   在 Android 或 iPhone 上安装 Signal 后，打开应用程序。你将被要求给出信号许可来访问联系人和电话。iPhone 的 Signal 也会请求允许发送通知。
*   在您给出必要的权限后，Signal 会询问您的手机号码。此手机号码是注册该服务所必需的。
*   然后，Signal 会向您的手机号码发送一个六位数的代码。您必须输入此代码才能继续。
*   代码之后，应用程序会要求您通过添加您的姓名和上传个人资料图片来设置您的信号个人资料。您可以选择跳过个人资料照片和姓氏，但名字是必需的。
*   然后 Signal 会要求您创建一个 PIN。此 PIN 用于加密您的个人资料信息和对话。您不会被要求输入此 PIN 码来登录应用程序，但如果您重新安装应用程序，则需要输入此 PIN 码来恢复您的帐户。PIN 可以是数字或字母数字，但长度至少为 4 位数。然后，您必须重新输入 PIN 进行确认。
*   完成 PIN 码生成后，您就可以使用该应用程序了。

### 如何在 iPad 上设置信号

有两种方法可以在 iPad 上设置信号。您可以选择将 iPad 应用程序链接到您现有的 Signal 帐户，也可以将 iPad 设置为单独的设备。

*   要将 Signal 的 iPad 版本链接到您现有的帐户，请在您的 iPad 上打开该应用程序，然后选择继续。
*   然后会要求您提供必要的权限。点击“允许”以获得这些权限。
*   获得许可后，它会询问您是要从另一台 iPad 转移现有帐户，还是要将 iPad 添加为新设备。由于这是您第一次在 iPad 上安装应用程序，请选取“添加为新设备”。然后你会被要求打开手机上的应用程序。在尝试将手机连接到 iPad 之前，请确定手机上的信号设置已完成。
*   打开手机上的应用程序，导航至其设置下的链接设备。
*   轻按 Android 上的加号(+)图标或在 iOS 上链接新设备。您可能会被要求向应用程序授予相机权限。
*   在 iPad 应用程序上点击下一步，然后用手机扫描二维码。
*   为链接的 iPad 选择一个名称，然后选择完成。你现在可以在你的 iPad 上使用这个应用了。

如果你计划将 iPad 设置为一个单独的 Signal 设备，请打开应用程序并点击右上角的 unlink 图标。现在你可以按照“如何在 Android 手机或 iPhone 上设置信号”一节中给出的说明来完成设置。

### 如何在桌面上设置信号

Signal for desktop 只能用作链接版本。因此，请确保您已经在 Android 或 iPhone 上设置了该应用程序，然后尝试在桌面上设置它。之后，在桌面上设置 Signal——Windows、macOS 和 Linux——就相当容易了。

只要打开它，你就会被要求使用手机上的应用程序扫描二维码。打开手机上的信号，并导航到其设置下的链接设备。然后在 Android 上点击加号(+)图标，或者在 iOS 上链接新设备。现在，您可以扫描二维码并为链接的设备命名。就这样，你完了。您现在可以在 Windows、Mac 或 Linux 机器上开始使用 Signal 了。

### Signal 上有多设备支持吗，安卓平板呢？

Signal 提供多设备支持，但受到限制。你可以在安卓手机、iPhone 或 iPad 上安装 Signal。之后，您可以将其链接到桌面设备。这样，你可以在多个设备上接收信号，但不能在多个移动设备上使用同一个信号帐户。另外，Signal 并不正式支持 Android 平板电脑。

* * *

## 如何使用信号

既然你已经在任何平台上运行了 Signal，它的工作方式类似于其他聊天应用程序，如 WhatsApp 或 Telegram。若要发送新的个人消息，请点击铅笔图标。根据您的平台，铅笔图标可能出现在右下角或右上角。点击铅笔图标将会弹出你所有已经在 Signal 上的联系人。您也可以使用铅笔图标开始新的群组对话或邀请联系人发信号。只需点击列表中的联系人，聊天窗口就会打开。然后，您可以开始交换消息。

在聊天窗口的顶部，您还会看到视频和语音通话图标，可分别用于发起视频或语音通话。此外，您可以在聊天框中点击某个联系人的姓名，以获取该联系人的特定设置。在这里，你可以选择打开消失消息，更改[聊天壁纸](https://www.xda-developers.com/signal-custom-wallpapers-animated-stickers/)以及修改声音和通知设置。

Signal 还支持最多八人的[群组视频和语音通话](https://www.xda-developers.com/signal-adds-encrypted-group-calls/)。您可以点击群组聊天框顶部的视频通话图标来发起群组通话。在“开始通话”屏幕上，轻触摄像头图标关闭群组语音通话，否则继续群组视频通话。

除了这些基本的消息功能，Signal 还包含许多其他有用的功能，特别是在隐私方面，你可能在其他消息应用程序上找不到，如匿名键盘、代理支持、屏幕安全和安全号码。

* * *

## 信号对话有多安全？

如前所述，Signal 是一个端到端的加密消息应用程序，这意味着您的所有对话都是安全的。您的信号对话只能被目标接收者读取或听到。这不是一个可选的功能-您所有的信息，图像，通话，文件和其他内容总是加密。

Signal Private Messenger 使用自己的开源信号协议进行这种端到端加密。该协议以其“完美的前向保密”实现而闻名，这使得用它加密的消息非常安全。与大多数创建永久密钥对来加密和解密特定设备上的消息的加密系统不同，Signal Protocol 使用棘轮加密，在每条消息后更改密钥。在该协议中有永久密钥对，但是系统将临时密钥与永久密钥结合起来，为每条消息创建一个新的共享秘密密钥。

“完美前向保密”的实现使得信令协议非常流行。除了 Signal，WhatsApp 和 Google Duo 也将该协议用于其端到端加密实现。

* * *

## Signal 支持聊天备份/恢复吗？

是的，您可以在 Signal 上备份和恢复消息、图片、文件和其他内容。但是，聊天备份支持仅限于 Android。您不能在 iOS 或桌面版本上备份聊天。此外，所有备份都驻留在本地设备上，由于隐私问题，该应用程序不支持在线备份。

您可以在 Android 上启用备份，方法是导航到信号设置>聊天>聊天备份，然后点击打开。您将被要求在您的手机上保存此备份的位置。备份使用 30 个字符的密码加密。没有此密码，您将无法恢复备份。记下密码，然后点击启用备份。

如果您在手机上重新安装了该应用程序，您可以使用备份来恢复您的邮件。在 Android 上，当信号从一个设备传输到另一个设备时，也可以使用备份。您不能跨平台使用备份。

幸运的是，Signal for iOS 确实支持将聊天迁移到其他 iOS 设备，所以如果你有一部装有该应用程序的旧 iPhone，你可以使用它将消息迁移到你的新 iPhone。

* * *

这些是你需要知道的关于 Signal Private Messenger 的一些事情。它包含了许多其他功能和增强功能，我们无法在这里介绍，但如果你想了解更多关于该应用程序的信息，你可以访问 [Signal 的官方网站](https://signal.org/)。您是否计划从其他消息服务迁移到 Signal，或者如果您已经使用了一段时间，请在评论部分告诉我们您的体验。