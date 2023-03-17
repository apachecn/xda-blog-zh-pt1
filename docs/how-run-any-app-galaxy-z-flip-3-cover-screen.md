# 以下是如何在 Galaxy Z Flip 3 的封面上运行任何应用程序

> 原文：<https://www.xda-developers.com/how-run-any-app-galaxy-z-flip-3-cover-screen/>

三星的新 [Galaxy Z Flip 3](https://www.xda-developers.com/samsung-galaxy-z-flip-3/) 比以前的 Galaxy Z Flip 型号进步了一大步。这款设备不仅比其前辈更耐用，而且还配备了更好的 SoC、120Hz 高刷新率显示屏和更大的覆盖显示屏。为了更好地利用外部显示屏，三星还在设备上打包了一些额外的软件功能，让你甚至不用打开手机就可以做各种事情。

[**三星 Galaxy Z Flip 3 评测:太好了，我买了两个**](https://www.xda-developers.com/samsung-galaxy-z-flip-3-review/)

然而，尽管 Galaxy Z Flip 3 的外部显示屏比旧款机型好得多，但它仍有一些局限性。例如，三星只为封面显示屏提供了一小部分小工具，让你控制音乐播放，访问三星健康数据，查看天气信息，阅读通知，并将其用作取景器。该公司不让你在封面屏幕上访问所有已安装的应用程序，这绝对是一个败笔。令人欣慰的是，我们的 [Galaxy Z Flip 3 论坛](https://forum.xda-developers.com/f/samsung-galaxy-z-flip-3.12351/)上的开发者已经提出了解决办法。

## 如何在 Galaxy Z Flip 3 的封面屏幕上运行任何应用程序

XDA 成员[卡鲁迪布](https://forum.xda-developers.com/m/carudibu.11784289/)已经[发现了一个有用的漏洞](https://forum.xda-developers.com/t/app-subui-browser-browse-the-web-on-the-cover-screen.4325963/)，可以让你在 Galaxy Z Flip 3 的封面上加载一个定制的小工具。这个漏洞本质上是让你在封面上打开一个基于 GeckoView 的浏览器，让你浏览网页，它还让你添加定制的小部件。这个漏洞最大的好处是它不需要根用户访问。XDA 公认的开发者 [twistedumbrella](https://forum.xda-developers.com/m/twistedumbrella.593514/) 已经发布了一个基于这个漏洞的 WIP 启动器，可以让你在封面上运行任何已安装的应用。

你可以在 Galaxy Z Flip 3 上尝试基于 GeckoView 的浏览器，方法是遵循 GitHub 页面上[给出的说明。请注意，在开始安装过程之前，您需要卸载 Samsung Health。同样值得注意的是，由于目前这只是一个概念验证，您可能会遇到一些问题。CarudiBu 的帖子指出，虽然你可以使用定制的小工具，并利用漏洞在封面屏幕上浏览网页，但你不能访问屏幕键盘或保存当前会话。](https://github.com/CarudiBu/SubUI-browser/releases/)

至于自定义封面屏幕启动器，你可以从这个 GitHub 页面下载它的 APK 并安装在你的设备上。因为它也是一个早期版本，所以有一些限制。当前状态下的封面屏幕启动器要求您将屏幕锁定类型设置为无。它也不提供屏幕键盘支持。此外，在封面屏幕上切换应用程序需要你点击电源按钮来关闭小工具，然后用不同的应用程序重新启动它。但你可以用滑动手势关闭应用列表。