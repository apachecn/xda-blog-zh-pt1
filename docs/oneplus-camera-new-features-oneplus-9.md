# 这是一加正在为其下一代手机开发的新相机功能

> 原文：<https://www.xda-developers.com/oneplus-camera-new-features-oneplus-9/>

上周，一加为一加 7 和 7T 系列推出了首个基于 Android 11 的 OxygenOS 公开测试版[。此次更新带来了一加相机应用程序的新版本——版本 6 . 4 . 23——其中包含新的资产、字符串和代码，暗示了新的相机功能。这些功能尚未在最新更新中启用，但可能会在未来的设备上启用。随着该公司的](https://www.xda-developers.com/oneplus-7-7-pro-7t-7t-pro-android-11-oxygenos-open-beta-1/)[下一个旗舰发布](https://www.xda-developers.com/oneplus-9-reportedly-launching-earlier-than-expected-next-year/)定于 3 月，这里是我们所知道的关于它可能首次亮相的相机功能。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

**倾斜移位模式**

更新中提到的一个新功能叫做“倾斜移位”。这是指倾斜移位摄影或微型伪造，一种使场景看起来比实际小得多的摄影技术。以下是添加的字符串:

```
 <string name="capture_mode_tiltshift">Tilt-shift</string>
<string name="tiltshift_introduction_guide_1">1\. Select location</string>
<string name="tiltshift_introduction_guide_1_detail">Tap the screen to change the location of the blurred area.</string>
<string name="tiltshift_introduction_guide_2">2\. Adjust the scope</string>
<string name="tiltshift_introduction_guide_2_detail">Adjust the blurred area with two fingers.</string>
<string name="tiltshift_introduction_guide_3">3\. Adjust the angles</string>
<string name="tiltshift_introduction_guide_3_detail">Change the angles with double finger rotation.</string>
<string name="tiltshift_introduction_guide_4">4\. Adjust intensity</string>
<string name="tiltshift_introduction_guide_4_detail">Tap the button to adjust the intensity of the blurred area.</string>
<string name="tiltshift_introduction_guide_end">Try it Out</string>
<string name="tiltshift_introduction_guide_start">Steps to take perfect photos:</string>
<string name="tiltshift_introduction_overview">Tilt-shift mode can transform the world into a miniature version. Buildings and people will resemble tiny models in the shifting lens, displaying the visuals of an \"artificial city\" in photos. Here are some samples!</string>
<string name="tiltshift_introduction_title">About Tilt-shift mode</string> 
```

感谢 XDA 会员 [Lossyx](https://forum.xda-developers.com/m/lossyx.5668276/) ，我们能够发布倾斜移位模式的介绍活动的截图，以展示该功能在一加相机应用程序中的外观，但我们的线人无法从他们的设备中捕捉任何实际的倾斜移位照片。

*演职员表:XDA 成员[LossyX](https://forum.xda-developers.com/m/lossyx.5668276/)*

**星爆**

当你把相机对准一个明亮的光源，如太阳，你可能会看到一个辐射的星形，而不是一个点。这被称为星爆效应，似乎一加相机应用程序将提供一个专门的模式来捕捉这种效应的照片。相机应用程序可能会选择一个最佳光圈，既足够小以实现效果，又足够大以最大限度地提高整体图像清晰度。

```
 <string name="starburst_hint_close">Starburst is off</string>
<string name="starburst_hint_open">Starburst is recommended while shooting with a light source</string>
<string name="night_mode_hint_starburst_effect">Starburst Effect</string> 
```

**月球模式**

而[一加 9 和 9 Pro](https://www.xda-developers.com/oneplus-9/) 可能不会有潜望式长焦相机——至少[根据 tipster Max 报道。对于那些想要捕捉夜空照片的人来说，一加正在追赶月亮模式的潮流。相机应用程序将提供不同的滤镜来调整月亮的颜色。](https://twitter.com/MaxJmb/status/1353750174137540608)

```
 <string name="settings_moon">About \"Moon Natural Colour Solution\"</string>
<string name="filter_black_white_moon">B&amp;W</string>
<string name="filter_moon_black_white_new">OBW 2</string>
<string name="filter_moon_mono">OBW 1</string>
<string name="filter_moon_snapseed">OBW 3</string>
<string name="filter_pop_moon">Vivid</string>
<string name="filter_soft_moon">Matte</string> 
```

**过度流逝**

一加相机应用已经提供了延时模式，但似乎很快也会提供专用的超延时模式。时间间隔通常是固定的，而超时间间隔会增加长距离的运动。

```
 <string name="hyperlapse">Hyperlapse</string>
<string name="user_assistive_put_subject_inside_frame">Please put the subject in the frame</string> 
```

**聚焦峰化**

最后，一个字符串指向一加相机应用程序中添加的对焦峰值功能。这个功能可能会突出取景器中的任何对焦区域，如果它类似于许多无反光镜相机中的功能。

```
 <string name="content_description_peeking_focus">Focus Peaking</string> 
```

正如我之前提到的，在最新版本的一加相机应用程序中，这些功能似乎都没有对用户开放。因此，我们怀疑这些功能是为即将推出的设备保留的，无论是在主要编号系列的 Nord 系列中。我们知道一加正在开发一些新设备，但我们不知道哪些设备将率先推出这些功能。

* * *

*感谢 XDA 会员 [Some_Random_Username](https://forum.xda-developers.com/m/some_random_username.8234677/) 的提示，感谢 PNF 软件为我们提供使用许可**[JEB Decompiler](https://www.pnfsoftware.com/?aid=xdadev)**，这是一款针对 Android 应用的专业级逆向工程工具。*

*专题图片:一加 8T 赛博朋克 2077 版*