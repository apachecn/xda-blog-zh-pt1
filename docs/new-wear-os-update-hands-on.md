# 多年来最大的 Wear 操作系统更新已经到来:下面是它的样子

> 原文：<https://www.xda-developers.com/new-wear-os-update-hands-on/>

今天早些时候， [Google I/O 2021](https://xda-developers.com/tag/google-io-2021) 开发者大会拉开帷幕，有 *lot* 重大消息宣布。从谷歌生态系统中许多服务的几个新功能和改进，到让开发者生活更轻松的新闻，谷歌 I/O 2021 一直是多年来最大的科技事件之一。当然，大会上最大的宣布是面向智能手机的 [Android 12](https://www.xda-developers.com/android-12/) 的正式发布。但并不是每一个安卓产品都是围绕手机发布的。谷歌终于再次对智能手表和 Wear OS 生态系统的 Android 给予了更多关注，新版本是 Wear OS 自首次推出以来最大的更新之一。

Wear OS 的这个新版本尤其引人注目，因为它不仅仅是新 Android 版本的又一个基础。相反，谷歌宣布与三星合作重建平台，令许多人感到惊讶。三星已经表明了其对重建智能手表平台的承诺，宣布他们将制作搭载 Wear OS 的[新款 Galaxy 智能手表，而不是该公司的 Tizen，他们与谷歌合作，采用了一些让 Tizen 如此受用户喜爱的功能，并将它们带到 Wear OS 上。结果不言自明。新版 Wear OS 看起来很清新。](https://www.xda-developers.com/fitbit-and-samsung-are-working-on-new-watches-with-wear-os/)

虽然我们还没有任何运行新版 Wear OS 的硬件，但谷歌已经更新了 Android Studio 中的官方 Wear 模拟器图像[，所以我们可以看到一些变化。](https://www.xda-developers.com/google-io-2021-new-features-jetpack-android-studio-kotlin/)

## 设计变更:材料你来了！

首先，我们需要谈谈新的设计。谷歌在今天的主题演讲中宣布了其产品系列的新设计语言， [Material You](https://www.xda-developers.com/material-you/) ，这是 Android 12 设备，至少是那些运行 Android 的设备将会运行的主题。与之前的任何其他材料设计相比，它更加注重个性化，这很可能是谷歌自 2014 年以来最大的设计变化，当时他们与 Android 5.0 Lollipop 一起宣布了最初的材料设计指南。Wear OS 也将遵循这些准则，它们与由该操作系统支持的较小外形智能手表完美融合。

从智能手表到菜单，到通知，以及介于两者之间的一切事物，都可以看到新的设计准则。应用程序列表中的项目被封装在药丸中，通知的边角更加圆润，粗体字体随处可见。这与以前版本的 Wear OS 中的材质主题指南有显著的不同。它们也很好地融入了新的 Android 设计语言，但它们肯定比智能手机更微妙。有些变化非常微妙，尤其是与以前相比，而另一些变化则很明显。这些新的设计变化也适用于谷歌应用程序。

首先，新的应用抽屉在每个项目上都有一个细长的药丸形状的设计，类似于我们在一些谷歌小工具中看到的。它在功能上与以前的 Wear OS 版本没有太大区别，但它看起来更光滑、更优雅。

Wear OS 没有壁纸，所以 Android 12 基于壁纸的主题化系统在这里根本看不到。我们还应该注意到，这个新版本的 Wear OS 基于 Android 11，尽管采用了更新的材料设计指南。截图中显示的默认表盘也差不多就是这样:默认表盘。每个原始设备制造商都会在表盘上打上自己的印记。

[video width = " 280 " height = " 280 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/05/New-Wear-OS-QS-tiles . MP4 "]

快速设置菜单也大大改进了可用性。较小的显示屏也使小按钮更难点击，因此 Wear OS 中新设计的快速设置菜单使用更大、更容易点击的按钮来提高可用性。考虑到这一点，亮度等部分也使用按钮，而不是智能手机中使用的典型滑块。磁贴在外观和功能上都得到了改进:现在，当你在磁贴上滑动时，当你到达终点时，它会自动回绕。向左滑动时，谷歌助手也不再可用:你现在需要双击电源按钮才能访问它。其他手势包括双击后退按钮在应用程序之间切换。

[video width = " 280 " height = " 280 " MP4 = " https://static 1 . xdaimages . com/WordPress/WP-content/uploads/2021/05/New-Wear-OS-Notification-animation . MP4 "]

最后，通知功能采用了全新的设计，这一次，更符合 Android 智能手机上可以看到的内容。通知采用圆角渐变设计，如果不能一目了然地看到完整的通知，可以通过按住通知来扩展。

## Wear OS 中的 Fitbit 精华，以及更多应用和功能！

谷歌还宣布，[谷歌最近收购的健身品牌](https://www.xda-developers.com/google-completes-fitbit-buyout-after-months-of-scrutiny/)Fitbit 的最佳功能将佩戴 OS 智能手表。Wear OS 将能够跟踪你的锻炼情况，跟踪你走了多少步，跟踪你一天的健康进展，甚至可以在手腕上显示目标庆祝活动，让你振作起来，激励你走向更健康的生活。目前还不清楚一些功能是否需要额外的硬件支持，或者它们是否与现有的 Wear OS 硬件兼容。

这并不意味着智能手表将很快取代健身带。有很多智能手表都有健身跟踪功能，其中很多都有专门的传感器。健身手环仍然在市场上占有一席之地，因为它们便宜得多，并且没有智能手表那样的功能。

谷歌还致力于为 Wear OS 生态系统带来更多更好的应用。Fitbit 只是实现这一目标的一步:谷歌地图和谷歌助手等其他谷歌服务也在改进，以在智能手表上提供更好的全方位体验。还有其他 app？嗯，Google very [最近为平台](https://www.xda-developers.com/gboard-wear-os-available/)带来了 Gboard，他们也想让开发者更容易将自己的应用程序带到操作系统上，这就引出了我们的下一点...

## 开发人员现在就可以开始行动了！

谷歌还敦促开发 Wear OS 应用的开发者严格遵守这些指导方针和 APIs 是的，甚至是设计方面。Android 开发者门户中的 Wear OS UI 文档已被更改，以展示新的设计语言，以及开发者需要如何遵循它。你设计语言的新材料适用于通知、复杂功能(手表表面的小部件)、叠加、磁贴、应用程序启动器，如果你想，还可以观察面部，你可以坚持或密切关注它们，同时也给应用程序带来你自己的个性化旋转。

这个更新被吹捧为有史以来“穿戴操作系统的最大更新”。我们当然明白谷歌的意思。谷歌甚至让三星加入了新的 Wear OS 版本，考虑到三星一直在以 Tizen 的形式开发智能手表 OS，这一点令人印象深刻。从现在开始，Wear OS 将在谷歌的生态系统中扮演更加重要的角色。

为了准备新版本的 Wear OS，谷歌还发布了几个开发工具和 API，让开发人员开始让他们的应用程序与这个新的操作系统兼容。作为这些更新的一部分，新的 Jetpack APIs 正在被添加，例如 [Tiles API](https://www.xda-developers.com/wear-os-third-party-custom-tiles/) ，它旨在向每个人开放 Wear OS Tiles，使开发人员可以轻松地使用它们。还有正在进行的活动 API，它允许你的用户在导航离开后返回到你的应用程序(开始不同的任务，如音乐播放)，方法是点击表盘底部的活动指示器图标，双击侧按钮，或使用应用程序列表的最近部分。

最后但同样重要的是，我们还有健康服务，这是一个与三星合作创建的健康和健身平台(可能也是 Fitbit 的功能依赖于其 Wear OS 支持)。该平台提供来自传感器的运动和健康数据，以及情境感知算法和持续健康监测。这些 API 可用于为可穿戴设备构建高质量、高效的健身和健康体验，同时需要较少的开发时间。

* * *

如果谷歌在 2021 年推出 Wear OS 的承诺得到兑现，我们可能会看到基于 Android 的智能手表平台自首次推出以来最大的一次改造。佩戴操作系统的智能手表实际上可能会与苹果手表竞争，只要我们[也能获得更好的硬件](https://www.xda-developers.com/google-giving-wear-os-attention-need-new-hardware/)，这几乎是肯定的，因为三星已经加入了。如何看待新版 Wear OS？