# 如何在 Windows、macOS 和 Linux 上安装 ADB

> 原文：<https://www.xda-developers.com/adb-fileexplorer-frees-you-from-adb-tedium/>

Android 平台的一些特性只能通过对普通用户隐藏的路径和方法来访问。这些通常是在一些命令行 Android Debug Bridge (ADB)命令的帮助下完成的，这是谷歌为开发人员提供的一个工具，用于调试他们的应用程序或系统的各个部分，但我们可以使用它来实现各种巧妙和隐藏的技巧。这些技巧的先决条件是在您的计算机上安装 ADB。因此，在本指南中，我们将向您展示如何快速、简单地在 Windows、macOS 和 Linux 上安装 ADB。

* * *

## 什么是 Android 调试桥(ADB)？

Android 调试桥(ADB)的内部结构基于经典的客户端-服务器架构。整个过程由三个部分组成。

1.  客户端，即您连接到 Android 设备的 PC 或 Mac。我们通过 USB 电缆或无线方式从计算机向我们的设备发送命令。
2.  在设备上运行命令的守护程序(称为“adbd”)。守护程序在每个设备上作为后台进程运行。
3.  服务器，管理客户端和守护程序之间的通信。服务器在 PC/Mac 上作为后台进程运行。

* * *

## 亚行是如何运作的？

因为 ADB 由三部分组成(客户机、守护程序和服务器)，所以首先需要启动并运行某些部分。因此，如果您刚刚启动了计算机(并且您没有设置在启动时启动守护程序)，那么您将需要它在任何通信可以发送到目标 Android 设备之前运行。您将在命令提示符或终端中看到以下消息，因为它将检查以确保守护程序正在运行。

如果守护进程没有运行，那么它将启动进程，并告诉您它是在哪个本地 TCP 端口上启动的。一旦 ADB 服务启动，它将继续监听 ADB 客户端发送的命令的特定端口。然后，它将建立与所有连接到计算机的运行设备的连接(包括模拟器)。如果电脑过去没有被授权过，这时你会在 Android 设备上收到授权请求。

* * *

## 如何建立亚行

注意:在电脑上设置 ADB 只是等式的一半，因为你还需要在智能手机或平板电脑上做一些事情来接受 ADB 命令。

### 电话设置

1.  启动手机上的**设置**应用程序。
2.  点击列表底部附近的**关于电话**选项。
    *   根据 OEM 皮肤,“关于手机”页面可能会被称为其他名称或隐藏在设备设置中的其他位置。

3.  然后点击**构建号**选项 7 次以启用开发者模式。完成后，您会看到一条祝酒词。
4.  现在回到主设置屏幕，你会看到一个新的**开发者选项**菜单。在谷歌 Pixel 手机和其他一些设备上，你可能需要导航到**设置** > **系统**来找到**开发者选项**菜单。
5.  进入并启用 **USB 调试**选项。
6.  您已经部分完成了电话设置过程。接下来，您需要向下滚动，并按照您的特定操作系统的其余说明进行操作。

按照您计算机上的操作系统进行操作。

* * *

### 如何在 Microsoft Windows 上设置 ADB

1.  [下载适用于 Windows 的 Android SDK 平台工具 ZIP 文件](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)。
2.  将这个 ZIP 文件的内容解压到一个容易访问的文件夹中(比如 C:\platform-tools)
3.  打开 Windows 资源管理器，浏览到解压缩该 ZIP 文件内容的位置
4.  然后从与 ADB 二进制文件相同的目录中打开一个命令提示符。这可以通过按住 Shift 键并右键单击文件夹，然后单击“在此打开命令窗口”选项来完成。Windows 11 用户应该在右键上下文菜单中看到“在终端中打开”，甚至不用按键盘上的 Shift 键。
5.  用 USB 线将智能手机或平板电脑连接到电脑。将 USB 模式更改为“文件传输(MTP)”模式。一些原始设备制造商可能需要也可能不需要，但是为了一般的兼容性，最好保持这种模式。
6.  在命令提示符窗口中，输入以下命令启动 ADB 守护程序:`adb devices`
7.  在手机屏幕上，您应该会看到一个允许或拒绝 USB 调试访问的提示。很自然，当出现提示时，您会希望授予 USB 调试访问权限(如果您不想再看到该提示，请点击 always allow 复选框)。
8.  最后，重新输入步骤 6 中的命令。如果一切顺利，您现在应该会在命令提示符(或 PowerShell 窗口)中看到设备的序列号。

