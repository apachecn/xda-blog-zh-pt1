# Google 相册 5.18 确认为 Google One 成员提供高级编辑功能

> 原文：<https://www.xda-developers.com/google-photos-5-18-confirms-premium-editing-features-google-one-members/>

在过去的几个月里，谷歌一直致力于为谷歌照片添加高级编辑功能。早在今年 3 月，我们[在 APK 对 Google 相册 4.45 版的拆解中首次发现了该功能的证据](https://www.xda-developers.com/google-photos-445-tests-ordering-photo-prints-memories-view-hints-premium-editing-features-one-subscribers/)。当时，我们得知该功能仅提供给 Google One 成员。在接下来的更新中，我们[发现了更多的字符串](https://www.xda-developers.com/google-photos-4-46-prepares-photo-creations-memories/)，这表明照片应用程序将向用户“追加销售”新的优质编辑工具。然而，字符串并没有揭示编辑功能。现在，我们终于设法在最新发布的 Google 相册中找到了一些关于即将推出的功能的具体证据。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Google Photos v5.18 最近开始通过 Play Store 向用户推出。从表面上看，更新只包括对*“改进编辑过的照片和视频在 SD 卡上的保存和存储”的错误修复*但是 APK 的拆卸揭示了突出显示关于高级编辑功能的新信息的字符串。

```
 <string name="photos_photoeditor_fragments_editor3_g1_callout_g1_member">As a Google One member, you get access to extra editing features</string>

<string name="photos_photoeditor_fragments_editor3_g1_callout_non_member">Get extra editing features with a Google One membership</string>

<string name="photos_photoeditor_fragments_editor3_upsell_banner">Unlock this feature and more with a Google One membership</string>

<string name="photos_photoeditor_fragments_editor3_upsell_title_with_storage">Unlock more editing features and {storage_amount} of storage with a Google One membership</string> 
```

首先，字符串包括新的提示，将提醒用户高级编辑功能，并敦促他们获得 Google One 会员资格。这些新的提示将如下所示:“作为 Google One 会员，您可以访问额外的编辑功能”，“使用 Google One 会员身份获得额外的编辑功能”，“使用 Google One 会员身份解锁此功能和更多功能”，以及“使用 Google One 会员身份解锁更多编辑功能和{storage amount}存储空间。”但是，尽管这些新的提示明确提到了高级编辑功能，但它们没有透露谷歌 One 订阅后将锁定哪些功能的确切信息。

**更新:** [安迪 J](https://disqus.com/by/AndrewSimonJones/) 在评论中说“彩色流行”编辑功能被他锁在谷歌 One 付费墙后面。在接下来的文章中，我们写了关于这个测试的更多细节[。](https://www.xda-developers.com/google-photos-tests-locking-color-pop-behind-a-google-one-paywall/)

### 预处理建议

接下来，我们发现了新的字符串，它们讨论了 Google 相册的预处理建议:

```
 <string name="photos_photoeditor_preprocessing2_dogfood_suggestion_dynamic">Dynamic</string>

<string name="photos_photoeditor_preprocessing2_dogfood_suggestion_hdr">HDR</string>

<string name="photos_photoeditor_preprocessing2_dogfood_suggestion_vivid">Vivid</string> 
```

这些字符串表明，应用程序中的照片编辑器将提供三种预处理建议——动态、HDR 和生动。但目前，还不清楚这些建议将如何展示给用户。

### skypaletta 建议

最后，以下字符串表明 Google 相册可能很快会有新的过滤器来帮助用户编辑天空:

```
 <string name="photos_photoeditor_skypalette_suggestion_afterglow">Afterglow</string>

<string name="photos_photoeditor_skypalette_suggestion_airy">Airy</string>

<string name="photos_photoeditor_skypalette_suggestion_ember">Ember</string>

<string name="photos_photoeditor_skypalette_suggestion_luminous">Luminous</string>

<string name="photos_photoeditor_skypalette_suggestion_radiant">Radiant</string>

<string name="photos_photoeditor_skypalette_suggestion_stormy">Stormy</string> 
```

Skypallete 的建议包括六种滤镜——余辉、轻风、余烬、发光、辐射和风暴。这些滤镜很可能会像 MIUI Gallery 应用程序中的[天空替换滤镜](https://www.xda-developers.com/download-miui-12-gallery-adds-ocr-screenshot-device-frames-new-sky-replacement-filters/)一样工作，允许用户用包含的预设替换他们图像中的天空。

截至目前，我们无法确认新的预处理和 Skypallete 建议是否会被锁定在 Google One 订阅之后。但由于它们是在新的高级编辑锁定的同时开发的，情况可能就是这样。

* * *

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*