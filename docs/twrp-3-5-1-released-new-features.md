# 随着团队为 Android 11 做准备，TWRP 3.5.1 发布了新功能

> 原文：<https://www.xda-developers.com/twrp-3-5-1-released-new-features/>

# 随着团队为 Android 11 支持做准备，TWRP 3.5.1 发布了新功能

TWRP 3.5.1 推出了受支持的设备，进行了大量的底层改进和错误修复。看看吧！

TWRP 或团队胜利恢复项目是一个非常熟悉的名字在 Android 的修改者。对于不知情的人来说，这是一个定制的恢复解决方案，为许多激动人心的机会打开了大门。基本上，它取代了手机自带的默认恢复，因此你可以刷新自定义的 rom 和内核，通过 Magisk 启动你的设备，等等。Android 修改者信赖 TWRP 的原因之一是它积极开发和支持各种各样的手机，新手机定期被添加到项目中。在 12 月下旬，recovery 收到了一个大更新，即 [TWRP 3.5.0](https://www.xda-developers.com/twrp-3-5-0-released-android-10-support/) ，它对解密、错误修复以及对 Android 10 开箱即用设备的支持进行了许多改进。当时，该团队表示，Android 11 版本的工作已经在进行中。现在，在期待已久的 Android 11 发布之前，该团队推出了一个迷你版 TWRP 3.5.1。

TWRP。[增加了对在刷新图像时刷新两个插槽的支持](https://twrp.me/site/update/2021/03/17/twrp-3.5.1-released.html)，对新的[可刷新 Magisk APK](https://www.xda-developers.com/install-magisk-manager-without-separate-zip/) 的支持，Bash 支持，以及许多其他的改进和修正。

TWRP 3.5.1 的完整变更日志如下:

### twp 3 . 5 . 1 变更日志

*   Android 9 分支:
    *   在 7.1 树中编译- CaptainThrowback
    *   SAR:不要跟踪块设备的符号链接
    *   clarity 的 SAR 更新脚本名称- CaptainThrowback
*   Android 9 和 Android 10 分支:
*   *   Wrappedkey 支持仅在 FBE 设备上运行- CaptainThrowback
    *   TWRP 应用程序日志信息减少- epicX67
    *   系统擦除和 adb 侧载后刷新详细信息- AdrianDC
    *   中文翻译更新- betaxb
    *   支持 keymaster 2 - PeterCxy
    *   将 tzdata 添加到 TWRP 时区- CaptainThrowback
    *   partitionmanager:支持延迟采用的存储装载- petercxy
    *   支持从文件管理器目录启动终端
    *   纳米载体- nebrassy
    *   添加 nano 支持从文件管理器打开文件
    *   包括将由 TWRP - ianmacd 安装的新 magisk apk 支持
    *   添加对更改 TWRP 存储备份的目录名的支持- epicX67
    *   添加 bash 支持——不是默认的 shell——darthjabba 9
    *   ORS 支持格式化数据- AdrianDC
    *   添加了在刷新映像时刷新两个插槽的支持- epicX67
    *   NL 翻译更新- ianmacd
    *   安装清理-删除重复包 ExtractFn - klabit87
    *   删除 logd-reinit 服务- CaptainThrowback
    *   还原系统根上下文- bigbiff
    *   如果树支持 keymaster 2，则只包括它- CaptainThrowback
    *   language_helper.py - ianmacd 中包含'-'的条带行
    *   未本地化的字符串 fix - ianmacd

TWRP 3.5.1 版本适用于大多数当前支持的设备。要为您的设备下载最新版本，请通过下面的链接访问 TWRP 官方网站。或者，您也可以使用谷歌 Play 商店上的 TWRP 官方应用程序直接从您的设备上获取新版本。

**[为您的设备下载 TWRP](https://twrp.me/Devices/)**