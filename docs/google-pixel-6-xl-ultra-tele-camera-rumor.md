# 谷歌相机暗示 Pixel 6 XL 可能有一个 5X“超远程”相机

> 原文：<https://www.xda-developers.com/google-pixel-6-xl-ultra-tele-camera-rumor/>

今天早些时候，谷歌为 Pixel 手机推出了 Android 12 的第三个测试版。最新的测试版增加了新功能，如滚动屏幕截图，更智能的自动旋转，以及我们正在开发的许多其他功能。除了新功能，还有更新的系统应用程序，最值得注意的是新的壁纸拾取器和新的谷歌相机应用程序。后者更新到了版本 8.3.252，这是对之前版本 8.2.400 的一个显著改进。从表面上看，新的谷歌摄像头更新似乎只支持 Android 12 的动态主题系统。然而，在 APK 内，我们发现了证据表明 [Pixel 6](https://www.xda-developers.com/google-pixel-6/) XL(或“Pro”)可能拥有 5X 变焦“超远距离”相机。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

著名的谷歌相机改装师和 XDA 资深会员 [cstark27](https://forum.xda-developers.com/m/cstark27.2712580/) 在谷歌相机应用的缩放 UI 的布局文件中发现了一个新行。我们在下面嵌入的新行的 id 为“zoom_toggle_ultratele ”,文本为“5x ”,表明取景器中将显示新的 5X 变焦选项。

```
 <TextView android:textSize="@dimen/zoom_toggle_button_text_size" android:textColor="@color/zoom_toggle_bar_text_color" android:gravity="center" android:layout_gravity="right|center_vertical|center_horizontal|center" android: android:clickable="false" android:layout_width="@dimen/zoom_toggle_unselected_button_size" android:layout_height="@dimen/zoom_toggle_unselected_button_size" android:text="<strong>5x</strong>" android:includeFontPadding="false" android:fontFamily="@font/google_sans_text_medium" android:textAlignment="center"/> 
```

深入挖掘谷歌相机应用程序，我们发现了一些关于新的“ultratele”变焦开关的参考资料。虽然没有找到直接的证据将“ultratele”变焦切换与传闻中 Pixel 6 XL/Pro 的代号“raven”联系起来，但开发者 cstark27 发现了长焦相机“真实”光学变焦水平可能是 4.3 倍的证据。作为参考，Pixel 4 的“真实”光学变焦水平是 1.6 倍，尽管谷歌相机应用程序显示 2 倍作为一个选项。Cstark27 还发现，超广角相机的变焦水平与 Pixel 4a 5G 和 Pixel 5 略有不同，具体来说，现在是 0.615 倍，而不是 0.670 倍。

上周，乔恩·普罗瑟[泄露了 Pixel 6 系列的规格](https://www.xda-developers.com/google-pixel-6-five-years-updates/)。泄露的消息表明，较小的 Pixel 6 将有一个 50MP 宽和 12MP 超广角的双后置摄像头设置，而较大的 Pixel 6 XL/Pro 将有一个 50MP 宽的三后置摄像头设置，由 48MP 长焦和 12MP 超广角组成。之前有传言称谷歌将为其 Pixel 6 系列设备之一采用潜望式长焦镜头，当然，[泄露的 CAD 渲染图](https://www.xda-developers.com/google-pixel-6-renders-premium-flagship/)似乎证实了这种可能性。从谷歌在 I/O 2021 上分享的视频中捕捉到的谷歌相机应用程序 UI 的静态图像也指向该应用程序获得 5X 变焦选项，但今天的应用程序更新是指向新 5X“ultra tele”变焦选项的第一个确凿证据。

随着今年秋季晚些时候 Pixel 6 系列发布日期的临近，我们可能会了解更多关于这两款设备的相机设置和功能的信息。新的证据表明，这款手机将被命名为 Pixel 6 XL，而不是 Pixel 6 Pro。

特色图片致谢:OnLeaks 和 91Mobiles。感谢 PNF 软件为我们提供了使用*[JEB Decompiler](https://www.pnfsoftware.com/?aid=xdadev)**的许可，这是一款针对 Android 应用的专业级逆向工程工具。*