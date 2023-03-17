# 谷歌下个月将最终允许应用程序请求访问 Android 11 上的所有文件

> 原文：<https://www.xda-developers.com/android-11-all-files-access-permission-form/>

谷歌已经开始向那些应用程序要求广泛访问设备存储的开发者发送电子邮件。这封邮件告诉开发者，从 5 月 5 日开始，他们必须告知谷歌为什么他们的应用程序请求广泛的存储访问权限，否则他们将不得发布针对 Android 11 的更新。

在 Android 11 之前，应用程序可以通过在清单中声明 READ_EXTERNAL_STORAGE 权限并请求用户授予它来请求对设备存储的广泛访问。许多没有合法需求读取设备存储上存储的所有文件的应用程序都在请求这一权限，导致谷歌通过 Android 11 的“范围存储”变化缩小了存储访问权限。然而，对于合理需要更广泛存储访问的应用程序，如文件管理器，谷歌鼓励他们继续以 Android 10 (API 级别 29)为目标，并通过在清单中声明`requestLegacyExternalStorage=true`来请求“传统”存储访问。

传统访问允许应用程序广泛访问设备的存储，而不受[范围的存储限制](https://www.xda-developers.com/android-q-storage-access-framework-scoped-storage/)。然而，所有面向 Android 11 (API 级别 30)及以上版本的应用都受到范围存储限制的约束，不能请求对设备存储的传统访问。相反，他们必须请求名为 MANAGE_EXTERNAL_STORAGE(向用户显示为“所有文件访问”)的新权限，以获得广泛的存储访问权限(不包括少数目录，如/Android/data 或/Android/obb)。

从 2021 年 11 月开始，提交到 Google Play 的所有应用和应用更新都必须以 Android 11 为目标，这意味着文件管理器应用和其他需要更广泛存储访问的应用最终必须切换到范围存储模式，并请求所有文件访问权限。唯一的问题是，谷歌目前不允许开发者请求“所有文件访问”权限。谷歌早些时候表示，在该应用被允许在 Google Play 上使用之前，它希望[开发者签署一份声明表](https://www.xda-developers.com/google-file-manager-devs-submit-form-broad-file-storage-access-android-11/)。这份声明旨在让谷歌剔除不需要“所有文件访问”的应用，就像谷歌如何限制对[短信、](https://www.xda-developers.com/google-play-developer-policy-call-log-sms/)通话记录和 [QUERY_ALL_PACKAGES](https://www.xda-developers.com/google-is-restricting-which-apps-can-see-the-other-installed-apps-on-your-device/) 权限的访问。

尽管谷歌早在 2019 年 11 月就宣布他们打算让开发者签署一份声明表格，但他们仍然没有让这些声明表格实际可用。该公司列举了来自新冠肺炎疫情的劳动力挑战，以解释他们为什么推迟允许针对 Android 11 的应用程序，并要求将“所有文件访问”上传到 Google Play。谷歌[将未指明的日期“2021 年初”](https://www.xda-developers.com/google-play-july-2020-policy-update-introduces-extended-timeline-compliance-detailed-violation-emails-other-changes-developer-console/)定为他们公开声明表格的时间。

现在，谷歌终于[开始通知开发者](https://www.reddit.com/r/androiddev/comments/mqzls8/ominous_scoped_storage_warning_messages/)应用程序何时可以请求“所有文件访问”权限。发给开发者的邮件措辞混乱，但是一个[新发布的支持页面](https://support.google.com/googleplay/android-developer/answer/10467955)增加了一些清晰度。根据支持页面，针对 Android 11 并请求“所有文件访问”的应用程序最终可以从 2021 年 5 月开始上传到 Google Play，这大概是申报表上线的时候。关于“所有文件访问”的允许使用、例外和无效使用的列表，以及建议的替代 API，[请访问谷歌的支持页面](https://support.google.com/googleplay/android-developer/answer/10467955)。