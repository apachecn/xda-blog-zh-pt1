# Android 12 新的最近网址共享功能使得复制链接变得容易

> 原文：<https://www.xda-developers.com/android-12-recent-url-sharing-feature/>

谷歌最近推出了 Android 12 beta 3，对之前的测试版进行了大量的修改和改进。虽然谷歌在博客中提到了第三个测试版中所有面向用户的重大变化，但该公司在公告中没有提到一个相当有用的功能——最近的 URL 共享。在本帖中，我们将快速浏览一下这个特性，并简要解释它是如何工作的。

Android 12 新的[最近 URL 共享](https://www.xda-developers.com/android-12-beta-3-features/#android12beta3_copylinks)功能可以让你快速复制最近应用概览中的链接。当 Beta 3 首次推出时，我们不知道它是如何工作的，因为谷歌没有正式宣布这项功能。但是该公司现在已经分享了[开发者文档](https://developer.android.com/about/versions/12/features#recents-url-sharing)，这让人们对这个很酷的新功能有了一些了解。

根据文档，最近的 URL 共享功能可以由任何提供 web UI 并覆盖 Activity 类的 [onProvideAssistContent](https://developer.android.com/reference/android/app/Activity#onProvideAssistContent(android.app.assist.AssistContent)) 方法的应用程序来启用。该方法[用于](https://developers.google.com/assistant/app/assistant-sharing)向助手应用提供关于当前前景内容的结构化信息。本质上，应用程序可以告诉助手当前的前台内容是从特定的网页加载的。在 Android 12 中，该 URL 被提取并显示给用户，允许他们轻松地从最近的应用概述中复制它。

正如你在所附的截图中看到的，在最近的应用程序概览中，该 URL 作为图标出现在应用程序卡的右上角。你可以点击它来查看完整的网址，然后从最近的应用概述中复制或分享它。点击按钮还会在底部显示联系建议，帮助您在同一个屏幕上分享网址。

目前，如果你想从谷歌 Chrome 复制一个链接并与朋友分享，你必须点击地址栏，然后点击复制按钮，切换到你选择的消息应用程序，然后在点击发送之前粘贴网址。或者，您可以点击地址栏，然后点击共享按钮，从共享表中选择您希望共享链接的应用程序，然后选择您希望与之共享链接的联系人。在这两种情况下，这是一个相当漫长的过程。

最近的 URL 共享功能旨在通过向上滑动打开最近的应用程序概览，然后从同一个屏幕复制或共享链接，在很大程度上简化这一过程。