耶！您现在可以在您的设备上运行任何 ADB 命令！现在前进，开始按照我们的教程广泛的列表修改你的手机！

* * *

### 如何在 macOS 上设置 ADB

1.  [下载 macOS 的 Android SDK 平台工具 ZIP 文件](https://dl.google.com/android/repository/platform-tools-latest-darwin.zip)。
2.  将压缩文件解压到一个容易拿到的位置(比如桌面)。
3.  开放终端。
4.  要浏览到您将 ADB 解压缩到的文件夹，请输入以下命令:`cd /path/to/extracted/folder/`
    *   例如，在我的 Mac 上是这样的:`cd /Users/Doug/Desktop/platform-tools/`

5.  使用兼容的 USB 电缆将您的设备连接到 Mac。将 USB 连接模式更改为“文件传输(MTP)”模式。并非每个设备都需要这样做，但最好让它处于这种模式，这样就不会遇到任何问题。
6.  一旦终端位于 ADB 工具所在的文件夹中，您就可以执行以下命令来启动 ADB 守护进程:`./adb devices`
7.  在您的设备上，您会看到“允许 USB 调试”提示。允许连接。
8.  最后，重新输入步骤 7 中的命令。如果一切顺利，您现在应该会在 macOS 的终端窗口中看到您的设备的序列号。

恭喜你！您现在可以在您的设备上运行任何 ADB 命令！现在前进，开始按照我们的教程广泛的列表修改你的手机！

虽然上面的指南肯定会起作用，但一些经验丰富的 macOS 用户应该知道，使用非官方的软件包管理器，如[家酿](https://formulae.brew.sh/cask/android-platform-tools)或 [MacPorts](https://ports.macports.org/port/android-platform-tools/summary) ，可以更容易地在他们的 MAC 上安装 ADB。

* * *

### 如何在 Linux 上设置 ADB

1.  [下载适用于 Linux 的 Android SDK 平台工具 ZIP 文件](https://dl.google.com/android/repository/platform-tools-latest-linux.zip)。
2.  将压缩文件解压到一个容易拿到的位置(比如桌面)。
3.  打开终端窗口。
4.  输入以下命令:`cd /path/to/extracted/folder/`
5.  这将把目录更改为您提取 ADB 文件的位置。
    *   示例:`cd /Users/Doug/Desktop/platform-tools/`

6.  用 USB 线把你的设备连接到你的 Linux 机器上。将连接模式更改为“文件传输(MTP)”模式。这并不总是每个设备都需要的，但是建议这样做，这样你就不会遇到任何问题。
7.  一旦终端位于 ADB 工具所在的文件夹中，您就可以执行以下命令来启动 ADB 守护进程:`./adb devices`
8.  回到您的智能手机或平板设备上，您会看到一个提示，要求您允许 USB 调试。去批准吧。
9.  最后，重新输入步骤 8 中的命令。如果一切顺利，您现在应该会在终端窗口输出中看到设备的序列号。

恭喜你。您现在可以在您的设备上运行任何 ADB 命令！现在前进，开始按照我们的教程广泛的列表修改你的手机！

一些 Linux 用户应该知道，在他们的计算机上安装 ADB 有一种更简单的方法。上面的指南当然对你有用，但是那些拥有基于 Debian/Ubuntu 或 Fedora/SUSE 的 Linux 发行版的用户可以跳过上面指南的步骤 1 和 2，使用下面的命令之一:

然而，选择 Android SDK 平台工具版本的最新二进制文件总是更好，因为特定于发行版的包通常包含过时的版本。

为了涵盖我们在这里的所有基础，用户可能需要在我们在未来教程中列出的 ADB 命令前面加上一个./，特别是当他们直接使用从平台工具 ZIP 中提取的二进制文件时。这可能是任何*nix 用户(或运行 PowerShell 的 Windows 用户)都已经知道的事情，但同样，我们希望尽可能多的人了解如何为 Android 做这些调整，不管你对你的操作系统了解多少。

* * *

### 可选:如何通过 Wi-Fi 使用 ADB

Android 11 及更高版本原生支持通过 Wi-Fi 的 ADB 连接。这消除了处理常见 USB 连接问题和额外步骤的需要，例如在 Windows 上安装 [Android OEM 驱动程序](https://www.xda-developers.com/download-android-usb-drivers/)。

为了设置无线调试，请执行以下操作:

1.  确保您的 PC/Mac 和手机连接到同一个无线网络。
2.  在手机上，进入**设置**下的**开发者选项**，启用**无线调试**。在**上允许在此网络上进行无线调试？**弹出，选择**允许**。[](https://www.xda-developers.com/debloat-your-phone-run-adb-shell-commands-no-root-no-pc/android-11-usb-debugging-and-wireless-debugging/)
3.  点击**无线调试**选项，选择**用配对代码**配对设备。[](https://www.xda-developers.com/debloat-your-phone-run-adb-shell-commands-no-root-no-pc/android-11-wireless-debugging-2/)
4.  记下电话屏幕上显示的配对代码、IP 地址和端口号。[](https://www.xda-developers.com/install-adb-windows-macos-linux/android-wireless-debugging-pair-device-with-pairing-code/)
5.  在您的 PC/Mac 上，运行以下命令:

    ```
     adb pair IP_Address:Port 
    ```

    使用步骤 4 中的 IP 地址和端口号。
6.  出现提示时，输入您在步骤 4 中收到的配对代码。将显示一条消息，提示您的设备已成功配对。
7.  接下来，在 PC/Mac 的终端窗口上运行以下命令:

    ```
     adb connect IP_Address:Port 
    ```

    查看步骤 3 中**无线调试**下的 **IP 地址&端口**部分的 IP 地址和端口。
8.  如果一切正常，那么您应该会看到如下消息:

    ```
     connected to 192.168.68.100:37173 
    ```

9.  现在您已经准备好键入您想要的任何 ADB shell 命令。

* * *

## ADB 命令示例

要检查是否已成功安装 ADB，请使用 USB 电缆将您的设备连接到您的 PC/Mac，并运行上述`adb devices`命令。它应该在命令提示符/PowerShell/终端窗口中显示您的设备。如果您得到不同的输出，我们建议从这些步骤开始。

如上所述，你可以使用 ADB 在 Android 设备上做各种事情。其中一些命令直接内置在 ADB 二进制文件中，应该可以在所有设备上运行。你也可以打开所谓的 ADB Shell，这样你就可以直接在设备上运行命令。直接在设备上运行的命令可能因设备而异(因为 OEM 可以删除对某些设备的访问，还可以修改 adb 行为),并且可能因 Android 版本的不同而不同。

下面是您可以在设备上执行的命令示例列表:

*   打印已连接设备的列表:`adb devices`
*   杀死亚行服务器:`adb kill-server`
*   安装应用程序:`adb install <path_to_the_APK_file>`
*   设置端口转发:`adb forward tcp:6100 tcp:7100`
*   从设备复制文件/目录:`adb pull <path_to_the_remote_object> <path_to_the_local_destination>`
*   将文件/目录复制到设备:`adb push <path_to_the_local_object> <path_to_the_remote_destination>`
*   启动亚行外壳:`adb shell`

### 奖金

对于那些想更进一步的人来说，你可以跟随我们一起制作的这个新教程，它将带你通过[如何设置 ADB，以便你可以从 Windows 或 Linux 桌面上的任何目录使用这个命令](https://www.xda-developers.com/adb-fastboot-any-directory-windows-linux/)。

* * *

## 我还能在亚行做些什么？

以下是各种设备的 XDA 教程列表，详细介绍了 ADB 命令的许多应用，以便修改隐藏设置、自定义 OEM 功能或用户界面，等等！