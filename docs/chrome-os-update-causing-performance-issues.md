# 最新的 Chrome 操作系统更新给许多用户带来了性能问题

> 原文：<https://www.xda-developers.com/chrome-os-update-causing-performance-issues/>

上周，谷歌在稳定频道上发布了新的 Chrome OS 更新。由于这是一个稳定的版本，大多数用户不会想到会遇到严重的错误和性能问题。但不幸的是，这正是许多安装了这个特定更新的用户所遇到的情况。

事实证明，最新的稳定更新 Chrome OS 版本 91.0.4472.147 毕竟不是那么稳定。许多 Chromebook 的所有者[报告称](https://www.reddit.com/r/chromeos/comments/ocv8dn/issues_after_update_9104472147/)(via[*Android Police*](https://www.androidpolice.com/2021/07/05/you-might-not-want-to-update-your-chromebook-to-the-latest-chrome-os-release-just-yet/))在安装最新的 Chrome OS 更新后性能严重下降。我们这里并不是在讨论在 Chrome 浏览器中打开多个标签或者在应用程序之间切换。根据不同用户的报告，即使是做一些基本的事情，比如打字、在用户界面上导航、打开应用程序，似乎也会让电脑陷入停顿。执行常见的故障诊断步骤，如禁用所有扩展、执行 powerwash、重启 Chromebook 等。也于事无补。

在某些情况下，问题与高 CPU 使用率有关，因为许多人在使用诊断应用程序检查时会注意到高达 100%的 CPU 使用率。

与此同时，一些用户注意到，即使在完全正常的 CPU 使用情况下，后台也没有运行任何对性能要求很高的程序，但仍然非常缓慢。

值得一提的是，这个问题似乎不会影响所有的 ChromebooksReddit 主题中的一些用户表示，在更新到 Chrome OS 版本 91.0.4472.147 后，他们没有遇到这样的性能问题。根据现有的数据，这个问题似乎仅限于带有*咕哝*和*舱口*板的设备。

如果你在安装 Chrome OS 91.0.4472.147 后面临上述性能问题，可以考虑在 Chromium bugs 追踪器中主演[这个 bug 报告](https://bugs.chromium.org/p/chromium/issues/detail?id=1226037)。或者，你也可以在 Chromebook 上按下 *alt+shift+i* ，向 ChromeOS 团队发送报告。如果你使用的是之前版本的 Chrome 操作系统，我们强烈建议你远离 91.0.4472.147 版本。

在安装了最新的 Chrome OS 更新后，您的 Chromebook 是否面临任何性能问题？请在下面的评论中告诉我们。