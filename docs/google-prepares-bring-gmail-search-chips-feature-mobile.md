# Android 版 Gmail 为过滤聊天信息准备了搜索芯片

> 原文：<https://www.xda-developers.com/google-prepares-bring-gmail-search-chips-feature-mobile/>

# 安卓版 Gmail 准备增加搜索芯片过滤聊天信息

Gmail 应用程序的拆除揭示了新的字符串，表明搜索芯片正在过滤聊天信息。

今年二月早些时候，谷歌在 Gmail 中引入了名为“搜索芯片”的新功能。这项功能在 Gmail 中为 G Suite 用户增加了可点击的搜索建议，使得搜索过滤器更容易使用。最初发布几个月后，谷歌[在 Gmail 中为消费者推出了搜索芯片](https://www.xda-developers.com/google-starts-rolling-out-search-chips-gmail-consumers/)。虽然该公司尚未在移动版 Gmail 中添加该功能，但他们正在为聊天工具的[用户带来类似的搜索过滤功能。](https://www.xda-developers.com/google-meet-google-chat-google-rooms-gmail-g-suite/)

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Android 版 Gmail 应用程序(v. 2020.10.04)的拆除发现了新的代码字符串，暗示即将推出的聊天信息搜索过滤器。在搜索栏中输入任何关键词都会在搜索栏下方显示相关的搜索芯片。点击搜索芯片将立即应用一个过滤器，并在下面显示所有相关信息。

```
 <string name="search_filtering_attachment_chip_title_with_count">Attachment+%d</string>
<string name="search_filtering_author_chip_title">From</string>
<string name="search_filtering_author_chip_title_with_name">From %s</string>
<string name="search_filtering_author_chip_title_with_name_and_count">From %1$s+%2$d</string>
<string name="search_filtering_dialog_attachment_icon_content_description">Attachment icon</string>
<string name="search_filtering_documents_chip_title">Documents</string>
<string name="search_filtering_documents_chip_title_with_count">Documents+%d</string>
<string name="search_filtering_images_chip_title">Images</string>
<string name="search_filtering_images_chip_title_with_count">Images+%d</string>
<string name="search_filtering_pdf_chip_title">PDFs</string>
<string name="search_filtering_pdf_chip_title_with_count">PDF+%d</string>
<string name="search_filtering_people_suggestion_header_title">Suggested</string>
<string name="search_filtering_sheets_chip_title">Sheets</string>
<string name="search_filtering_sheets_chip_title_with_count">Sheets+%d</string>
<string name="search_filtering_slides_chip_title">Slides</string>
<string name="search_filtering_slides_chip_title_with_count">Slides+%d</string>
<string name="search_filtering_video_chip_title">Videos</string>
<string name="search_filtering_video_chip_title_with_count">Video+%d</string> 
```

正如你在下面 Android 开发者和逆向工程师 Alessandro Paluzzi 的截图中看到的，有几个过滤建议，包括作者和附件。点击这些建议会缩小你的搜索范围，这比键入 Gmail 的旧过滤器要简单得多。

到目前为止，我们还没有从谷歌得到任何关于手机版 Gmail 中搜索芯片整合的信息。我们将在 Gmail for Android 的未来版本中启用该功能后立即更新这篇文章。

*本文于美国东部时间 2020 年 10 月 30 日下午 1:43 更新，以反映这些搜索过滤器旨在过滤聊天消息而非电子邮件。*