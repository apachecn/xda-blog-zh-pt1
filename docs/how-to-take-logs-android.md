# 如何在 Android 上记录日志:Logcat、dmesg 和 ramoops

> 原文：<https://www.xda-developers.com/how-to-take-logs-android/>

当开发人员诊断一个软件的错误时，日志非常有用。因此，作为一名用户，当你向开发者抱怨他们的 Android 应用程序或售后固件(定制 ROM)的问题时，他们会要求你提交一份日志来帮助他们解决问题。Android 包括许多处理固件不同部分的日志，有许多方法可以收集这些日志。在本指南中，我们将讨论各种常见的日志，以及如何在 Android 上收集这些日志以用于错误报告。

在我们开始之前，您应该在您的计算机上设置 Android 调试桥，因为您可能需要 ADB 访问这些日志。关于如何在任何电脑上设置 ADB，我们有一个很好的指南。

## 内核紧急日志

内核紧急日志有助于了解在不成功的引导过程中发生了什么。如果你试图运行一个定制的 ROM，但是你的手机在启动循环时卡住了，你可以收集内核紧急日志来帮助 ROM 开发者找出错误所在。

大多数 Android 制造商在出现紧急情况后使用上游的“pstore”和“ramoops”驱动程序来存储内核日志。Ramoops 在系统崩溃前将其日志写入 RAM。使用 root 访问权限，可以从以下位置检索这些日志:

```
 /sys/fs/pstore/console-ramoops 
```

文件名可能略有不同，但它将位于 pstore 目录中。你可以使用亚行拉或任何其他你想要的方式。例如:

`adb pull /sys/fs/pstore/console-ramoops C:\Users\Gaurav\Desktop\filename`

## 驱动程序消息

来自驱动程序消息缓冲区的日志可用于诊断系统驱动程序的问题以及某些东西不工作的原因。在 Android 上，您可以使用“dmesg”输出来获取这些日志。不过，您将需要 [root 访问权限](https://www.xda-developers.com/root/)来获取这些日志。使用以下 ADB 命令导出完整的日志。

```
 adb shell su -c dmesg > dmesg.log 
```

## 系统日志

当系统中出现错误时，系统日志非常有用。Android 允许使用 Logcat 收集系统日志。可以在 Android Studio 的 Logcat 窗口中查看日志消息，也可以使用命令行工具来获取日志消息。

Google Play 商店中也有几个 Android 应用程序，可以轻松访问这些工具。我们将在本文后面讨论这些应用程序。此外，一些定制的 rom 在开发者设置中带有收集系统日志的选项。

要使用 ADB 收集日志，请使用以下命令。这个命令将导出一个连续的日志，所以使用 Ctrl + C 来停止它。

```
 adb logcat > logcat.txt 
```

您可以使用-d 参数一次性导出完整的日志。

```
 adb logcat -d > logcat.txt 
```

如果您愿意，也可以使用以下命令查看或保存无线电缓冲区。

```
 adb logcat -db radio > radio.txt 
```

如果您的设备是 rooted 用户，您可以使用设备本身的终端应用程序来收集日志。要使用手机上的终端保存日志，请键入以下命令，以便将日志保存在手机上。

```
 logcat -d -f /sdcard/logcat.txt 
```

## 用于收集日志的 Android 应用

### Logcat Extreme

Logcat Extreme 可以帮助您读取 Logcat 和 dmesg 输出以及记录日志。需要 root 访问权限才能正确显示日志。

### Logcat 阅读器

Logcat Reader 是一款开源应用，可以让你读取和保存系统日志。它根据日志优先级对日志进行颜色编码。

### live boot(live boot)

这个应用程序不是 logcat 的合适替代品，但它以自己的方式很酷，值得一提。这个应用的重点不是实际上帮助你调试，而是给你一个另类的开机动画，看起来像是从科幻电影里出来的。

LiveBoot 用 logcat 和 dmesg 输出替换设备的引导动画。它的输出配置包括 logcat 级别、缓冲区和格式选择、是否显示 dmesg 等等。它需要 root 访问权限以及 SuperSU 版本 2.40 或更新版本。你可以在其 [XDA 主题](https://forum.xda-developers.com/t/app-5-0-root-2020-12-21-liveboot-logcat-dmesg-boot-animation-v1-84.2976189/)中找到关于该应用的更多信息。

* * *

这些是你可以在 Android 上收集日志的一些方法。如果你正在寻找一种在你的 Android 手机上获得 root 权限的方法，看看我们关于如何给你的手机 root 的详细指南[。](https://www.xda-developers.com/root/)