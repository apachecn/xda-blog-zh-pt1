# 谷歌详细说明了开发者何时必须使用安卓应用捆绑包

> 原文：<https://www.xda-developers.com/google-android-app-bundle-play-store/>

谷歌周四详细说明了开发者何时必须使用 Android 应用捆绑包在 Play Store 上发布内容。

搜索巨头[表示](https://android-developers.googleblog.com/2020/11/new-android-app-bundle-and-target-api.html)从 2021 年 8 月开始，Google Play 控制台将要求所有新应用与 Android 应用捆绑发布(。aab)格式。谷歌在 I/O 2018 上首次推出了替代应用分发格式，后来在今年早些时候宣布了即将到来的强制性要求。

[正如我们所解释的](https://www.xda-developers.com/google-play-billing-v3-app-bundle-requirement-2021/#div-gpt-ad-xda-developerscom35950:~:text=Mandatory%20Android%20App%20Bundles%20for%20Newly%20Published%20Apps%20in%202021)，Android 应用捆绑包的目标是减少最终 Android 应用包的文件大小。apk)交付给用户，减少了用户的安装大小和下载时间。

> 的。aab 文件包含基本应用程序大小和所有支持的架构(ARM、ARM64 和 x86)、语言和布局变体的 APK 文件。这种格式要求向 Google 提供一份应用程序签名密钥的副本，以便 Google Play 开发者控制台可以生成一个捆绑包，其中包含每个 APK 的签名版本；特定设备的架构、语言和布局的正确 APK 通过 Google Play 动态交付交付。

谷歌表示，转向 Android 应用捆绑交付也将影响使用传统即时应用 ZIP 格式的即时体验。这家搜索巨头表示，从 2021 年 8 月开始，新的即时体验和现有即时体验的更新将被要求发布即时应用捆绑包。

从消费者的角度来看，不会有太大变化。但是开发者和死忠用户可能会注意到一些不同。Android 应用捆绑包将使其他平台上的再分发更加困难，而 aab 更难手动侧装，这可能会导致一些令人头疼的问题。

谷歌还表示，从 2021 年 8 月开始，谷歌 Play 控制台将要求所有新应用程序利用播放资产交付或播放功能交付来交付下载大小超过 150MB 的资产或功能。新应用将不再支持扩展文件(OBB)。开发者还将被要求从 2021 年 8 月开始，针对上传到 Google Play 的新应用，将 API 级别设定为 30(Android 11)；与此同时，从 2021 年 11 月开始，现有应用的更新必须以 API 级别 30 为目标。