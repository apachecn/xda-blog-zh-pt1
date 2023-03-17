# 谷歌将 WireGuard VPN 添加到 Android 12 的 Linux 内核中

> 原文：<https://www.xda-developers.com/google-adds-wireguard-vpn-android-12-linux-kernel-5-4/>

**更新 1(10/26/2020 @ 06:11PM ET):**Android 的 Linux 内核 4.19 树中也加入了对 WireGuard VPN 协议的原生内核支持。滚动到底部了解更多信息。下面保留了 2020 年 10 月 13 日发表的文章。

由于新冠肺炎的出现，远程工作成为许多企业的常态，用虚拟专用网络(VPN)保护网络连接比以往任何时候都更重要。服务可以使用多种 VPN 隧道协议，但是一种相对较新的叫做 *WireGuard* 的实现已经在技术世界掀起了风暴。正如我们之前解释的那样，WireGuard 是下一代 [VPN 协议](https://www.xda-developers.com/wireguard-vpn-project-support-android-roms/)，它采用了现代加密标准，并具有安全、可审计的代码库。在包含在 [Linux 内核 5.6](https://www.xda-developers.com/wireguard-vpn-linux-kernel-5-6/) 之后，谷歌现在正在将对该协议的支持添加到 [Android 12](https://www.xda-developers.com/android-12/) 的 Linux 内核 5.4 树中。

谷歌派生出每个 Linux 内核版本，以包括“Android 社区感兴趣的补丁，这些补丁还没有被合并到主流或长期支持的(LTS)内核中。”这些内核被称为 [Android 通用内核](https://source.android.com/devices/architecture/kernel/android-common)，它们构成了今天市场上每一个 Android 设备上搭载的 Linux 内核版本的基础。对于每一个 Android 版本，谷歌都支持少数 Linux 内核版本；对于 Android 11，目前是 Linux 内核版本 4.14 和 4.19，而对于 Android 12，[将是版本 4.19](https://android-review.googlesource.com/c/platform/hardware/interfaces/+/1431736/2#message-148e57dbe35431e1534e2f90f67c4e87c1b26f15) 和 5.4。

今天典型的旗舰 Android 设备[运行在 Linux 内核 4.19](https://source.android.com/devices/architecture/kernel/android-common) 的分支之上，但一旦高通和其他 SoC 供应商的新芯片搭载在下一代 Android 设备上，这种情况有望改变。这些即将推出的设备中有许多将在 2021 年底在 Linux 内核 5.4 的基础上运行下一版本的 Android-Android 12，这些设备可能是第一批在 Android 上原生支持 WireGuard VPN 的设备。

今天早些时候，我们发现了一系列[对安卓通用内核](https://android-review.googlesource.com/q/I2e8819aff9c76fbcf4da749292bfc486556f7382)[安卓 12-5.4 树](https://android.googlesource.com/kernel/common/+log/refs/heads/android12-5.4)的新提交。在这些新的提交中有 [WireGuard VPN 协议本身](https://android.googlesource.com/kernel/common/+/0933807d35a8ce84f16e5bfef17a35e7791efb60)，以及[一个在 Android 内核](https://android.googlesource.com/kernel/common/+/a5d10f0defc377d43672b304e31e37a517fbf0bf)上实现这一点的配置选项。这是由经验丰富的稳定内核开发人员 Greg KH 添加的，他将这一变化描述为“为 sane VPN 添加本机内核支持”

然而，在用户能够在 Android 12 上使用 WireGuard 协议本地启用 VPN 之前，谷歌需要添加 API 来与内核模块接口。人们可能会认为这正是谷歌接下来要做的，我们将密切关注 AOSP，跟踪明年 Android 版本中 WireGuard 支持的进展。

感兴趣的 Pixel 用户现在可以通过启动他们的设备并安装预建的内核模块来利用这种内核加速。在其他设备上，您可以刷新一个自定义内核，该内核在 XDA 论坛上宣传 WireGuard 支持。对于没有 root 用户的用户来说，WireGuard 应用程序仍然工作得很好，仍然是最快的 VPN。要了解更多信息，请在您的安卓智能手机[或安卓电视设备](https://www.xda-developers.com/wireguard-project-announces-big-android-update-android-tv-support-more-modern-code-api-third-party-apps/)上从 Google Play 下载 [WireGuard 应用程序。如果你有兴趣参与这个项目，你可以联系 WireGuard 开发团队——他们正在积极寻找新的 Android 应用维护者。](https://play.google.com/store/apps/details?id=com.wireguard.android)

## 更新 1:在 Android-4.19-稳定树中启用

Android 12 支持的所有 Linux 内核版本都将支持 WireGuard VPN。在合并到 android12-5.4 通用内核树之后，对 WireGuard 的本机内核支持已经被添加到 android-4.19 稳定树中。这意味着 WireGuard 的内核加速将在装有 Linux 内核 4.19 和 5.4 的设备上的 Android 12 中得到支持，尽管谷歌是否会在 Android 12 的稳定发布前及时添加 API 以与内核模块接口仍有待观察。