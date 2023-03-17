# Chrome for desktop 测试 Android 11 风格的一次性位置权限

> 原文：<https://www.xda-developers.com/google-chrome-allow-users-grant-location-access-sites-per-visit-session/>

# Chrome 将很快允许用户在每次访问时访问网站的位置

在 Chrome Canary 的最新版本中，谷歌正在测试一个针对位置权限的改进的每次访问权限模型。看看吧！

Chrome 桌面版将很快让用户更好地控制网站如何访问他们的位置。现在，当一个网站请求访问你的位置时， [Chrome](https://www.xda-developers.com/chrome-89-revamped-profiles-reading-list-more/) 只给你两个选项:允许或阻止。如果允许的话，该网站基本上可以随时访问你的位置信息，甚至在后台，当然，除非你去网站设置，找到那个网站，然后手动撤销访问。许多网站没有明确说明为什么他们首先需要我们的位置。这就是为什么每当一个网站询问位置时，我们的鼠标指针就会跳动，不可避免地停在“屏蔽”按钮上。但值得庆幸的是，谷歌正在让可疑网站更难在后台追踪你的位置。

正如我们可靠的消息来源*[Some _ Random _ Username](https://forum.xda-developers.com/m/some_random_username.8234677/)*所发现的，谷歌 Chrome 正在测试一个改进的位置许可模型，该模型将允许用户在每次会话或单次的基础上提供对网站的位置访问。该功能在 [Chome Canary](https://www.google.com/intl/en_in/chrome/canary/) 91.0.4442.1 中是实时的，并且开箱即用，无需启用任何标志。

当一个网站请求位置时，用户现在会在左上角看到一个弹出窗口，有三个选项，而不是两个:“每次访问”、“只有这一次”和“阻止”选择“每次访问”大概会允许网站只有在前台打开并运行时才能访问你的位置。同时，“只有这一次”应该以 Android 11 的一次性位置和麦克风权限的相同方式工作，仅在单个会话中授予站点位置访问权限。下面是新的权限对话框(右边)与我们在 Chrome stable 89.0.4389.82 中看到的当前对话框(左边)相比的样子。

这确实是一个很大的改进，我们希望看到它尽快进入稳定的 Chrome。我们会密切关注，当它最终到达稳定频道时，我们会让你知道。