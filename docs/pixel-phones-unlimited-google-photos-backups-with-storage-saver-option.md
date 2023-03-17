# 未来的 Pixel 手机不会获得无限制的 Google 相册备份

> 原文：<https://www.xda-developers.com/pixel-phones-unlimited-google-photos-backups-with-storage-saver-option/>

**更新 1 (05/06/2021 @ 08:56 PM ET):** 看起来“存储节省器”只是 Google 相册中现有“高质量”选项的新名称。[点击这里了解更多信息。今天早些时候发表的这篇文章保留在下面。](#update1)

从下个月开始，Google 相册[将不再为存储“高质量”照片提供免费的无限存储空间](https://www.xda-developers.com/google-photos-unlimited-free-storage-expires-next-month/)。这意味着在 2021 年 6 月 1 日之后上传到 Google 相册的任何新照片，无论是“高质量”、“原始质量”还是“快速质量”，都将计入分配给你的 Google 帐户的 15GB 限制。如果你用完了这个限额，你将不得不为 Google One 付费。幸运的是，目前的谷歌 Pixel 手机不受此影响，将继续终身获得无限制的高质量上传。有报道称，谷歌不打算在未来的像素上提供这项额外待遇。该公司甚至正式证实，未来的 Pixel 手机确实[不会获得无限的高质量照片备份](https://www.xda-developers.com/future-pixel-phones-reportedly-wont-get-unlimited-google-photos-backups/)。但谷歌似乎仍然可以在未来的 Pixel 手机上提供某种形式的无限备份。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

在谷歌照片应用 v5.4.1 中，我们发现了一个新的存储保护照片质量选项的证据，该选项可以允许未来的 Pixel 手机进行无限备份。

目前，Google 相册提供三种备份选项:原始、高质量和快速质量(在特定市场)。但以下新字符串表明，谷歌正在努力增加一个新的存储保护选项，似乎可以让你备份照片的质量略有下降。

```
 <string name="photos_autobackup_particle_items_left_with_saver_storage_policy">{count, plural, =1{1 item left • Storage saver} other{# items left • Storage saver}}</string>
<string name="photos_backup_settings_saver_title_with_description">Storage saver (slightly reduced quality)</string> 
```

新的存储保护选项将允许 Pixel 手机免费上传无限的照片和视频。由于现有的 Pixel[已经拥有无限的高质量备份特权](https://www.xda-developers.com/google-photos-preps-same-day-prints-7-eleven-storage-management-features/)，我们猜测这一变化很可能适用于未来的 Pixel 手机。或者，谷歌也可能只是将现有的“高质量”选项更名为“存储节省程序”，因为它们在描述中都提到了同一个“质量略有下降”的短语。

```
 <string name="photos_cloudstorage_strings_impl_saver_learn_more_footer_pixel">Unlimited storage in Storage saver only applies to photos &amp; videos backed up from this Pixel device. &lt;a href=help:>Learn more&lt;/a></string>
<string name="photos_cloudstorage_strings_impl_saver_learn_more_footer_pixel_express">Unlimited storage in Storage saver or Express only applies to photos &amp; videos backed up from this Pixel device. &lt;a href=help:>Learn more&lt;/a></string>
<string name="photos_cloudstorage_strings_impl_storage_meter_progress_pixel_unlimited_saver">Backing up in Storage saver quality from your %s is free and unlimited</string>
<string name="photos_cloudstorage_strings_saver_title">Storage saver</string>
<string name="photos_pixel_offer_full_pixel_saver_backup_quality_description">New items will back up in Storage saver backup quality (slightly reduced quality). Items uploaded before %s will remain free at Original quality.</string>
<string name="photos_pixel_offer_full_pixel_updated_backup_saver_quality_summary">New photos will back up in Storage saver backup quality</string>
<string name="photos_quotamanagement_summary_free_hq_storage_pixel_saver_backup">You’re backing up in Storage saver quality from your %s, which is free &amp; unlimited</string>
<string name="photos_quotamanagement_summary_free_saver_storage_pixel_ab_off">Storage saver quality on this device is free &amp; unlimited. Turn on in &lt;a href=backup_settings>backup settings&lt;/a>.</string>
<string name="photos_quotamanagement_summary_free_saver_storage_pixel_oq_backup">Backing up in Storage saver quality on this device is free &amp; unlimited. Change in &lt;a href=backup_settings>backup settings&lt;/a>.</string> 
```

这个新的存储保护选项还没有在 Google 相册中推出。如果我们发现任何新的证据，我们将更新这个帖子的更多细节。

* * *

## 更新 1:“存储保护程序”不是 Google 相册中的新备份层

谷歌发言人联系了我们，并发表了以下声明:

> #### “我们之前宣布的关于 Pixel 设备的 Google 相册存储没有变化。我们正在为我们的照片备份选项探索新的名称，并且没有计划引入额外的存储选项。”

因此，“存储保护程序”并不是 Google 相册中的新备份层，而是现有“高质量”层的新名称。谷歌正计划对更名进行 A/B 测试，这是有道理的，因为“高质量”和“原始质量”之间的区别可能会让一些人感到困惑。不幸的是，未来的 Pixel 手机仍将不受即将到来的存储政策变化[的影响，该变化将于下月](https://www.xda-developers.com/google-photos-unlimited-free-storage-expires-next-month/)生效。

*本文更新于美国东部时间 2021 年 5 月 7 日下午 2:16，谷歌发言人发表声明。*