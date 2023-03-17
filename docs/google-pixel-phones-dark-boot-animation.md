# Pixel 手机很快就会一直显示黑暗开机动画

> 原文：<https://www.xda-developers.com/google-pixel-phones-dark-boot-animation/>

# Pixel 手机将很快总是显示黑暗启动动画，不管主题是什么

无论系统主题如何，谷歌 Pixel 手机都会显示黑暗启动动画，以减少夜间干扰。

Android 的启动动画由手机启动时循环播放的一系列图像组成，这是 OEM(和高级用户)定制最简单的事情之一。在 Android 10 出现之前，Pixel 手机的开机屏幕有一个炫目的白色背景。在 Android 10 中，谷歌[终于添加了](https://www.xda-developers.com/android-q-beta-5-dark-boot-animation/)一个黑暗主题的引导选项，每当系统主题设置为黑暗模式时都会使用。谷歌现在正准备将这种暗启动动画作为唯一选项，而不考虑用户定义的系统主题。

提交到平台/硬件/谷歌/pixel 分支中的 Android 开源项目(AOSP)库的一个新的[提交](https://android-review.googlesource.com/c/platform/hardware/google/pixel/+/1612364)调整了 pixel 手机的公共 init 文件中的几行代码。以前，代码检查 persist.sys.theme 属性的值，以确定何时应用暗启动标志。现在，代码只是检查设备是否已被供应(即已完成首次设置过程。)根据提交描述，这一变化是 Pixel UI 团队决定“在设备配置后始终使用黑暗启动”的结果...因此，用户在晚上进行定期更新时，受到的干扰会更少。”

一旦该提交被合并，并且包含该代码变更的更新被推出到 Pixel 手机，那么用户将不再能够改变引导动画的主题。相反，它将永远是一个黑暗的启动动画。就个人而言，我认为这是一个好的改变，但我知道有些人不喜欢黑暗主题。

*感谢 XDA 公认的开发者 [luca020400](https://forum.xda-developers.com/m/luca020400.5778309/) 的提示！*