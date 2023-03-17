# 使用 Android 11 的一加 7/7T 系列设备可以启用常亮显示功能，具体操作如下

> 原文：<https://www.xda-developers.com/enable-always-on-display-oneplus-7-7t-android-11/>

长期以来，一直显示一直是几款智能手机的一项功能。具有讽刺意味的是，直到 OxygenOS 11 的[发布，一加设备才真正实现了 AOD。然而，该公司决定不在上周发布的一加 7 和 7T 系列](https://www.xda-developers.com/oneplus-phones-always-on-display-oxygenos-11/)的[首批基于 Android 11 的开放测试版中包含这一受欢迎的功能。根据变更日志，该功能仍在内部测试中，并将在随后的一加 7/7 Pro 和一加 7T/7T Pro 的公开测试更新中发布。](https://www.xda-developers.com/oneplus-7-7-pro-7t-7t-pro-android-11-oxygenos-open-beta-1/)

**[一加七大论坛](https://forum.xda-developers.com/c/oneplus-7.8833/)| |[一加七大论坛](https://forum.xda-developers.com/c/oneplus-7-pro.8847/)|**

**[一加 7T 论坛](https://forum.xda-developers.com/c/oneplus-7t.9249/) ||| [一加 7T Pro 论坛](https://forum.xda-developers.com/c/oneplus-7t-pro.9327/)**

好吧，XDA 的开发者社区再次伸出援手。事实上，OEM 已经在最初的测试版固件中留下了始终显示模式的代码，可以利用它来解锁这些设备上的功能。正如 XDA 公认开发者 [Quinny899](https://forum.xda-developers.com/m/quinny899.3563640/) 所发现的，你所需要做的就是在 root shell 中执行以下命令，强制 OxygenOS 的“OPFeatures”框架启用 AOD。

```
 setprop sys.aod.debug_support_always_on 1 
```

执行该命令并重新加载系统 UI(使用`pkill systemui`)后，启用 AOD 的选项将出现在设置>显示>环境显示>总是在环境显示下。

请记住，前面提到的恢复常亮显示的过程不会在重启后继续存在，但是可以编写一个特殊的 [init](https://en.wikipedia.org/wiki/Init) 脚本来在启动时执行该命令。好消息是，之前创作了 [OPAodMod](https://www.xda-developers.com/opaodmod-customizable-always-on-display-rooted-oneplus-phones/) 的 Quinny899 也发布了一个现成的脚本来做这件事。如果您已经使用 Magisk 对运行 OxygenOS 11 开放测试版的一加 7/7T 进行了根目录设置，您可以遵循本教程:

1.  从这个帖子的第一个帖子[下载附件。](https://forum.xda-developers.com/t/root-magisk-enable-always-on-ambient-display-on-oxygen-os-11-beta-1.4222275/)
    *   请注意，虽然附件是一个 ZIP 文件，但它既不是 Magisk 模块，也不是可恢复的 flash ZIP 文件。
2.  解压缩 ZIP 文件，从中获取名为`aodenable.sh`的脚本。
3.  使用合适的根文件管理器，将脚本复制到`/data/adb/service.d`。
4.  将其权限设置为`rwxr-xr-x` ( `chmod 755`)。
5.  重新启动。
6.  就是这样！

如果你不喜欢手动安装过程，XDA 资深会员 [DanGLES3](https://forum.xda-developers.com/m/dangles3.8714092/) 已经[提出了一个方便的 Magisk 模块](https://forum.xda-developers.com/t/root-magisk-enable-always-on-ambient-display-on-oxygen-os-11-beta-1.4222275/post-84342785)，它做的事情和上面提到的一样。要了解更多细节，请看下面链接的讨论主题。

**[为一加 7 和 7T 系列](https://forum.xda-developers.com/t/root-magisk-enable-always-on-ambient-display-on-oxygen-os-11-beta-1.4222275/)** 启用 Oxygen OS 11 Beta 1 上的持续显示