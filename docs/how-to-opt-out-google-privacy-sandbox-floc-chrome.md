# 如何在 Chrome 中退出谷歌的隐私沙箱(FLoC)

> 原文：<https://www.xda-developers.com/how-to-opt-out-google-privacy-sandbox-floc-chrome/>

在线广告目前依赖于第三方“cookies”，这是一种在不同网站上跟随你的小标识符。Cookies 允许公司跟踪你的浏览活动并创建广告档案，这就是为什么许多以隐私为中心的网络浏览器(如 Firefox 和 Vivaldi)在很大程度上[阻止它们](https://www.xda-developers.com/firefox-android-enhanced-tracking-protection-block-redirect-tracking/)。谷歌 Chrome 仍然允许 cookies 不受限制地工作，但现在谷歌正在研究一种新技术来取代它们:群体联合学习(FLoC)。

然而，新技术仍然依赖于(不太准确的)行为跟踪，其他一些浏览器已经决定他们不会实现 FLoC。也可以在 Chrome 中关闭 FLoC，谷歌称之为隐私沙箱。那么，FloC 到底是什么，怎么关掉？

## 什么是絮状物？

[群体联合学习(FLoC)](https://www.xda-developers.com/duckduckgo-brave-and-vivaldi-will-block-googles-floc/) 是谷歌 Chrome 正在测试的一项新功能，它允许在不使用跨站点跟踪 cookies 的情况下进行定向广告。FLoC 查看您的浏览历史，并根据您的行为将您放入广告定位组。该技术旨在比跨站点跟踪 cookies 更隐私，因为不再有个人配置文件(只针对群体)，但它仍因默认启用和允许其他类型的跟踪而受到批评。

出版商和广告商正在犹豫要不要告别跨站点跟踪 cookies，几乎所有其他已经屏蔽跟踪器的网络浏览器都承诺禁用 FLoC。Vivaldi Browser 写了[一篇博客文章](https://vivaldi.com/blog/no-google-vivaldi-users-will-not-get-floced/)批评该功能:

> 在 Vivaldi，我们捍卫用户的隐私权。我们不赞成任何形式的跟踪和侧写。我们当然不会允许我们的产品建立本地跟踪档案。
> 
> 对我们来说，“隐私”这个词意味着真正的隐私。我们不会把它扭曲成对立面。我们甚至没有观察您如何使用我们的产品。我们的隐私政策简单明了；我们不想跟踪你。

火狐浏览器的开发者 Mozilla 在一份声明中表示，目前还没有在火狐浏览器中实现 FLoC 的计划:

> 我们目前正在评估许多隐私保护广告提案，包括谷歌提出的提案，但目前没有实施任何提案的计划。[...广告和隐私可以共存。广告业的运作方式可能会与过去几年有所不同。我们期待在寻找建设更好网站的解决方案中发挥作用。

微软和苹果仍在决定未来是否将 FLoC 引入他们的浏览器——目前 Safari 中还没有，微软已经在 Edge 中关闭了它。

## 如何退出隐私沙盒

在网络上保持隐私的最佳方式是使用不属于广告公司的浏览器，但如果你出于这样或那样的原因不得不坚持使用 Chrome，谷歌确实提供了关闭 Chrome 中 FLoC 的设置(至少目前是这样)。在 Android 上的 Chrome 中，打开主菜单，然后进入**设置>隐私和安全>隐私沙箱**。

在桌面 Chrome 浏览器中，将**Chrome://settings/privacy sandbox**粘贴到地址栏中，按回车键即可找到设置。该设置应该与您的 Google 帐户同步，因此如果您在一台设备上关闭它，FLoC 也会在您的其他设备上关闭。

如果你根本看不到任何设置，那么你的浏览器或账户还没有启用 FLoC，所以你没什么好担心的。