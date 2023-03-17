# 本周在 Chrome OS: Chrome 的材质更新

> 原文：<https://www.xda-developers.com/this-week-in-chrome-os-chromes-material-update/>

休息一周后我们回来了。上周，三星几乎主导了科技新闻，所以关于 Chrome 没有太多可说的。让我们看看 Chrome OS 中的本周。本周我们有几个有趣的 Chromium 提交来检查即将到来的特性。Chrome 浏览器不仅在设计上有所改变，Chrome OS 还增加了一些有用的新功能，以更好地与 Android 集成。

还有一些新的 Chromebook 硬件发布和泄露，特别是在惠普方面。我们预计这一趋势将在下个月左右继续，因为我们正处于返校季。我们将讨论一些即将推出的设备，并预览可能会出现的其他设备。我还会简单介绍一下我的华硕 Chromebook CX9 评测，以及与 Galaxy Chromebook 2 的对比。

我决定稍微调整一下专栏的格式，这样你就可以找到你想看的东西了。展望未来，我们将以即将到来的 Chrome 功能/更新开始，转向硬件发布，然后以任何不属于任何其他地方的随机部分结束。我们开始吧。

## 即将推出的 Chrome 操作系统功能/更新

### Chrome 的材料改造

我们都知道谷歌在 Android 12 中努力改进材料设计，所以他们在其他产品中继续这些努力是有道理的。最初是由[肯特·杜克在 Android Police](https://www.androidpolice.com/2021/08/19/chrome-is-getting-a-fresh-material-makeover-for-its-system-pages/) 发现的，Chrome 浏览器正在进行材料改造，减少蓝色口音。

这个新的 Chromium Gerrit commit 为 Chrome 的偏好设置、书签、下载、扩展和历史添加了样式更新。您可以通过使用标志来启用更改:

**chrome:flags # webui-branding-update**

这个标志似乎主要影响了 Chrome 中灯光主题的风格。如果你使用的是黑暗模式，变化就不那么明显了。黑暗模式下的对比度稍高，但远不如明亮主题中从蓝色到白色的变化明显。

### Android 应用程序中的邻近共享集成

Chrome OS 与 Android 的集成越来越好。在 Chrome 操作系统中，已经可以在你的 Android 手机上接收所有的通知和信息。现在，谷歌正准备在 Android 应用程序中添加 Chrome OS Nearby Share。

我们最初在本周早些时候发现了这个 Chromium Gerrit commit。该承诺表明，附近的共享正在 Android 应用程序中进行测试。似乎开发者已经在 Hatch 和 Eve Chrome 平台上测试了这些功能。显然，这将使你在 Android 手机上与附近的 Chromebook 分享内容更加方便。在应用程序中添加共享选项也将鼓励用户更经常地使用附近的共享，因为它目前还不太容易使用。

我们不确定 Android 应用程序何时会提供附近共享，但我们肯定会密切关注这一发展中的功能。

在另一个有趣的 Gerrit 承诺中，Chrome OS 似乎将很快获得一个 Windows 风格的菜单来控制窗口位置。这个[提交很少涉及细节](https://chromium-review.googlesource.com/c/chromium/src/+/3098927)，因为这是新特性的第一次提交。我们希望它看起来像下面的 Windows 菜单。

很明显，这个特性将使用 Chrome 标志进行测试，所以我们最终将有机会测试它。这是一个受欢迎的功能，因为 Chrome OS 对于控制和重新定位窗口来说不是最直观的。我们将继续关注更多的进展。

## 本周在 Chrome OS:硬件

### 惠普开发阿尔德湖 c1030

我们在 Chrome Unboxed 的朋友发现了[惠普正在研发](https://chromeunboxed.com/hp-chromebook-x360-13c-c1030-12th-gen-intel-alder-lake)奥尔德湖版本的 Chromebook c1030 的证据。这个硬件发现也是通过检查 Chromium 提交来实现的。新的奥尔德湖模型内部代号为 Redrix。

我们知道这将是对 c1030 的更新，承诺表明这两款设备具有相同的设计。这非常令人兴奋，因为 c1030 是目前最好的 Chromebooks 之一。对老化处理器的更新会受到许多惠普粉丝的欢迎。

### 面向 2021 年更新的 HP Pro c640

惠普 Chromebook Pro c640 最近被更新为 2021 年。您可以获得更新的第 11 代英特尔处理器，价格也更低，为 849 美元。这不是一个明显的升级，但价格下降幅度很大。Pro c640 的 2020 型号售价超过 1000 美元，即使对于企业设备来说也很贵。

如果你是一个企业客户，这是一个坚实的内部升级。这个版本还没有更新，最初的昏暗显示(250 尼特)似乎也没有任何改进。尽管如此，从性能角度来看，Tiger Lake 芯片和 Iris Xe 显卡无疑使这款设备令人印象深刻。

### 华硕推出面向教育的加固型可拆卸产品

华硕发布了全新[华硕 Chromebook 可拆卸 CZ1](https://www.asus.com/Laptops/For-Students/Chromebook/ASUS-Chromebook-Detachable-CZ1-CZ1000/) 的登陆页面。除了新的加固改进之外，这款设备与华硕 Chromebook CM3 可拆卸设备相同。这对于教育部门来说是一个明显的趋势，耐用的橡胶装饰和 3D 纹理便于抓握。

在内部，华硕 Chromebook CZ1 采用了与 CM3 和联想 Duet 相同的联发科 Kompanio 500。它还配有 4GB 内存和 64GB 或 128 GB eMMC 两种存储版本。它拥有相同的 1920 x 1200，16:10 显示屏，garaged 触控笔和一个 USB-C 端口。你还可以得到一个 3.5 毫米的耳机插孔，这是联想 Duet 所不包括的。

CZ1 的一个好处是在购买价格中包含了一个键盘套。许多可拆卸设备都有可选的键盘外壳，但对于教育设备来说，在购买时看到盒子里的所有东西是很棒的。键盘外壳还配有触摸板，这是华硕从以前的可拆卸键盘中省略的东西。目前还没有定价，但这看起来是一款适合 K-12 学生的伟大设备。

## 本周在 Chrome 操作系统:随机位

我鼓励每个人都来看看我对华硕 Chromebook CX9 的全面评论，这绝对是目前金钱可以买到的最好的 Chromebook。我还与 [CX9 和 Galaxy Chromebook 2](https://www.xda-developers.com/asus-chromebook-cx9-vs-samsung-galaxy-chromebook-2/) 进行了全面的比较，这两款设备在许多方面都很相似。目前，CX9 已经取代 Galaxy Chromebook 2 成为我日常使用的首选 Chromebook，这主要归功于键盘。

随着 Borealis 成为 Chrome OS 的现实越来越近，希望我们将开始听到更多关于 Chrome OS 上 Vulkan 支持的信息。在那之前，应该会有很多有趣的硬件出现。我个人希望谷歌会给所有人带来惊喜，并在 10 月份发布 Pixelbook Go 继任者。让我知道你想在新的 Pixelbook 中看到什么。