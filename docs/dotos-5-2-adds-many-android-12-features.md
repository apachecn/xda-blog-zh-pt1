# DotOS 5.2 发布了类似 Android 12 的动态主题化系统

> 原文：<https://www.xda-developers.com/dotos-5-2-adds-many-android-12-features/>

# DotOS 5.2 增加了受 Android 12 启发的新功能，包括基于壁纸的主题化等

期待已久的 DotOS 5.2 版本终于发布了，它带来了许多受 Android 12 启发的功能。请继续阅读。

上个月，DotOS 定制 ROM 项目[的开发者为他们即将发布的版本设计了一个新的基于 Android 12 的动态主题引擎](https://www.xda-developers.com/dotos-new-android-12-based-dynamic-theming/)。期待已久的[新版本](https://blog.droidontime.com/blog/september-release-2021)——DotOS 5.2——终于来了，除了字幕系统范围的主题化系统，它还带来了几个新功能和变化，包括重新设计的设置仪表板，新的游戏模式，新的电池管理器应用程序，新的时钟小部件等等。

DotOS 5.2 最大的亮点当然是 MonteWannabe 2.2 主题化系统，其灵感来自 Android 12 代号为“monet”的新主题化引擎。新的主题引擎基于 [kdrag0n 强大的基于 zcam 的颜色生成引擎](https://www.xda-developers.com/android-12-material-you-theming-system-recreated/)和 [Quinny899](https://forum.xda-developers.com/m/quinny899.3563640/) 的 MonetCompact 支持库，现在能够将动态主题应用于比以前版本更多的系统 UI 部分。

接下来，DotOS 5.2 将加入一个受 Android 12 游戏面板启发的专用游戏模式。启用后，游戏模式会屏蔽通知，并提供游戏内截图和启动屏幕录制的控件。

最新版本还添加了一个基于 [Buoy](https://github.com/tytydraco/Buoy) 的新电池管理器应用，并提供了几种电池配置文件，以最大限度地延长电池寿命。

最后，DotOS 5.2 增加了新的 [Android 12 风格的时钟小工具](https://www.xda-developers.com/android-12-beta-5-changelog/)以及改进的设置页面。

DotOS 5.2 版本现已面向官方支持的设备推出。要查看您的设备是否受支持，请查看 [DotOS 下载页面](https://droidontime.com/devices)。

DotOS 5.2 版的完整变更日志如下:

### DotOS 5.2 changelog

*   九月安全补丁(Android11 r45)
*   固定系统界面崩溃时，设备在景观。
*   移除了彩色状态栏图标功能
*   添加了新的 APN。
*   修正了 OTA 不兼容问题
*   crowdin 的最新翻译
*   UI/UX 改进
*   稳定性和发动机舱盖下的改进
*   提高了 Oneplus 设备的亮度

#### MonetWannabe 2.2

*   基于最新的 kdrag0n 的 ZCAM 实现的主题引擎(更好的颜色生成方式)
*   增加了壁纸颜色选择器支持
*   增加了主题色彩控制
*   增加了主题亮度控制
*   增加了主屏和锁屏壁纸的独立调色板
*   增加了对全球 Monet 支持的支持(自定义，设置，系统界面，核心元素等)
*   清除代码
*   将颜色生成移至 SystemUI 线程

#### 改进的定制应用程序

*   几乎完全重新设计，以确保一个更好的 UX
*   实施壁纸计划
*   增加了 Monet 支持

#### 增加了“游戏面板”

*   实现了游戏模式，但有更好的用户界面和 UX
*   实现了一个早期版本的“快速控制”——一个在你玩游戏时可以方便控制的浮动药丸

#### 增加了电池管理器

*   最初基于 Buoy——一款电池节电模式定制应用
*   把所有和电池有关的东西都搬到这里了
*   增加了省电模式
*   增加了电池节电模式定制
*   添加智能充电
*   增加了智能截止

#### 设置

*   添加了隐私仪表板
*   增加了 Monet 支持
*   重新设计的黑暗模式预览
*   重新设计的仪表板图标
*   设备卡略有改进
*   修正了设置中某些部分的滚动问题

#### 系统

*   增加了低分辨率屏幕录制选项
*   添加了部分截图
*   添加了指南针快速设置磁贴
*   添加了重启、恢复、关机快速设置磁贴
*   修复了在 QSPanel 中使用“数据使用”选项时的延迟
*   移除了 QSPanel 中的拖拽药丸
*   已实施 A12 Beta 4 媒体控制面板
*   增加了 monet 对通知和 qs 按钮的支持
*   改进了折叠 QSPanel 和定制器(添加/删除/移动图块菜单)中的空间
*   实施了 12 针/型号锁屏安全设计(+monet 支持)
*   实施新的 A12，如默认锁屏时钟
*   基于 FOD 实现更好的稳定性
*   支持 monet 的重新设计的音量面板
*   重新设计的支持莫奈的快速面板

#### 系统更新

*   增加了 monet 支持
*   增加了设备变更日志支持

#### 权限对话框

*   略有改进的设计
*   增加了 monet 支持

#### AOSP 计算器

*   重新设计并增加了 monet 支持