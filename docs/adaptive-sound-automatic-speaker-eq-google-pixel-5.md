# 谷歌为 Pixel 5 上的自动扬声器均衡器准备了自适应声音

> 原文：<https://www.xda-developers.com/adaptive-sound-automatic-speaker-eq-google-pixel-5/>

大约一年前，谷歌为其 Pixel 智能手机推出了第一个“像素功能下降”，带来了大量新功能。随着下周一 Android 安全补丁级别的提高，谷歌可能会为其 Pixel 手机推出下一个 Pixel 功能。第五个功能将是新的 Pixel 4a 5G 和 Pixel 5 的第一个功能，我们已经发现了一个名为“自适应声音”的新功能的证据，该功能可以添加到 Pixel 5(很可能也包括 Pixel 4a 5G)。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

**[谷歌 Pixel 4a 5G 论坛](https://forum.xda-developers.com/pixel-4a-5g)**| |**|[谷歌 Pixel 5 论坛](https://forum.xda-developers.com/pixel-5)**

## 自适应声音

在谷歌 2020 Pixel 智能手机上推出的最新版本的设备个性化服务应用程序中，我们为“自适应声音”功能提供了一个新的设置。这不要与谷歌在第二代 Pixel Buds 上提供的同名功能相混淆。虽然该功能会根据环境的噪音水平自动调整音量，但 Pixel 5 的 Adaptive Sound 旨在根据环境的声学特性自动调整声音均衡器设置，从而提高扬声器的音质。

这是我们为该功能提供的设置页面:

这是在那个页面上播放的视频:

https://gfycat.com/ifr/ScarceDesertedAsianporcupine

该视频展示了在家中不同房间如何调节音频(通过描述 7 波段图形均衡器的变化)。有趣的是，谷歌在发布时(h/t @ [siluah](https://twitter.com/siluah/status/1333886756085768193) )显然在其亚马逊商店列表上宣传了 Adaptive Sound(但没有指名道姓)，但在发布后不久，对该功能的引用似乎就被删除了。

我们不确定 Adaptive Sound 何时推出，也不知道它是否会在旧的 Pixel 手机上得到支持。除了 Pixel 5 之外，该功能很有可能也将在 Pixel 4a 5G 上提供，根据功能描述，应该没有任何技术障碍阻止它在运行 Android 11 的旧 Pixel 设备上启用。我们将不得不等待下一个像素功能的下降来找出答案，假设谷歌届时发布该功能。

## 实时字幕改进

我们还在设备个性化服务中发现了新的字符串，表明直播字幕功能将获得一个以前只在现在播放的功能:歌曲识别。当实况字幕检测到正在播放音乐时(实况字幕实际上无法为音乐提供字幕)，字幕似乎不仅仅显示[音乐]，而是实际显示曲目标题和艺术家姓名。

```
 <string name="captions_recognition_full_format">♫ %1$s by %2$s ♫</string>
<string name="captions_recognition_partial_format">♫ %1$s ♫</string> 
```

我们还不能激活这个特殊的功能，但如果我们做到了，我们会更新这篇文章。我们也不知道这种对实时字幕的增强何时推出，但它是未来像素功能下降的另一个可能的竞争者。

* * *

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*