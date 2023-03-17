# 如何在旧款 Pixel 手机上启用 Pixel 5 的自适应声音功能

> 原文：<https://www.xda-developers.com/enable-pixel-5-adaptive-sound-feature-older-pixel-devices/>

谷歌本月早些时候推出了第五款 Pixel 功能 Drop ，为新旧 Pixel 手机带来了许多新功能。一些老款 Pixel 手机获得了 Hold for Me 和 Extreme Battery Saver 等功能，而只有谷歌最新的 Pixel 4a 5G 和 Pixel 5 支持新的自适应声音功能。自适应声音功能旨在通过根据周围环境调整均衡器来改善手机的音频输出，多亏了 XDA 公认的开发者 [Freak07](https://forum.xda-developers.com/m/freak07.3428502/) ，有一种方法可以在旧的 Pixel 设备上启用该功能。如果你有兴趣在你的手机上尝试一下，下面是你需要做的:

## 在旧的 Pixel 设备上启用自适应声音(带 root)

在根 Pixel 设备上，您可以通过几个简单的步骤来启用自适应声音功能，即使在重新启动设备后，它也会保持启用状态。为此，你首先需要从 APK 镜报下载 Pixel 5 专用版本的设备个性化服务应用程序，并将其安装在你的设备上。是的，你已经安装了设备个性化服务应用程序，但谷歌推送到你手机上的应用程序版本不包括自适应声音功能。因此，你需要使用谷歌为 Pixel 4a、5G 和 Pixel 5 设计的那个。您可以通过点击[此链接](https://www.apkmirror.com/apk/google-inc/device-personalization-services/device-personalization-services-r-9-playstore-pixel5-342894738-release/)下载该版本的应用程序。

安装应用程序后，您需要从 Magisk 管理器应用程序下载并安装 Adaptive _ Audio _ Settings _ Enabler Magisk 模块，然后重新启动您的设备。或者，您可以通过点击[此链接](https://forum.xda-developers.com/attachments/adaptive_audio_settings_enabler-zip.5159569/)下载模块并手动刷新。成功重启后，您应该会在设备设置中看到 Adaptive Sound 选项。

## 在旧的 Pixel 设备上启用自适应声音(无 root)

在非根像素设备上，启用自适应声音的过程有点复杂，因为您必须执行几个 shell 命令。但在这之前，你必须安装 APK 镜报的 Pixel 5 专用版设备个性化服务，并将其安装在你的设备上。关注[此链接](https://www.apkmirror.com/apk/google-inc/device-personalization-services/device-personalization-services-r-9-playstore-pixel5-342894738-release/)即可获得 app。

一旦安装了应用程序，请确保在您的设备上启用了 USB 调试。你可以在开发者选项中点击 USB 调试设置旁边的开关。你还需要确保你的电脑上有一个运行的 ADB 环境(我们在这里有一个教程)。完成后，您需要将手机连接到 PC，并逐一执行以下 3 个命令:

```
 adb shell
device_config put device_personalization_services AdaptiveAudio__enable_adaptive_audio true
device_config put device_personalization_services AdaptiveAudio__show_promo_notification true 
```

执行这三个命令后，您应该会在设备设置中看到自适应声音选项。不过，与根设备的方法不同，这种方法不会永久启用自适应声音选项，一旦重新启动设备，它就会被删除。因此，请确保在完成上述步骤后不要重启设备，否则您将不得不再次重新启动设备。

**[在老像素设备上启用自适应声音 XDA 论坛线程](https://forum.xda-developers.com/t/guide-enable-adaptive-audio-on-pixel-4-xl.4203781/)**