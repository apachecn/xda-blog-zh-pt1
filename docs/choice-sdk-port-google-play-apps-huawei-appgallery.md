# 这个新的 SDK 使得将应用移植到华为设备变得更加容易

> 原文：<https://www.xda-developers.com/choice-sdk-port-google-play-apps-huawei-appgallery/>

华为多年来一直在建立自己的应用生态系统，在谷歌的应用和服务被切断后，该公司的努力进一步加强。华为生态系统的一个重要组成部分是华为的应用商店 [AppGallery](https://www.xda-developers.com/appgallery-huawei-alternative-google-play-store-android/) ，但将应用程序带到没有谷歌移动服务的手机上并不总是容易的。幸运的是，新的 SDK 旨在解决这个问题。

Choice SDK 主要由总部位于 T2 的 BlueSource 开发，它为应用程序提供了一个单一的界面，可以与谷歌移动服务/Firebase 或华为移动服务进行交互，无论是用户手机上的哪一个。开发者不必为华为设备和谷歌设备维护两个独立的代码库，或者自己为两个平台编写所有代码，而是可以拥有一个在两个平台上都能工作的代码库。这并不是一个即插即用的解决方案，因为开发人员仍然需要用 Choice SDK 的等价物来替换特定于 GMS 的调用，但这比其他选择要简单。

Choice SDK 最初是由 BlueSource 创建的，用于将银行应用程序移植到华为设备上，但根据该项目，Choice SDK 现在被“多个商业、公共和私人运营的应用程序”使用。它支持 GMS 和 HMS 的分析、定位、地图绘制、消息传递和登录功能，并且代码是开源的。

Choice SDK 是否会导致移植到华为手机上的流行应用增多，还有待观察。跨多个应用商店维护应用程序本身就是一个困难的过程，美国仍然施加的贸易限制意味着许多潜在的开发者不能合法地与华为合作。Play Store 上的许多[当前热门应用，目前包括脸书、Discord 和 Facebook Messenger 等应用，都是由美国公司开发的。然而，对于能够并愿意将应用程序引入华为手机的开发者来说，新的 SDK 可以节省一些时间。](https://play.google.com/store/apps/collection/cluster?clp=0g4jCiEKG3RvcHNlbGxpbmdfZnJlZV9BUFBMSUNBVElPThAHGAM%3D:S:ANO1ljKs-KA&gsr=CibSDiMKIQobdG9wc2VsbGluZ19mcmVlX0FQUExJQ0FUSU9OEAcYAw%3D%3D:S:ANO1ljL40zU)