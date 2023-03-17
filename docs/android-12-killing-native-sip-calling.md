# Android 12 准备取消对 SIP 通话的原生支持

> 原文：<https://www.xda-developers.com/android-12-killing-native-sip-calling/>

会话发起协议，或称 [SIP](https://en.wikipedia.org/wiki/Session_Initiation_Protocol) ，是一种常用于通过互联网进行语音通话的协议。几年前，SIP 客户端和提供商相当受欢迎，因为他们提供免费或廉价的全球互联网通话，而许多美国运营商甚至没有在其网络上提供无限制的语音通话。多年来，Android 原生支持添加 SIP 帐户并通过默认拨号器拨打 SIP 电话，但随着 [Android 12](https://www.xda-developers.com/android-12/) 更新，这一点似乎将不复存在。

从 Android 12 开始，股票拨号器应用程序似乎不再提供 SIP 设置，在 Pixel 手机上，股票拨号器应用程序是谷歌手机应用程序。这意味着您不能添加 SIP 帐户或使用普通拨号器拨打 SIP 电话。

谷歌通过 Wi-Fi 打电话的[支持页面](https://support.google.com/phoneapp/answer/2811843?hl=en#zippy=%2Coption-use-a-voip-service-to-make-calls-over-wi-fi%2Coption-use-a-mobile-carriers-wi-fi-calling)仍然将 SIP 列为一个选项，但他们的开发者文档指出, [SipManager 类](https://developer.android.com/reference/kotlin/android/net/sip/SipManager)在 API level 31 中已被否决。尽管这个类被弃用了，但它看起来并没有完全移除 Android 的原生 SIP 堆栈——至少现在还没有。

基于这些承诺，谷歌似乎准备从 Android 的电话服务中完全移除 SIP 呼叫支持。一旦 SIP 服务从框架中移除，依赖安卓原生 SIP 堆栈的应用[可能会崩溃。由于提交的内容似乎还没有合并，像](https://developer.android.com/guide/topics/connectivity/sip) [ACR Phone Dialer](https://play.google.com/store/apps/details?id=com.nll.cb) 这样拥有自己 SIP 客户端的第三方应用应该可以在 Android 12 上继续工作，但我们尚未验证它们是否可以工作。如果您有一个 SIP 帐户，并且可以通过依赖于 Android 原生 SIP 堆栈的第三方 SIP 客户端验证通话仍然有效，请务必让我们知道！

无论如何，很明显谷歌不再认为在 Android 中保留 SIP 支持是值得的。SIP 堆栈已经很多年没有更新了，所以它几乎已经被抛弃了——这些代码变化只是使它变得正式。

*感谢 XDA 公认的开发者 [luca020400](https://forum.xda-developers.com/m/luca020400.5778309/) 的提示！*