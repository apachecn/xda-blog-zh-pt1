# 如何用 Googlefier 在华为设备上轻松安装 Google apps

> 原文：<https://www.xda-developers.com/project-tango-play-store/>

美国政府对华为实施的谷歌禁令导致这家中国科技巨头一度蓬勃发展的手机业务跌落悬崖，因为尽管华为的智能手机硬件可能很棒，但无法访问 YouTube 和 Google Drive 等核心谷歌移动服务应用程序使得 mainland China 以外的许多人很难使用手机软件。

但仍有一些发烧友对拥有一部华为手机感兴趣。例如，只要看看 XDA 的[论坛](https://forum.xda-developers.com/f/huawei-mate-x2.12103/)，就有人有兴趣支付 3000 多美元来进口一台华为 Mate X2。

虽然有几种方法可以在华为设备上安装 GMS，但迄今为止公布的所有方法对于普通用户来说都太复杂，因此成功率各不相同。这就是 Googlefier 应用的用武之地。

Googlefier 本质上是一个来自 XDA 资深成员 [bender_007](https://forum.xda-developers.com/member.php?u=3279781) 的非官方 GMS 安装程序，之前因其在 LG 手机 AutoRec 项目中的工作而闻名。它提供了在您的华为设备上安装 GMS 和 Google apps 的简单分步说明，无需将设备连接到 PC——前提是设备运行 EMUI 10。

不过，华为最近向其设备推送了 EMUI 11 更新，所以如果你的华为设备已经更新，你必须回滚到 EMUI 10，才能使用 Googlefier。您将需要一台 Windows PC 来进行回滚，但该过程本身并不复杂。我们将在接下来的几段中指导您。

如果您的华为设备仍在运行 EMUI 10，那么只需从下面链接的论坛线程下载 APK，并将其安装在您的华为设备上。安装完成后，授予该应用程序所有必需的权限，然后按照概述的步骤在您的手机上安装 GMS。

## 从 EMUI 11 回滚到 EMUI 10

你需要做的第一件事是 ***备份你的手机*** 因为回滚到 EMUI 10 会把里面的东西都抹掉。一旦你做到这一点，按照以下步骤。另请注意，这种方法不适用于华为 Mate X2，其软件无法回滚。

*   从华为网站下载适用于 Windows PC 的华为 HiSuite 软件。(尽管在 Mac 上可以使用 HiSuite，但这个版本不允许软件回滚)
*   允许通过 HDB 进行 USB 连接，为此，请前往设置>安全>更多设置>然后打开 HDB 切换
*   通过 USB 电缆将您的华为设备连接到您的计算机
*   选择“传输文件”
*   批准所请求的权限
*   HiSuite 将要求您输入验证码以确认同步，在您插入手机后不久，验证码将显示在您的华为设备的屏幕上
*   在 HiSuite 主屏幕上，点击“更新”按钮
*   然后点击“切换到其他版本”按钮
*   点击“恢复”
*   点击“回滚”
*   根据您的互联网连接和一天中的时间，回滚过程可能需要 20 分钟到 45 分钟不等。一旦完成，你的华为设备将重启，一旦重启，你将回到 EMUI 10

## 在 EMUI 10 中使用 Googlefier

在安装过程中，Googlefier 会先替换你现有的备份 app，恢复 LZPlay，这是 Mate 30 推出后广为流传的 GMS 安装 app/方法。完成后，Googlefier 会在你的设备上安装基本服务。为此，您需要遵循屏幕上显示的说明。完成所有五个步骤后，您就可以在设备上安装谷歌 Play 商店和其他谷歌应用程序，然后登录您的谷歌帐户。整个过程需要大约 5-7 分钟，如果你按照指示正确，你应该不会得到任何错误。

**[从 XDA 论坛](https://forum.xda-developers.com/android/apps-games/googlefier-install-gms-huawei-honor-t4180485)下载 Googlefier】**

我们在运行 EMUI 10 的[华为 P40 Pro](https://forum.xda-developers.com/huawei-p40-pro) 和[华为 MatePad Pro](https://forum.xda-developers.com/huawei-matepad-pro) 上测试了 Googlefier。下面嵌入的视频显示了在我们的一台 XDA P40 Pro 上的安装过程。

如果你已经尝试用不同的方法在你的设备上安装谷歌应用程序，我们建议你重置设备，用谷歌浏览器重新启动。这将确保您在安装过程中不会遇到任何错误。值得注意的是，该应用程序还包括一个功能，可以让你轻松撤销所有这些更改，并将你的华为设备恢复到 GMS 前的状态。