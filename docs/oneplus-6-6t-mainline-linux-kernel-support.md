# OnePlus 6 和一加 6T 看到主线 Linux 内核支持的工作

> 原文：<https://www.xda-developers.com/oneplus-6-6t-mainline-linux-kernel-support/>

# OnePlus 6 和一加 6T 看到主线 Linux 内核支持的工作

一名开发人员正在努力将主流 Linux 内核支持引入 OnePlus 6 和一加 6T。继续阅读，了解更多信息！

购买一加智能手机的好处之一是售后发展支持。该公司通常以其及时的内核源代码发布而闻名(他们在发布源代码方面已经慢了几次),以及为 EOL 设备推广定制 rom 的 T2(T3)等等，这使得它成为开发者社区中的粉丝最爱。我们经常谈论[设备的寿命远远超过他们那一代](https://www.xda-developers.com/samsung-galaxy-s-ii-unofficial-android-11-lineageos-18-1/)，现在看起来两款一加手机即将在第三方开发方面实现类似的非凡壮举。OnePlus 6 系列推出已近三年，但如果你仍有一台 OnePlus 6 或一加 6T，可能很快就可以用主线 Linux 内核启动它。

**[OnePlus 6 论坛](https://forum.xda-developers.com/c/oneplus-6.7609/)| |[一加 6T 论坛](https://forum.xda-developers.com/c/oneplus-6t.8257/)**

有一件事可能会说服许多用户最终放弃他们的旧设备，那就是如果非官方的软件支持在可预见的未来结束——这几乎是几乎每部智能手机都会发生的事情。然而，有一个名为 [Caleb Connolly](https://github.com/calebccff) 的独立开发者，[一直在努力](https://www.reddit.com/r/oneplus/comments/l1ne81/linux_on_the_oneplus_6_and_6t/)将 OnePlus 6 和 6T 包含在主线 Linux 内核中，这必将有助于为这些设备的延长寿命铺平道路。他已经迈出了重要的一步，在 device duo 上成功启动了一个 [postmarketOS](https://www.xda-developers.com/postmarketos-touch-optimized-linux-distro/) 实例。

随着 OnePlus 6/6T 建立在高通骁龙 845 平台之上，上游工作并不太复杂，但主要是为内核添加适当的设备树位。由于[现有的对平台](https://wiki.postmarketos.org/wiki/SDM845_Mainlining)的最小主线支持，像蓝牙、Wi-Fi 和 3D 加速这样的功能已经在当前的开发阶段工作了。更有趣的是，用户甚至可以使用开发者创建的自定义安装程序在 OnePlus 6 和 6T [上双启动 postmarketOS 和 Android。](https://github.com/calebccff/pmos-oneplus6)

**[一加 6 和一加 6T](https://wiki.postmarketos.org/wiki/OnePlus_6_(oneplus-enchilada))T3 的售后服务**

此前，已经有另一家独立开发商为一加 6T 自举 Windows 10 ARM，尽管这并没有引发太多兴趣。现在的情况完全不同，因为 Caleb 一直积极参与内核补丁的上游过程，希望在不久的将来改善那些希望在 OnePlus 6 和 6T 上运行 Linux 的人的情况。我们期待着这些手机的持续发展。