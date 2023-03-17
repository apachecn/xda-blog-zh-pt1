# Chromebooks 将在 Chrome OS 89 中获得一个原生剪贴板管理器

> 原文：<https://www.xda-developers.com/chromebooks-native-clipboard-manager-chrome-os-89/>

# Chromebooks 将在 Chrome OS 89 中获得一个原生剪贴板管理器

根据 Chromium Gerrit 中最近合并的提交，Chromebooks 将在 Chrome OS 89 中获得一个原生剪贴板管理器。

过去几个月，谷歌一直在努力为 Chromebooks 添加一个原生剪贴板管理器。今年 6 月，当 Chromium Gerrit 中增加了一个名为“Multipaste”的新提交时，我们第一次发现了这个特性的证据。当时，我们已经了解到剪贴板管理器将允许用户通过使用“Search+V”键盘快捷键来粘贴最后 5 个复制的项目。但当时，我们没有关于可能的发布时间表的信息。现在，我们在 Chromium Gerrit 中发现了另一个合并提交，这表明该功能将向 Chrome OS 89 用户开放。

[新提交](https://chromium-review.googlesource.com/c/chromium/src/+/2578005)的标题为“默认启用多路径”，其描述称该功能将“在 M-89 中启动”，并且默认启用。如果你错过了我们之前的报道，Chromebook 剪贴板管理器将存储最近复制的五个项目。这些可以包括文本、格式化文本、图像、书签格式的链接，以及名为“ [web 智能粘贴](https://chromium-review.googlesource.com/c/chromium/src/+/2240267/10/ash/tote/multipaste_controller.cc#61)”的东西谷歌可能还会在快速设置托盘中添加一个[按钮，在没有键盘快捷键的情况下打开剪贴板管理器。](https://chromium-review.googlesource.com/c/chromium/src/+/2188934/6/ash/system/status_area_widget.h#30)

由于谷歌最近在稳定频道上发布了 Chrome OS 87，新的原生剪贴板管理器距离用户还有一段时间。但我们很高兴谷歌决定推进这项功能，因为如果你做大量的复制和粘贴，它真的会派上用场。Windows 10 和 Gboard [提供了类似的剪贴板管理器](https://www.xda-developers.com/gboard-clipboard-manager/)，我经常使用它们。所以我可以向你保证，这是一个很棒的附加功能，可以帮你节省很多时间。但我真的希望谷歌考虑升级 Chrome OS 剪贴板管理器，以保存不止五个条目。虽然提交目前没有突出任何这样的变化，但谷歌可能会在剪贴板管理器准备就绪的时候增加限制。