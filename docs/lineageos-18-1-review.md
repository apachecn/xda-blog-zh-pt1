# LineageOS 18.1 回顾:Android 11，来到你身边的老手机

> 原文：<https://www.xda-developers.com/lineageos-18-1-review/>

LineageOS 在公司支持的 CyanogenMod 项目崩溃后，于 2016 年创建，作为一个类似股票的 Android 定制 ROM。自那以后，它经历了几次重大更新，但 LineageOS 继续为几十款手机和平板电脑带来类似于股票的 Android(也可以选择不使用谷歌)体验。最近的版本——T2 linea geos 18.1 T3——终于在三月底发布，为 50 多种设备提供 Android 11。

不过，18.1 版本带来的不仅仅是底层 Android 操作系统的更新——一如既往，Lineage 在谷歌开源 Android 代码的基础上添加了自己的功能。新版本中有太多需要探索的地方，所以我们决定对它进行全面的审查。

## 安装 LineageOS 18.1

如果你曾经在手机或平板电脑上安装过定制的 ROM，那么 LineageOS 18.1 的过程可能不会有太大的不同。Lineage 与其他 rom 最重要的区别是 Lineage 提供了自己的恢复软件，而不是依赖于第三方恢复系统，如 TWRP。虽然你*应该*还能在 LineageOS 18.1 上使用 TWRP，但还是建议坚持使用项目自己的恢复软件(如果你设备的维护者这么建议的话)。

