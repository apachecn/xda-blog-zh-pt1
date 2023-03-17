# 谷歌 Chrome 将很快让选项卡静音变得更加容易

> 原文：<https://www.xda-developers.com/google-chrome-tab-mute-feature/>

谷歌 Chrome 可能会恢复一个功能，让你通过点击扬声器图标来快速静音。这一功能在旧版本的 Chrome 中存在，但在 2018 年 9 月，谷歌决定将其从浏览器中移除。但看起来它可能会很快卷土重来。

正如 Reddit 用户 *Leopeva64-2* 所发现的，一个[的新补丁](https://chromium-review.googlesource.com/c/chromium/src/+/3115507)已经上传到 Chromium Gerrit，这表明谷歌可以将静音选项带回 PC 上的 Chrome 浏览器。

补丁的描述如下:

> 恢复“删除-启用-选项卡-音频-静音”
> 
> 这将恢复提交 479 cc 17585 a 64910853 e 9949 b 053499 ecbeca 9 a 5。
> 
> 恢复的原因:将此恢复

目前，Chrome 允许你通过右击标签并从上下文菜单中选择“静音站点”选项来静音。选择此选项将使该特定网站的所有标签静音，直到您取消静音。但是，这个选项可能并不总是理想的选项，因为它完全禁用了网站的音频播放功能。

一旦这种新的静音选项推出，用户只需点击出现在播放音频标签上的扬声器图标。这样做将暂时静音您当前的标签，而不是整个网站。

这项功能在微软的 Edge 浏览器中可用，你可以在下面附的 GIF 中看到它的运行情况(礼貌: *Leopeva64-* 2)

请注意，新的选项卡静音选项仍在开发中，并没有在任何 Chrome 版本中推出。正如 Leopeva64-2 指出的，仅仅因为补丁已经上传到 Chromium Gerrit，并不保证它会进入 Chrome 浏览器——它永远有可能不会被合并。

与此同时，一个类似的静音按钮[和音量滑块一起被添加到 Chrome 的全球媒体控制中。谷歌](https://www.reddit.com/r/chrome/comments/p8n54c/global_media_controls_now_have_a_mute_button/?utm_source=share&utm_medium=web2x&context=3)[自五月以来一直致力于这些功能](https://www.xda-developers.com/google-chrome-media-player-update/)，它们现在已经在最新版本的 Chrome Canary 中上线。