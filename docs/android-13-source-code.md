# 谷歌开始向 AOSP 上传 Android 13 源代码

> 原文：<https://www.xda-developers.com/android-13-source-code/>

# 谷歌开始向 AOSP 上传 Android 13 源代码

在万众期待之后，谷歌终于发布了 Android 13 的源代码。最终版本也已经推出了！

经过一番期待，谷歌发布了 Android 13 的源代码。虽然发布时间比预期晚了一点，但该公司已经开始将源代码上传到 Android 开源项目(AOSP) Git 仓库。这通常需要一些时间，通常需要几个小时来完全填充更新。结果，没看到就耐心点。这次源代码发布也伴随着 Android 13 的[完整版。](https://www.xda-developers.com/android-13-released)

在发布之前，谷歌更新了其 [Android 13 安全发布说明](https://source.android.com/security/bulletin/android-13?hl=en)，其中包含了 Android 中存在的安全漏洞的详细信息。此次更新显示了 Android 13 中已修复的安全漏洞。运行安全补丁级别为 2022-09-01 或更高版本的 Android 13 的设备将免受这些问题的影响。如果你想检查你正在运行的 Android 版本和安全补丁级别，大多数制造商都会在设置下的关于手机部分列出。

Android 13 源代码的发布非常重要，不仅对于那些想要修补操作系统的人来说如此，对于像 LineageOS 这样构建定制 rom 和 Android 售后发行版的社区来说也是如此。主要制造商也必须依赖这个库来发布他们自己的 Android 版本。你可以去[谷歌 Git](https://android.googlesource.com) 看看 Android 13 的源代码。

对于开发者来说，这是一个重要的时刻，因为是时候发布兼容版本的应用程序，并利用 API 构建更多功能了。谷歌正在发布 Apache 许可证版本 2.0 下的 Android 13 源代码。Apache 2.0 是一个许可的而不是版权所有的许可证，这意味着开发人员可以自由地修改和分发代码，而不需要开源他们的修改。这种许可制度允许智能手机制造商开发自己的 Android 闭源分支。

如果你对分析 Android 13 源代码感兴趣，你可以去 [Android Git 仓库](https://android.googlesource.com/)寻找新的 Android 13 分支和标签。具体来说，就是寻找“android-13.0.0_r#”标签。谷歌内部代码库的整体被推送到公共的 AOSP 库需要一段时间，所以在你可以同步所有东西之前，预计要等几个小时。谷歌还上传了每个版本的提交历史，这为 Android 团队在添加或删除功能时的思维过程提供了很多见解。