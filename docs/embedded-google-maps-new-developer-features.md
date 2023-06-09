# 嵌入式谷歌地图即将通过新的开发者功能得到改进

> 原文：<https://www.xda-developers.com/embedded-google-maps-new-developer-features/>

# 嵌入式谷歌地图体验将随着新的开发者特性而得到改善

谷歌正在给嵌入式谷歌地图和对 3D 地图的 WebGL 测试版支持注入一些活力。继续阅读，了解更多信息！

每个人都可以通过网站或移动应用程序免费访问谷歌地图，但正如你可能已经注意到的那样，在具有谷歌地图元素的网站和应用程序上，第三方公司和网站/应用程序开发者也可以使用各种可用的 SDK 或 API 之一将谷歌地图视图嵌入到他们自己的应用程序或网页中。这可以更容易地找到商业信息，给用户指路，等等。其中一个 API 是 [Maps JavaScript API](https://developers.google.com/maps/documentation/javascript/overview) ，它旨在供 web 开发人员添加和“使用您自己的内容和图像定制地图，以便在网页和移动设备上显示。”

谷歌根据用户访问该 API 的频率向使用该 API 的网络开发者收费，但对于许多希望在其网站上提供卓越嵌入式地图体验的公司来说，这是值得的。在[谷歌 I/O 2021](https://www.xda-developers.com/tag/google-io-2021/) 上，谷歌[正式推出了](https://cloud.google.com/blog/products/maps-platform/google-maps-platform-announcements-google-io-2021)地图 JavaScript API 的 WebGL 测试版。这一面向开发人员的新特性是向基于云的地图样式转变的一部分，该样式通常适用于 Maps JavaScript API 和 Maps Static API。这使得嵌入式地图比以前更快，更具性能，谷歌表示，他们将提供相同的“高性能，WebGL 加速的地图，你知道从谷歌地图网络体验。”

这也为矢量地图增加了几个新功能，如倾斜和旋转以及 WebGL 叠加视图。前者非常简单:嵌入式地图目前被锁定在一个专门的 2D 方向，通过倾斜和旋转，用户可以以一种全新的视角体验嵌入式地图，倾斜 67.5 度和 360 度旋转，包括建筑物的 3D 模型。然而，后者允许开发人员通过直接链接到用于渲染矢量地图的 WebGL 渲染上下文的生命周期来构建新的制图体验，并允许开发人员直接在底图上渲染二维和三维对象，从而允许他们与地图同时进行渲染。

听起来不错？然后查看官方的 [WebGL codelab](https://goo.gle/maps-platform-webgl-codelab) 和文档，开始使用这些测试版 API。