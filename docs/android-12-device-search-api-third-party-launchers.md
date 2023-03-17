# Android 12 为第三方启动器增加了新的设备搜索 API

> 原文：<https://www.xda-developers.com/android-12-device-search-api-third-party-launchers/>

# Android 12 为第三方启动器增加了新的设备搜索 API

Android 12 为第三方启动器添加了新的设备搜索 API，为芝麻等通用搜索应用提供了原生替代。

谷歌[上个月发布了第二个 Android 12 开发者预览版](https://www.xda-developers.com/android-12-developer-preview-2/)，它让我们一瞥几个即将到来的功能。其中一个是[为 Pixel Launcher](https://www.xda-developers.com/android-12-dp2-hidden-features/#android12dp2searchwidget) 开发的新搜索工具，它可以让用户在他们的设备上搜索应用、联系人、设置等等。现在看来，这一功能将不仅限于 [Android 12](https://www.xda-developers.com/android-12/) 上的 Pixel 启动器。

广受欢迎的第三方主屏幕替换应用程序 [Niagara Launcher](https://www.xda-developers.com/niagara-launcher-out-of-beta/) 的开发者[在 Android 12 预览版文档](https://developer.android.com/reference/android/app/appsearch/AppSearchManager)中发现了新的证据，这表明谷歌正在 Android 12 中添加一个新的设备搜索 API，该 API 将让第三方启动器提供类似的通用搜索功能。正如你在附加的推文中看到的，该功能将让第三方启动器“访问由系统维护的集中式应用搜索索引。”

它进一步强调了 AppSearch index 是一个用于管理结构化数据的搜索库，具有以下特点:

*   完全离线的设备上解决方案
*   一组 API，供应用程序索引文档并通过全文搜索检索它们
*   允许系统在系统 UI 表面上显示其内容的应用程序 API
*   类似地，应用程序的 API 允许系统与其他指定的应用程序共享它们的内容。

这一功能本质上将为通用搜索应用程序(如 [Sesame](https://play.google.com/store/apps/details?id=ninja.sesame.app.edge) )提供一个原生的替代品，让用户可以选择在他们的设备上即时搜索几乎任何东西。虽然我们目前没有关于这一集成的进一步信息，但我们希望在即将到来的 Android 12 开发者预览版中了解更多信息。一旦我们有了更多关于整合的信息，我们将会更新这篇文章。

值得一提的是，一加已经在其原生启动器应用程序上提供了类似的通用搜索功能。然而，它被限制在一个特定的区域。随着新的 Android 12 设备搜索 API 的推出，它可能也会进入其他地区。

* * *

*特色图片:Pixel Launcher 的新搜索工具*