# 无法登录您的 Chromebook？谷歌正在准备修复

> 原文：<https://www.xda-developers.com/cant-login-chromebook-google-readying-fix/>

谷歌上月底在稳定频道推出了 Chrome OS 91.0.4472.147。但是更新被取消了，因为它在几个 Chromebook 型号中引起了性能问题。上周，[谷歌恢复推出](https://www.xda-developers.com/chrome-os-91-high-cpu-bug-fixed/)，新的 Chrome OS 91 版本没有同样的高 CPU 使用率问题。然而，它带来了另一个恼人的错误。

*Android Police* [报道](https://www.androidpolice.com/2021/07/20/a-new-chrome-os-91-update-is-breaking-chromebooks-like-a-bull-in-a-china-shop/)最新的 Chrome OS 91 版本(v91.0.4772.165)引入了一个不允许用户登录 Chromebooks 的 bug。关于 *Reddit* 的几份报告揭示了新版本造成的损害程度，用户透露他们的 chrome book[在更新后的登录屏幕](https://www.reddit.com/r/chromeos/comments/oniply/warning_the_latest_stable_update_is_stopping/h5ryqx0?utm_source=share&utm_medium=web2x&context=3)上不接受他们的密码。根据一位用户的说法，一个 [powerwash 对他们的华硕 Chromebook C436 没有任何帮助](https://www.reddit.com/r/chromeos/comments/onhfrg/updated_chromebook_spin_713_and_unable_to_log_in/h5runh0?utm_source=share&utm_medium=web2x&context=3)，他们不得不求助于使用恢复 USB 来让他们的 Chromebook 工作。

虽然谷歌已经意识到这个问题，并正在更新，但如果你在 Chromebook 上收到更新提示，请不要关闭它。如果你这样做，Chrome OS 将在重启时自动安装更新，你可能会被锁定在 Chromebook 之外。

谷歌澄清说，Chrome OS 团队已经发现了最新版本的潜在问题，并将于 7 月 21 日发布修复程序。与此同时，如果你的 Chromebook 不允许你登录，我们建议你等待新的更新推出。一旦完成，你的 Chromebook 将会自动更新，你应该可以再次登录，而不需要重新启动。

虽然谷歌还没有分享任何关于这个问题的信息，但一位 [*Reddit* 用户透露](https://www.reddit.com/user/elitist_ferret/)代码中的一个[拼写错误是最近一次惨败的原因。如果你看看](https://www.reddit.com/r/chromeos/comments/onlcus/update_it_seems_google_has_pulled_the_165_stable/h5vev76?utm_source=share&utm_medium=web2x&context=3)[这个文件](https://chromium-review.googlesource.com/c/chromiumos/platform2/+/3039560/2/cryptohome/vault_keyset.cc#b471)的区别，你会注意到 Chrome OS 团队忘记在条件语句中添加第二个“&”，阻止用户登录他们的 Chromebooks。