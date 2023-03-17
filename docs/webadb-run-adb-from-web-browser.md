# WebADB 允许您直接从 web 浏览器运行 ADB

> 原文：<https://www.xda-developers.com/webadb-run-adb-from-web-browser/>

[Android Debug Bridge (adb)](https://www.xda-developers.com/install-adb-windows-macos-linux/) 是一个命令行工具，允许用户与 Android 设备进行通信。使用开发工具，您可以执行许多操作，包括安装和调试应用程序，还可以运行漂亮的 shell 命令。

XDA 论坛成员 [SteelToe](https://forum.xda-developers.com/member.php?u=9050867) 没有在你的电脑上安装 ADB，而是发布了一个新网站([www.webadb.com](https://webadb.com/#/))，允许用户直接从你的网络浏览器执行该工具提供的所有功能。“没有安装，没有驱动程序，什么都没有，”SteelToe 说。“你只需要一个支持 web USB 的 web 浏览器，如 Chrome 或新的微软 Edge，就可以了。”WebUSB API 提供了从网页到 USB 设备的访问，默认情况下在基于 Chromium 的浏览器上是启用的。

Web ADB 的当前功能包括:

*   APK 装置
*   交互式外壳
*   屏幕录制
*   [SCRCPY](https://www.xda-developers.com/scrcpy-control-android-on-pc/) —从浏览器控制您的设备
*   设备信息
*   文件管理器
*   通过 WiFi 启用 ADB

**[WebADB XDA 论坛线程](https://forum.xda-developers.com/android/software/tool-webadb-run-adb-browser-installation-t4195079)| |[GitHub 上的源代码](https://github.com/yume-chan/ya-webadb)**

如果你需要在你的机器上安装 ADB 的帮助，我们有一个的[指南。否则，如果你想要一个不太复杂的体验，你可以使用](https://www.xda-developers.com/install-adb-windows-macos-linux/) [Web ADB](https://webadb.com/#/) 门户。如果你遇到问题，该网站有一些说明，包括如果你得到一个访问被拒绝的错误。

请记住，您仍然需要在智能手机上启用 USB 调试，它位于开发者设置中，通过设置>点击“关于手机”七次即可访问。

ADB 是一个非常通用的命令行工具，尤其是如果你经常使用 Android 智能手机的话。虽然建议将该实用程序安装在您常用的计算机上，但在某些情况下，您可能只需要几个命令。这就是像 Web ADB 这样的工具出现的时候。使用常用的 ADB 命令，您可以安装应用程序、从设备拷贝文件或目录以及将文件或目录拷贝到设备、设置端口转发等等。这些命令本身可能不会完成那么多，但根据您的智能手机 OEM 可能设置的限制，ADB 可以很方便地使用这些命令，以您希望它们在您的设备上出现的方式改变事情。