我用了一个谷歌 Pixel 3a XL 来试用 LineageOS 18.1，所以[安装过程](https://wiki.lineageos.org/devices/bonito/install)相对简单。我在我的电脑上使用 [ADB 和 Fastboot](https://www.xda-developers.com/install-adb-windows-macos-linux/) 解锁了引导加载程序，然后用一个简单的 Fastboot 命令临时刷新了血统恢复。一旦你进入了恢复软件，你必须用 ADB 加载最新的 LineageOS 版本，这样就可以安装操作系统和恢复分区。之后，如果你愿意，你可以刷新 Google apps 或根包，然后重启设备到完整的系统。

我在安装 [MindTheGapps](http://downloads.codefi.re/jdcteam/javelinanddart/gapps/) 时确实遇到了问题 Gapps 安装程序会说一切都很成功，但当我启动 LineageOS 时，就没有谷歌应用了。执行另一次工厂重置，并在安装 Lineage 和 Gapps 之间重新启动恢复分区，最终修复了这个问题。我不确定这是 Lineage 的恢复软件还是 zip 包的问题，但不管是哪种情况，我都尝试了几次让 Lineage 与常用的谷歌应用程序一起工作。确保你完全按照书写的步骤*去做*，以减少任何问题发生的几率。

## 你好，安卓 11

如果你安装了 Gapps 包，LineageOS 的初始设置过程与 Pixel 手机非常接近。你登录一个谷歌账户，选择你的备份和同步选项，设置语音匹配，并做一些其他杂项步骤。如果你没有谷歌应用和服务，你通常会被要求提供姓名、时区和其他基本信息。

通过设置屏幕，你会看到 Trebuchet，这是自 CyanogenMod 时代以来默认的主屏幕启动器。它在功能上接近 Pixel Launcher，但有一些附加功能。你可以使用图标包，但与一加的 OxygenOS 不同，定制图标只显示在主屏幕和应用抽屉上(而一加会在整个系统中显示它们)。

你还可以通过 PIN 或指纹隐藏启动器中的应用程序，这也可以隐藏 widget 菜单中的 widget。最后，还有图标标签和锁定编辑的额外选项。那些拥有高度定制主屏幕的人可能会坚持使用其他发射器，但 Trebuchet 几乎拥有我个人想要的主屏幕上的所有东西。

LineageOS 18.1 的其余部分看起来和感觉上与运行 Android 11 的 Pixel 或诺基亚手机没有太大区别。媒体控制出现在快速设置面板中，提醒被分成对话(其中一些可以显示为浮动气泡)和其他通知，智能家居设备([或 Tasker tasks](https://www.xda-developers.com/tasker-test-hijacks-android-11-power-menu/) )可以从电源菜单中管理，等等。如果 Android 11 中有什么东西，最有可能是 LineageOS 18.1 中的。

尽管 LineageOS 与普通 Android 相比已经增加了一些额外的安全/隐私功能，但 LineageOS 18.1 受益于 Android 11 带来的许多安全相关的改革。[临时权限](https://www.xda-developers.com/android-11-developer-preview-privacy-security-features-changes/#:~:text=One-time%20Permission%20Access)防止应用程序重复获取位置、麦克风和摄像头数据。应用程序也无法在后台获取你的位置。最后，Android 11 标志着谷歌向[范围存储](https://www.xda-developers.com/android-11-developer-preview-privacy-security-features-changes/#:~:text=Scoped%20Storage%20changes)过渡的开始，这是一种有争议的 API，它限制第三方应用程序可以访问你设备上的哪些文件。虽然对 Scoped Storage 的工作方式有一些[有效的抱怨](https://www.xda-developers.com/android-q-storage-access-framework-scoped-storage/)，但我个人仍然是一个粉丝——它不会阻止对我经常需要访问的任何文件夹的访问，我手机上的大多数应用程序也没有理由无限制地访问我手机上的所有本地文件。

当然，LineageOS 18.1 缺少一些功能，即使你安装了谷歌应用套件。定制的 rom 没有通过谷歌的安全网测试，所以一些应用程序会拒绝运行，而其他的则会隐藏在 Play Store 搜索结果之外(比如网飞和 Hulu)。安装 root 和 Magisk 可以修复这一点，但绕过 SafetyNet 最终是谷歌和开发者之间的猫捉老鼠游戏，它很可能会在某个时候停止工作。

令我惊讶的是，我的 Pixel 3a XL 上的 LineageOS 保持了对宽藤 L1 的支持，所以只要你最喜欢的流媒体服务在运行时不需要安全网检查，它应该在 LineageOS 18.1 上运行良好。一旦我从 APK 安装了 Hulu(Play Store 列表对修改后的设备是隐藏的)，电影和电视节目就能以原始质量播放。这可能因设备而异，但这是我在 Pixel 3a XL 上的体验。

## LineageOS 18.1 系统功能

LineageOS 18.1 保留了 LineageOS 和 CyanogenMod 以前版本中的大多数非库存功能。状态栏可以大量定制，具有各种时钟/电池样式和可选的网络流量监视器。你还可以改变时钟在屏幕的哪一边，这样你就可以重温 Android 把时钟放在右边的美好时光。

LineageOS 18.1 还为你的手机或平板电脑的按钮提供了比库存 Android(和大多数 OEM 皮肤)更多的选项。如果你坚持默认的三按钮导航条，你可以设置自定义的动作来按住或者双击主屏幕按钮和长按最近按钮。电源按钮可以设置为打开或关闭手电筒(对于我深夜遛狗来说，这是一个非常有用的附加功能)，音量摇杆可以接听电话或控制音乐播放。

系统配置文件也从以前版本的 LineageOS 和 CyanogenMod 中回归。它们的功能类似于三星设备上的 [Bixby 例程](https://shop-links.co/1737249278333429435?u1=1d0c526f-344f-4882-9c63-827d248dd479)以及 iPhones 和 iPads 上的[快捷方式](https://support.apple.com/guide/shortcuts/welcome/ios)，允许您在您定义的触发器(例如连接到某个 Wi-Fi 网络或蓝牙设备)被激活后更改一些系统设置。例如，您可以在回家时让环境显示自动关闭，或者在工作时将媒体音量设置为 0%。

对于简单的自动化来说，拥有系统配置文件是很好的，但是该功能主要限于改变设备设置。您不能自动打开应用程序，也不能使用通知和其他常见操作作为触发器。任何希望创建更复杂设置的人都会更喜欢使用 [Tasker](https://forum.xda-developers.com/f/tasker-tips-tricks.5015/) 。

## LineageOS 18.1 系统应用程序

Android 操作系统是开源的，但你需要完整的智能手机体验的大多数应用程序都不是。谷歌几年前就停止了在 AOSP 积极维护大部分应用程序，在零售设备上用谷歌化的版本(如 Gboard、Gmail 等)取代它们。).这导致 LineageOS 项目不得不更新或彻底替换许多谷歌放弃的系统应用程序。

取决于你如何安装 LineageOS 18.1，你可能看不到这些应用程序中的一些或全部——许多谷歌应用程序安装程序会卸载或禁用它们，所以你不会得到两个时钟应用程序或两个电子邮件客户端。一些非官方版本也可能没有它们。

LineageOS 浏览器仍然是我最喜欢的应用程序项目，部分原因是它设计良好，具有足够的现代网络浏览功能，还因为它在系统最近菜单中显示标签。在棒棒糖时代，这是 Chrome 的一个选项，但是几年前就被移除了。然而，它不支持许多现代 web 应用程序功能，包括推送通知和离线缓存。

还有一个计算器应用程序，包括你在科学计算器中看到的大多数功能，通过向下滑动可以访问历史记录。时钟和联系人应用程序几乎与 Pixel 手机上的相同，还有一个用于在音频配置文件之间切换的 AudioFX 实用程序。如果您过去使用过 LineageOS，这里没有多少新内容。

LineageOS 18.1 中的日历应用程序与你在以前版本中发现的完全不同——linea geos 没有继续维护过时的(heh) AOSP 日历应用程序，而是派生了开源的 [Etar 日历](https://github.com/Etar-Group/Etar-Calendar)(它本身基于 AOSP 日历)并添加了一些更改。它可以显示任何使用 Android 内置 CalDAV 提供程序同步到你的设备上的日历，通常看起来和工作起来都很棒。同样，开源的 [SeedVault](https://calyxinstitute.org/projects/seedvault-encrypted-backup-for-android) 应用已经集成到 LineageOS 中，允许你在没有谷歌账户的情况下备份你设备的设置和数据。

LineageOS 18.1 也有自己的图库应用，与 Google Photos 相比有点简陋，但仍然支持相册，并有简单的图片编辑器。照片只能以大网格平铺显示，并且不能快速跳转到某个月份或年份，因此找到一张特定的图像可能会很困难。对于不一定是照片的文件，有一个文件应用程序，它只需打开 Android 的文件选择器。

说到照片，LineageOS 18.1 中有一个相机应用程序，它有一系列不错的设置和切换，尽管大多数都需要点击几下才能到达。照片、视频、全景和二维码有单独的模式，顶部有一个汉堡菜单可供选择。我的 Pixel 3a XL 的照片质量似乎比谷歌相机应用程序差一点，谷歌相机应用程序是定制 rom 的正常程序。照片和视频质量因设备而异，但有[改进的 GCam 应用程序](https://www.xda-developers.com/google-camera-port-hub/)可用于大多数应该在 LineageOS 等定制 rom 上工作的手机。

LineageOS 18.1 上像素 3a XL 的照片样本

LineageOS 18.1 中的默认消息应用程序与大多数其他应用程序一样:没有太多功能，但它很实用，看起来很干净。您可以轻松管理群组对话、阻止特定号码以及发送图像和联系人等附件。Messages 应用中没有 RCS 支持，因为谷歌[仍然没有向第三方客户端开放 RCS API](https://www.xda-developers.com/google-rcs-api-3rd-party-apps/)——你需要安装 Play 服务和[谷歌 Messages](https://play.google.com/store/apps/details?id=com.google.android.apps.messaging) 。有趣的时光。

LineageOS 18.1 中的电话拨号应用程序或多或少与谷歌手机相同，尽管其设计比谷歌更新(也更白)的设计语言更适合早期的材料主题。还有一个基本的语音记录器应用程序，带有方便的通知控制，以及改变音质的选项。没什么特别的，但它让我不必下载可能有弹出广告的第三方记录器应用程序。

LineageOS 18.1 中最后一个 note 的系统应用是音乐，和 LineageOS 17.1 变化不大。你可以按艺术家或专辑对本地存储的音乐进行分类，创建播放列表，或者只是查看你拥有的每首歌曲的庞大列表。一个新功能是通知现在有一个搜索栏，就像 Android 10 首次发布时添加的许多音乐和播客播放器一样。我希望播放屏幕上的控件大一点，但这真的是我唯一的抱怨。

这个列表中缺少了一个应用程序:电子邮件客户端。LineageOS 已经决定放弃其位于 AOSP 的电子邮件应用程序，一名开发者称其为“老旧、不安全、过时”Gmail 已经与第三方电子邮件客户端合作多年，有一些开源电子邮件应用程序可供选择(如 [K-9 邮件](https://k9mail.app/)，所以这并不是太大的损失。

## 结论

LineageOS 一直有两个主要目标:让旧手机和平板电脑保持更新，并让你对你的设备有更多的控制权。LineageOS 18.1 最终在这两个方面都取得了成功，因为它为 50 多种手机和平板电脑提供了正式版本(更多版本正在开发中)，同时保留了以前版本中大多数经典的 LineageOS 和 CyanogenMod 功能。由于 LineageOS 及其设备维护人员的努力工作，即使像 LG G2 和三星 Galaxy S4(都是 2013 年生产的)这样老的手机也可以运行与 2021 年发布的新 1000 美元手机相同的操作系统。

LineageOS 18.1 继续携带着另一个重要的衣钵:保持*开放* Android。谷歌已经放弃了 AOSP 的许多核心应用，因此天堂团队已经介入填补空白。网络浏览器、画廊、音乐播放器和其他应用程序有助于创建完整的智能手机体验，无需专有软件或多次前往 F-Droid 应用程序商店。当然，如果你想安装 Google Play 服务，这不是一个问题，但对于那些试图将手机去谷歌化的人来说，这很重要。

LineageOS 是多么完整的一个包，而且它仍然可以免费下载和安装，我很难抱怨什么。你仍然需要一台 PC 和一些基本的终端知识来安装它，偶尔会有应用程序阻止修改后的设备，但仅此而已。

如果你有兴趣试用 LineageOS，请前往[官方网站](https://lineageos.org/)下载和安装指南。如果可以的话，在 [PayPal](https://paypal.me/LineageOS) 或 [Patreon](https://patreon.com/LineageOS) 上为这个项目投点钱——服务器不是免费的。