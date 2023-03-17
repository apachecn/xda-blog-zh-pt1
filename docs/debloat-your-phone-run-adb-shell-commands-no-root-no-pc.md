# 如何在不连接电脑的情况下解锁手机(以及更多功能)

> 原文：<https://www.xda-developers.com/debloat-your-phone-run-adb-shell-commands-no-root-no-pc/>

Android Debug Bridge，简称 ADB，是一个很棒的开发工具，可以与您的手机进行接口，用于调试和测试。通过 ADB，开发者可以以比用户安装的应用更大的权限访问 Android 内置的 Linux 命令行 shell。这使开发人员能够安装或卸载应用程序，授予或拒绝权限，更改系统设置值，以及做更多的事情，所有这些都可以从命令行完成。虽然这些命令是为开发人员设计的，但也有助于您解除手机屏蔽、调整隐藏设置和启用其他选项。

ADB 命令可以发送到连接到 PC 或连接到与 PC 相同的无线网络的手机上。它们通常是从个人电脑的终端或命令提示窗口发送的，不能从手机本身发送，除非它已经被[根化](https://www.xda-developers.com/root/)。然而，通过一款名为 Local ADB Shell(简称 l ADB)的应用程序，ADB 命令可以直接从手机上发送，而不需要启动它或将其连接到 PC。

由 XDA 知名开发者 [tytydraco](https://forum.xda-developers.com/m/tytydraco.8155542/) 开发，LADB 利用 Android 对无线 ADB 的内置支持，提供了一个直接从设备发送 shell 命令的 GUI。在 Google Play 上搜索“终端模拟器”,你会发现几十个提供安卓命令行外壳访问的应用。LADB 与其他应用程序的不同之处在于，它在应用程序中捆绑了一个 ADB 服务器，这使得它可以被设置为以与 ADB shell 相同的权限运行 shell 命令。有了亚行的外壳特权，你可以从你的手机上做一些事情，比如[解除你手机的屏蔽](https://www.xda-developers.com/uninstall-carrier-oem-bloatware-without-root-access/)，改变隐藏的设置，以及[等等。](https://www.xda-developers.com/what-is-adb/)

不过，为了设置 LADB，你首先需要在 WiFi 上启用 ADB，但根据你的设备和 Android 操作系统版本的不同，这个过程会有所不同。

对于运行 Android 10 或更早版本的设备，[可以在 PC 上进行一些初始设置后](https://developer.android.com/studio/command-line/adb#wireless)启用无线 ADB。这意味着在旧版本的 Android 上，你仍然需要通过[在你的 PC 上设置 ADB](https://www.xda-developers.com/install-adb-windows-macos-linux/)。完成后，您就可以让应用程序向设备上启动的 ADB 服务器发送命令。

由于 Android 11 [引入了对无线调试的原生支持](https://www.xda-developers.com/android-11-developer-preview-3-announced/)，LADB 可以完全在设备上设置，而不需要 root 或连接到 PC 进行初始化。以下是如何在 Android 设备上设置 LADB 的方法。为了这个教程，我们假设你的设备运行 Android 11，因为如果不是，你将不得不[在你的 PC](https://www.xda-developers.com/install-adb-windows-macos-linux/) 上手动设置 ADB 来让它工作，这违背了使用 LADB 的主要目的。(如果你有一部运行基于 Android 10 的 OxygenOS 10 的一加手机，你可以使用 LADB wire 和 PC-free，因为一加内置了他们自己的无线调试功能。)

## 如何在 Android 11+上使用 LADB 解锁你的手机

1.  从 Google Play 下载并安装 [LADB 应用，或者从 source](https://play.google.com/store/apps/details?id=com.draco.ladb) 编译[。](https://github.com/tytydraco/ladb)
2.  打开“设置”>“关于手机”,点击“内部版本号”字段 7 次。这将启用“开发人员选项”(注意:“关于手机”页面可能会被称为其他名称或隐藏在设备设置中的其他位置。)
3.  前往“设置”>“系统”>“开发者选项”,启用“USB 调试”和“无线调试”(注意:与“关于手机”一样，“开发者选项”页面也可以在您设备的“设置”中找到。)
4.  打开 LADB 应用程序。它将显示一个“配对信息”对话框。
5.  打开最近的应用程序屏幕。按住应用程序的图标并点击“分屏”以在分屏多任务视图中打开 LADB。
6.  在下半部分，打开设置。进入系统>开发者选项>无线调试。点击“将设备与配对代码配对”您将看到一个弹出的“与设备配对”对话框。
7.  复制 6 位数的“Wi-Fi 配对代码”并将其粘贴到 LADB 的“配对代码”框中。从 IP 地址复制 5 位数端口号(冒号后的 5 个数字)并粘贴到 LADB 的“端口”框中。
8.  在 LADB 点击“ok ”,你应该会看到“成功！*\(^o^)/*”
9.  现在，您可以在底部的“shell command”框中键入您想要的任何 ADB shell 命令。找事情做？查看我们的亚洲开发银行教程列表，你可以尝试一下！

如果您在设置 LADB 时遇到问题，请务必点击右上角的三点菜单图标，然后转到帮助部分。您可以在此重置服务器，将应用恢复至出厂设置，并删除配对信息和 ADB 服务器文件。您还可以通读故障排除提示，找到常见问题的答案。

我在几个不同的设备上使用过 LADB，包括华硕 ZenFone 7 Pro 和运行 Android 11 的谷歌 Pixel 4。我在这两个平台上都没有遇到太多麻烦，但我确实注意到，任何启用了“网络调试”的安卓电视设备都会奇怪地干扰 LADB 的配对过程。如果您在配对时遇到问题，并且有 Android TV 设备，请检查以确保“网络调试”没有打开。当你试图在手机上设置 LADB 时，如果你看到电视上出现 ADB 授权提示，你就知道这是在干扰你。

如果您有任何反馈或问题要问开发人员，请查看下面链接的 LADB XDA 论坛主题，或者发电子邮件到[tylernij@gmail.com](mailto:tylernij@gmail.com)给开发人员。该应用也是[开源的](https://github.com/tytydraco/ladb)，如果你有兴趣为自己编译它 Google Play 上的价格可以被视为对开发人员制作该应用的捐赠！

**[LADB - XDA 论坛线程](https://forum.xda-developers.com/t/say-hello-to-ladb-a-local-adb-shell-without-needing-root-or-a-computer.4204855/)**