# 这就是为什么你不能下载谷歌相机和录像机的更新

> 原文：<https://www.xda-developers.com/google-camera-recorder-sideload-failed-verification-android-11/>

当谷歌在 10 月份推出 Pixel 5 时，我们很高兴能接触到它的新应用。(手机本身[也很酷](https://www.xda-developers.com/google-pixel-5-review/)。随着 Pixel 5 的发布，我们与社区分享了新版的[谷歌相机](https://www.xda-developers.com/download-google-camera-8-0-from-pixel-5-other-pixel-phones/)和[谷歌录像机](https://www.xda-developers.com/download-google-recorder-2-0-pixel-5-other-pixel-devices/)应用。然而，当许多旧 Pixel 设备的用户试图下载更新时，他们遇到了一个错误(如上所示)。奇怪的是，并不是每个人都有安装更新的问题。有些人能够很好地安装它们，而其他人不得不进行工厂重置，以便安装新版本。由于这个问题看似随意，许多人将其归因于一个错误。我们现在很有信心，这个问题不是源于一个错误，而是谷歌在 Android 11 中使用了一个新的 API 来阻止侧载更新。

如果你试图在运行 Android 11 的 Pixel 设备上侧载谷歌相机 8.0 或更高版本或谷歌记录器 2.0 或更高版本，你会看到一条错误消息，称验证无法成功。即使您尝试使用 shell 命令从侧面加载 APK，您也不会得到安装失败的更具体的原因。您将得到的安装返回代码是"[INSTALL _ FAILED _ VERIFICATION _ FAILURE](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/core/java/android/content/pm/PackageManager.java;l=1340?q=INSTALL_FAILED_VERIFICATION_FAILURE)"，不幸的是，它没有告诉您为什么验证没有成功。通过检查 logcat，我们可以了解验证失败的确切原因:

```
 AppIntegrityManagerServiceImpl: Integrity check of com.google.android.GoogleCamera result: DENY due to [Rule: (PACKAGE_NAME EQ com.google.android.GoogleCamera) AND (VERSION_CODE GTE 32045130) AND (APP_CERTIFICATE EQ F0FD6C5B410F25CB25C3B53346C8972FAE30F8EE7411DF910480AD6B2D60DB83) AND NOT (INSTALLER_NAME EQ com.android.vending), DENY] 
```

根据该消息，对 Google Camera 安装的完整性检查失败，因为“INSTALLER_NAME”与谷歌 Play 商店的包名“com.android.vending”不匹配。(我试图用 APKMirror 安装程序安装谷歌相机 8.0，不管它值不值得。)这条消息是由“[AppIntegrityManagerServiceImpl](https://android.googlesource.com/platform/frameworks/base/+/android11-release/services/core/java/com/android/server/integrity/AppIntegrityManagerServiceImpl.java)”添加到系统日志中的，这是 Android 新的“应用完整性”功能的一部分。根据 AOSP 的代码，App Integrity 旨在在软件包管理器现有的 APK 签名验证的基础上提供额外的一层检查。App Integrity API 似乎使用一套[规则](https://android.googlesource.com/platform/frameworks/base/+/master/core/java/android/content/integrity/Rule.java)来决定是否允许或拒绝安装。规则由一个系统应用程序提供——我们认为是 Google Play 服务——并且[存储在一个文件](https://android.googlesource.com/platform/frameworks/base/+/master/services/core/java/com/android/server/integrity/IntegrityFileManager.java)中。

此外，如果清单的元数据中嵌入了“源标记”，App Integrity [还会调用另一个名为](https://android.googlesource.com/platform/frameworks/base/+/android11-release/services/core/java/com/android/server/integrity/AppIntegrityManagerServiceImpl.java#484)[的类](https://android.googlesource.com/platform/frameworks/base/+/master/core/java/android/util/apk/SourceStampVerifier.java)。例如，下面是我们认为来自谷歌相机应用程序清单的“源戳”:

```
 <meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/> 
```

据我们所知，source stamp 用于验证包安装程序的签名。因此，举例来说，你不能欺骗 AppIntegrity 允许安装，即使你[冒充 Play Store](https://developer.android.com/studio/command-line/adb#-t-option:~:text=APK.-,%2Di) 作为安装程序。

除此之外，我们无法确切了解谷歌如何使用 AppIntegrity 和相关 API 来阻止谷歌相机和谷歌录像机应用程序的侧装更新。对 APK Google Play 服务的快速检查显示，它正在使用这些 API，但代码过于混乱，无法真正理解所有内容。我们甚至找到了存储完整性规则的目录— /data/system/integrity_rules —但是它没有什么用处，因为它只包含序列化的数据。我们也没有找到禁用完整性验证的方法(这似乎不像只是[改变设置](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/core/java/android/provider/Settings.java;l=10026?q=INTEGRITY_CHECK_INCLUDES_RULE_PROVIDER)那么简单)，尽管我们认为工厂重置对一些人有效的原因是 Google Play 服务没有机会初始化其规则集来阻止安装。尽管如此，logcat 消息和 Android 11 中这些新 API 的引入强烈表明这完全是设计使然，而不是一个错误。

谷歌还没有公开评论其对这些 API 的使用(我们也不期望他们这样做)，当被联系评论时，他们也没有回应。不过，我们有一些理论来解释为什么他们会阻止侧装更新。首先，它们可以防止人们为他们的设备安装错误版本的应用程序。谷歌向特定的像素设备提供特定版本的应用程序。例如，可以在网上找到几个版本的设备个性化服务应用程序。尽管它们都可以安装在 Pixel 设备上，但通过下载为旧 Pixel 设备构建的版本，[可能会在 Pixel 4 上失去直播字幕功能](https://twitter.com/MishaalRahman/status/1197930331397070848)。另一个原因可能是“提高未经授权发布的应用程序的可追溯性”，正如 Google 在 SourceStampVerifier 类中解释的那样。

到目前为止，只有少数使用应用捆绑格式的谷歌应用(如谷歌相机和谷歌录像机)阻止非播放商店安装，但我们不知道该公司是否会将这种行为扩展到其他应用[，一旦它们都转换到 AAB 格式](https://www.xda-developers.com/google-android-app-bundle-play-store/)。我们还考虑了转换到应用捆绑包是否有必要实现应用完整性，但我们发现当用户试图安装一个不具备所有必要分裂的应用时，谷歌已经[有了一个解决方案](https://stackoverflow.com/a/60622124)来处理。无论情况如何，我们不认为谷歌打算阻止其应用程序的所有侧装，尽管这些工具肯定允许他们这样做。

*感谢开发人员 vvb2060、aviraxp 和 Quinny899 对本文的帮助，感谢 t* *到 PNF 软件公司为我们提供了使用许可* *[JEB 反编译程序](https://www.pnfsoftware.com/?aid=xdadev)* *，这是一款用于 Android 应用程序的专业级逆向工程工具。*