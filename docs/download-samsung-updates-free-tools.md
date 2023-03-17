# 这里有 4 个免费工具可以将更新下载到三星 Galaxy 设备上

> 原文：<https://www.xda-developers.com/download-samsung-updates-free-tools/>

如果你曾经试图搜索固件来安装在你的三星 Galaxy 智能手机或平板电脑上，这可能会很烦人。虽然谷歌、一加和小米等公司在其网站上提供下载链接，但三星尚未提供官方固件下载门户。这也是为什么有这么多第三方三星固件下载网站的原因之一。这些网站从三星的 FUS(固件更新服务器)获取最新的固件版本，并按照型号、运营商/地区和操作系统版本对它们进行分类。然而，这些服务中的许多使用“免费增值”模式，这抑制了基础层的下载速度。要想获得更高的带宽或更高级的功能，你必须付费。

幸运的是，并不缺少社区开发的工具来直接下载兼容 Galaxy 设备的新软件更新。我们在过去已经多次讨论过两个这样的工具——SamFirm T1 和 T2 Frija T3。 [Samloader](https://www.xda-developers.com/samloader-download-updates-samsung-galaxy/) 是另一个开源的跨平台选择。虽然我个人认为使用这些实用程序下载三星固件足够简单，但有些人可能仍然觉得它们不足以满足他们的需求。如果你这样做，那么这里有几个解决方案，使你的设备更容易获得官方三星固件包。

## 1.SamFirm _ 重生

SamFirm_Reborn 由 XDA 知名开发者 [Ivan_Meler](https://forum.xda-developers.com/m/ivan_meler.4610599/) 创建，是[原始 SamFirm 工具](https://forum.xda-developers.com/t/tool-samfirm-samsung-firmware-downloader-checker.2988647/)的一个转世。开发人员反编译了遗留应用程序，并修补了代码库，使其与三星的服务器端更改兼容。SamFirm_Reborn 是[开源的](https://github.com/ivanmeler/SamFirm_Reborn)，除了熟悉的 GUI 之外，它还提供了一个方便的命令行界面。

**[下载 SamFirm _ 重生](https://github.com/ivanmeler/SamFirm_Reborn/releases)**

SamFirm-continued 作为遗留 SamFirm 的另一个开源分支开始了它的旅程，但是维护者在几个月前放弃了这个项目。后来，XDA 成员[东塔](https://forum.xda-developers.com/m/tungtata.8243977/)接过接力棒，创建了 SamFwTool。SamFwTool 的一个亮点是自动检测功能。只需在 MTP 模式下连接您的手机，然后按“自动检测”来识别您的设备型号和地区代码。

**[下载 SamFwTool](https://forum.xda-developers.com/t/tool-samfwtool-check-and-download-newest-samsung-firmwares-new-functions.4187119/)**

## 3.SamFirm.js

整个三星固件下载传奇现在处于一个不同的水平，因为 XDA 认可的开发商 [jesec](https://forum.xda-developers.com/m/jesec.6371894/) 已经推出了 SamFirm.js，一个用 JavaScript 编写的流媒体下载器、解密器和提取器。使用 SamFirm.js 作为后端，您应该能够构建一个 web 应用程序来获取库存的 Samsung 固件包。[这个项目](https://github.com/jesec/samfirm.js)是开发商 jesec 和 [LuK1337](https://forum.xda-developers.com/m/luk1337.5075128/) 的合作。

**[下载 samfirm . js](https://github.com/jesec/samfirm.js/releases)**

## 4.SamFetch

如果您正在寻找 Samloader 项目的 web API 变体，您应该尝试一下 SamFetch。XDA 成员 [YusufCihan](https://forum.xda-developers.com/m/yusufcihan.7161164/) 将 Samloader 代码中的功能重新实现为 web routes，以公开一个简化的 REST API 来下载三星固件。

**[下载 SamFetch](https://github.com/ysfchn/SamFetch)**

* * *

你尝试过以上任何一个或类似的项目吗？请在下面的评论中告诉我们！