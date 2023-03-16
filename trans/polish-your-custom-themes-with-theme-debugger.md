# Android 12 会自动从你的壁纸中为你的 UX 添加主题

> 原文：<https://www.xda-developers.com/polish-your-custom-themes-with-theme-debugger/>

Android 12 已经从开发者预览阶段毕业， [Android 12 Beta](https://www.xda-developers.com/android-12-beta-1-google-io-2021/) 激活了许多隐藏在之前版本中的功能。这些以前被禁用的功能包括隐私指示器、改进的小工具、快速设置的彻底改革的设计等。最新版本还带来了自 Android 9 Pie 以来的首次重大设计变革，由新的[材料 You](https://www.xda-developers.com/material-you/) 设计语言提供动力。这种新的设计理念最令人兴奋的一个特点是，它是自适应的，并优化了用户界面中的颜色，以匹配您的壁纸。

谷歌坚持认为，Android 12 旨在让你的体验变得私密和“非常个性化”。根据这一议程，Android 12 现在会根据手机当前壁纸中使用的颜色，在系统 UI 中自动选择一组相关的调色板。这个功能在内部被称为“莫奈”，可以被视为 RRO 和 OMS API 的演变，这些 API 已经在 Android 中使用了几年，并在谷歌的“像素主题”应用程序中得到初步利用。

根据谷歌 I/O 2021 的主题演讲，颜色将统一应用于锁屏、快速设置、通知面板等元素，甚至是新添加的[自适应小工具](https://www.xda-developers.com/google-android-12-widgets-overhaul/)。

谷歌对该功能的说明很有前途，但遗憾的是，它在 Android 12 测试版中不容易获得。因在 ProtonAOSP ROM 和 ProtonKernel for Pixel 设备上的工作而获得认可的开发人员 [kdrag0n](https://forum.xda-developers.com/m/kdrag0n.7291478/) ，已经设法让它在 Android 12 DP1 上工作。当时，他们告诉我们，该功能通过基于颜色相似性动态应用 RRO 覆盖的*来工作。*“他们也有最新测试版的功能演示。

自从几个月前我们第一次观察以来，这个系统已经有了改进。今天，谷歌表示，颜色提取系统使用一种带有材料颜色目标的聚类算法来确定主色和次主色，然后应用与你的壁纸匹配的色调。丰富的 5 种颜色(2 种中性色和 3 种强调色)和 12 种材料色可用于确定与用户壁纸最接近的色调。然后应用程序可以从索引中抓取 Android 的系统颜色到调色板中，并以许多不同的微妙方式使用它。小工具甚至可以使用颜色提取功能来与用户在主屏幕上的主题相协调。

我们预计该功能将在 Pixel 手机上首次亮相后，在未来的公开 Android 12 版本中推出，我们非常兴奋能够亲自尝试。

**查看我们所有的[谷歌 I/O 报道](https://www.xda-developers.com/tag/google-io-2021/)！**