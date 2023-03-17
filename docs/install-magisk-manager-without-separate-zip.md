# Magisk 经理 APK 现在可以在 TWRP 内部闪现了

> 原文：<https://www.xda-developers.com/install-magisk-manager-without-separate-zip/>

Magisk 的开发者 Topjohnwu 今天宣布了对流行的开源生根工具的重大改变。最大的变化是，根你的手机所需的二进制文件和脚本现在包含在管理器应用程序中，而不是通过互联网下载。因此，你只需要下载一个文件 Magisk 管理器 APK 的最新版本——就可以让你的手机 root 并管理 root 访问。

在今天的更新之前，安装 Magisk 最常见的方法是首先安装 Manager 应用程序，然后从 Manager 应用程序中下载最新的 flashable ZIP，其中包含 Magisk 安装所需的二进制文件和脚本，最后在像 TWRP 这样的自定义恢复中刷新该 ZIP。在今天的更新之后，你所要做的就是下载最新的经理 APK，把它的扩展名改为 ZIP，这样它就会被 TWRP 识别为一个可刷新的文件，然后刷新 ZIP。这可以工作的原因是，APK 文件遵循 ZIP 文件格式，所以[通过一些修改](https://github.com/topjohnwu/Magisk/commit/ec8fffe61cf6c2ce66a52d9e8b33cd6e60c7ceb8)，APK 既可以作为 Android 安装包，也可以作为 TWRP 认可的可闪存 ZIP 文件。

除了降低复杂性，这也使得整个安装和卸载过程完全离线。以前，管理器应用程序需要活跃的互联网连接才能从 GitHub 下载最新的 Magisk ZIP。因为所需的二进制文件和脚本包含在管理器 APK 中，所以您可以不需要下载任何文件到您想要作为根的目标设备上。

此外，topjohnwu 表示，通过将所有二进制文件作为管理器 APK 的“原生库”发布，管理器应用程序的目标 SDK 版本可以设置为 29 或更高。他说，原因是因为 Android 10 的 SELinux 限制在应用程序的主目录中执行文件，同样的限制也迫使 Termux 开发者放弃在 Google Play 上提供应用程序更新。但是，目标 SDK 版本尚未增加，将在未来的提交中解决。

和往常一样，你可以从 topjohnwu 的 [GitHub](https://github.com/topjohnwu/Magisk) 中找到 Magisk 的最新版本。你可以在这里找到最新的发行说明、安装说明和常见问题[。](https://topjohnwu.github.io/Magisk/)