# 谷歌照片准备从 7-11 当天打印；新的存储管理工具

> 原文：<https://www.xda-developers.com/google-photos-preps-same-day-prints-7-eleven-storage-management-features/>

早在 10 月份，谷歌就为谷歌照片用户推出了一项[高级打印服务](https://www.xda-developers.com/google-photos-monthly-print-service/),每月收取费用，提供 10 张高质量的照片打印服务。这项服务依靠机器学习从你的谷歌照片库中推荐 10 张照片。您可以编辑照片选择，在哑光和光面之间进行选择，并在每月发货前为照片添加边框。除了新的打印服务，谷歌还将 Wallgreens 添加到了当天打印取件地点的列表中。现在谷歌准备再增加一个位置。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

在最新版本的 Android 谷歌照片应用程序(v5.39)中，我们发现了一些字符串，表明谷歌照片用户将能够从当地的 7-Eleven 商店订购当天的照片。

```
 <string name="photos_printingskus_kioskprints_storefront_tooltip_body">Conveniently order prints from Google Photos and pick them up at 7-Eleven</string>
Prints orders will need to be placed from the Google Photos app. Users will be shown an estimated price based on the "most recent information available." The final price will be confirmed at the store at the time of checking out.
<string name="photos_printingskus_kioskprints_ui_checkout_button_disclaimer_price_estimate">* Estimated price based on most recent information available. Final price will be shown at the multicopy printer.</string>
<string name="photos_printingskus_kioskprints_ui_checkout_button_text">Place order</string>
<string name="photos_printingskus_kioskprints_ui_checkout_order_header_title">Order details</string>
<string name="photos_printingskus_kioskprints_ui_checkout_pay_in_store">Pay in store</string>
<string name="photos_printingskus_kioskprints_ui_checkout_pickup_header_title">Pick up details</string> 
```

此外，我们还发现了与 Google 正在开发的一些新的存储管理功能相关的字符串。谷歌的[免费无限存储将于 2021 年 6 月 1 日](https://www.xda-developers.com/psa-google-photos-will-no-longer-offer-free-unlimited-storage-next-year/#:~:text=Google%20also%20said%20it%20will%20offer%20a%20new%20free%20tool%20next%20summer%20that%20will%20help%20Photos%20app%20users%20easily%20manage%20their%20already%20backed%20up%20media)到期，从那时起上传的所有照片和视频都将计入分配给你的谷歌账户的 [15GB 限制](https://support.google.com/photos/answer/6220791?co=GENIE.Platform%3DAndroid)。为了帮助人们充分利用 15GB 的空间，谷歌将分析你的照片库，并通过删除模糊、太暗或重复的照片来提供清理空间的建议。它还会告诉你这些照片占用了多少空间。

```
 <string name="photos_quotamanagement_data_blurry_empty_state_subtitle">Blurry photos detected in your library that count towards your storage will show here</string>
<string name="photos_quotamanagement_data_blurry_empty_state_title">No blurry photos to delete</string>
<string name="photos_quotamanagement_data_blurry_photos_category_title">Blurry photos</string>
<string name="photos_quotamanagement_data_dark_empty_state_subtitle">Dark photos detected in your library that count towards your storage will show here</string>
<string name="photos_quotamanagement_data_dark_empty_state_title">No dark photos to delete</string> 
```

Google 相册会显示你的图库中是否有过大的照片或视频，以及它们占用了多少空间。此外，它将向您显示来自其他应用程序和截图的照片和视频如何影响您的存储配额。

```
 <string name="photos_quotamanagement_data_large_empty_state_subtitle">Large photos or videos detected in your library that count towards your storage will show here</string>
<string name="photos_quotamanagement_data_large_empty_state_title">No large photos or videos to delete</string>
<string name="photos_quotamanagement_data_large_photos_and_videos_category_title">Large photos &amp; videos</string>
<string name="photos_quotamanagement_data_other_app_empty_state_subtitle">Photos &amp; videos detected from other apps that count towards your storage will show here</string>
<string name="photos_quotamanagement_data_other_app_empty_state_title">No photos or videos from other apps to delete</string>
<string name="photos_quotamanagement_data_other_applications_category_title">Other apps</string>
<string name="photos_quotamanagement_data_screenshot_empty_state_subtitle">Screenshots detected in your library that count towards your storage will show here</string> 
```

Google 相册还会根据您的使用模式，预测您的存储空间在几个月或几年内可以使用多长时间。这个估计会在几个月的定期照片和视频上传后出现。

```
 <string name="photos_quotamanagement_forecast_about_months_of_storage">{months, plural, =1{About 1 month of storage left} other{About # months of storage left} }</string>
<string name="photos_quotamanagement_forecast_about_years_of_storage">{years, plural, =1{About 1 year of storage left} other{About # years of storage left} }</string>
<string name="photos_quotamanagement_forecast_more_than_years_of_storage">{years, plural, =1{More than 1 year of storage left} other{More than # years of storage left} }</string>
<string name="photos_quotamanagement_forecast_subtitle_no_data">You’ll see an estimate here after you upload photos &amp; videos consistently for a few months</string> 
```

最后，有一些新的字符串确认谷歌 Pixel 手机将不会受到新变化的影响，并将在 2021 年 6 月 1 日之后继续享受免费、无限的高质量和快递质量备份。这可能只适用于现有的谷歌 Pixel 手机，因为谷歌已经确认未来的 Pixel 手机[不会在谷歌照片中提供无限的高质量备份](https://www.xda-developers.com/future-pixel-phones-reportedly-wont-get-unlimited-google-photos-backups/)。

```
 <string name="photos_quotamanagement_summary_free_hq_storage_pixel_ab_off">High quality on this device is free &amp; unlimited. Turn on in &lt;a href=backup_settings>backup settings&lt;/a>.</string>
<string name="photos_quotamanagement_summary_free_hq_storage_pixel_express_backup">You’re backing up in Express from your %s, which is free &amp; unlimited</string>
<string name="photos_quotamanagement_summary_free_hq_storage_pixel_hq_backup">You’re backing up in High quality from your %s, which is free &amp; unlimited</string>
<string name="photos_quotamanagement_summary_free_hq_storage_pixel_oq_backup">Backing up in High quality on this device is free &amp; unlimited. Change in &lt;a href=backup_settings>backup settings&lt;/a>.</string> 
```