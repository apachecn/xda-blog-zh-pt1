# WhatsApp 准备为 Android 添加面部解锁支持

> 原文：<https://www.xda-developers.com/whatsapp-prepares-face-unlock-support-android/>

WhatsApp 是全球数亿用户的主要沟通方式之一。它是免费的，使用起来没有痛苦，即使 Telegram 等替代产品已经在功能上击败了它。脸书旗下的服务并不是每天都有新功能，但当它真的有了新功能时，这对用户来说是一个激动人心的时刻。我们已经知道几个新的 WhatsApp 功能正在酝酿中，如果来自 *[WABetaInfo](https://wabetainfo.com/whatsapp-beta-for-android-2-20-203-3-whats-new/)* 的报道属实的话，我们现在正在了解更多的功能。

在未来的某个时候，WhatsApp 增加了对指纹解锁的支持，允许 Android 用户轻松锁定应用程序，防止人们窥探你的私人谈话。然而，对于那些支持面部解锁的 Android 设备，你不能真正使用这个功能。一些 Android 设备，如谷歌 Pixel 4，有专门的传感器进行精确的 3D 面部识别，所以 WhatsApp 现在准备增加对更多形式的生物认证的支持。一旦该功能推出，“指纹锁”设置将被重命名为更通用的“生物识别锁”。

*图片来源:[WABetaInfo](https://wabetainfo.com/whatsapp-beta-for-android-2-20-203-3-whats-new/)*

我们猜测新的设置将基于 Android 的 BiometricPrompt API，该 API 允许应用程序使用面部扫描仪和指纹传感器进行生物认证。但是现在，没有办法知道这个特性是否可用，甚至在最新的测试版中也没有。然而，我们希望它能很快在未来的更新中出现。

Android 设备上面部解锁的采用已经停滞不前，尽管我们刚刚看到最近一个高调的设备发布会。第一个支持 3D 人脸解锁的主要 Android 设备是 Pixel 4 系列，谷歌一直在慢慢推动应用程序开发人员从旧的 FingerprintManager API 转换到新的 BiometricPrompt API。不过，现在已经没有太多动力支持面部解锁了，因为就连谷歌自己的 Pixel 5 也回到了安装在背面的老式指纹扫描仪上。由于新冠肺炎的兴起，戴面具的人越来越少，这意味着面部解锁不再受欢迎，这意味着指纹扫描仪的回归来得正是时候。尽管如此，很高兴看到 WhatsApp 等应用程序准备为那些少数实际上可以利用它的 Android 设备支持面部解锁。