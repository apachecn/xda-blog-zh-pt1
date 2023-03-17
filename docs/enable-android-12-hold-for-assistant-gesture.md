# 在旧版本的 Android 12 上启用“等待助手”手势

> 原文：<https://www.xda-developers.com/enable-android-12-hold-for-assistant-gesture/>

谷歌的大型(虚拟)I/O 开发者大会上周举行，在展会上，我们得到了山景城公司正在开发的所有新服务和功能的预告片。对我们来说，最激动人心的消息是 [Android 12](https://www.xda-developers.com/android-12/) 的大发布，尽管第一个测试版[缺少了很多承诺的功能](https://www.xda-developers.com/android-12-beta-1-hands-on/)，但它仍然有很多值得我们仔细研究的地方。Beta 1 中的一个新功能是一个名为“等待助手”的手势，但事实证明，这个手势本身对 Android 来说并不陌生。事实上，早在 Android 10 的代码库中就有启用它的方法，我们将向您展示如何启用它。

在 Android 12 Beta 1 中，你会发现新的“等待助手”手势隐藏在设置>系统>手势>电源菜单下。启用时，该功能允许用户“通过按住电源按钮来触发助手”根据你的设备，类似的手势可能已经存在，但启用该功能的设置至少对 Pixel 手机来说是新的。

*左:按住一加 9 上 OxygenOS 11 中的电源按钮设置。右图:谷歌 Pixel 5 上 Android 12 Beta 1 中的电源菜单设置。*

使用简单的 ADB shell 命令，可以改变 Android 10 和 Android 11 上长按电源按钮手势的行为，以模仿 Android 12 的“等待助手”手势。这是可能的，因为谷歌在 Android 中添加了代码，允许长按电源按钮功能在运行时调整。这种代码变化是在 2019 年合并到 Android 中的[，并且存在于 Android 10 中，正如我在我的~~专用 Google Photos 上传机器~~ Google Pixel XL 上确认的那样。你所需要做的就是修改`Settings.Global.power_button_long_press`和`Settings.Global.power_button_very_long_press`的值，这两个设置值分别覆盖了框架定义的值`config_longPressOnPowerBehavior`和`config_veryLongPressOnPowerBehavior`。“`power_button_long_press`和“`power_button_very_long_press`的可能值在 AOSP 的](https://cs.android.com/android/_/android/platform/frameworks/base/+/b458f4eee871292dcd94892cc0700fd7998fc279) [PhoneWindowManager](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/services/core/java/com/android/server/policy/PhoneWindowManager.java) 类下定义。但是，您不需要仔细阅读这些页面，因为我将演示如何更改这些值以及可以将它们更改为什么。

## 在 Android 10-11 上启用 Android 12 的“等待助手”手势

**这种方法可能并不适用于所有运行 Android 10 或 Android 11 的设备。虽然我们知道它可以在 Pixel 手机上工作，但我们不知道 OEM 厂商对 Android 的改变是否阻止了这种方法。您的里程可能会有所不同！**

1.  在你的 PC 上安装并设置[ADB](https://www.xda-developers.com/install-adb-windows-macos-linux/)或者在你的手机上安装并设置[LADB](https://www.xda-developers.com/debloat-your-phone-run-adb-shell-commands-no-root-no-pc/)(仅限 Android 11)。这两种方式都可行，因为我们只需要访问 Android 的 shell 界面，并拥有足够的权限来修改设置表。(这意味着像 Play Store 下的“素材终端”这样的应用将无法工作，除非[你有 root 权限](https://www.xda-developers.com/root/)。)
2.  在 shell 中运行以下命令来更改长按电源按钮的行为:

    ```
     adb shell settings put global power_button_long_press X 
    ```

    其中“X”是下列之一:
    *   “0”表示“什么都不做”(即。长按电源按钮不起任何作用)
    *   “1”代表“全球行动”(即显示正常电源菜单)
    *   “2”代表“关闭”(即关闭电话电源)
    *   “3”表示“关闭无确认”(即立即关闭电话电源)
    *   “4”表示“转到语音助手”(启动带有自上而下对话框和“搜索歌曲”按钮的旧助手 UI)
    *   “5”代表“助理”(即。启动默认助手服务，如“设置”下的“默认应用程序”中所定义)
3.  在 shell 中运行以下命令来改变*非常* (3.5s)长按电源按钮的行为:

    ```
     adb shell settings put global power_button_very_long_press X 
    ```

    其中“X”是下列之一:
    *   “0”表示“什么都不做”(即。很长时间-按下电源按钮不起作用)
    *   “1”代表“全球行动”(即显示正常电源菜单)
4.  为了不把自己锁在电源菜单之外(有趣的是，目前在 Android 12 Beta 1 中，当你启用“等待助手”时就是这种情况！)，我建议用下面的值运行上面的两个命令:

    ```
     adb shell settings put global power_button_long_press 5 
    ```

    ```
     adb shell settings put global power_button_long_press 1 
    ```

    这将让你长按电源按钮 0.5s 来启动谷歌助手(或任何其他你设置为默认的助手应用程序)，同时让你长按电源按钮 3.5s 来访问电源菜单。
5.  要恢复到默认行为，只需将“`power_button_long_press`”更改为 1，将“`power_button_very_long_press`”更改为 0，或者运行以下命令:

    ```
     adb shell settings delete global power_button_long_press 
    ```

    ```
     adb shell settings delete global power_button_long_press 
    ```

如果你想知道，改变这些值不会影响*非常，非常，非常*长按电源按钮的行为(即。强制重启电话)，这是用户不能禁用的安全特征。

* * *

正如我们最近发现的，谷歌应用程序正准备[为“等待助手”手势添加自己的支持](https://www.xda-developers.com/google-app-launch-google-assistant-power-button/)。该功能目前尚不可用，但最新版本的谷歌应用[增加了](https://twitter.com/MishaalRahman/status/1395537577051054081)一个“用电源按钮与谷歌对话”屏幕，通知用户他们可以长按电源按钮来访问谷歌助手。有趣的是，这个屏幕还告诉用户，他们可以通过告诉 Assistant“关机”来关闭手机，这是 Assistant 目前不支持的功能。

我们不知道谷歌应用程序将如何实现这一功能——它是否仅限于 Android 12，或者谷歌是否会使用上面提到的内置功能在 Android 10 和 Android 11 上启用它。谷歌应用程序目前缺少完成上述操作所需的必要权限，也缺少触发设备关机或重启所需的权限。我们可能不得不等待新版谷歌应用的出现，但与其等待，不如现在就运行本文中的 ADB 命令来获得 Android 12 的“等待助手”手势！