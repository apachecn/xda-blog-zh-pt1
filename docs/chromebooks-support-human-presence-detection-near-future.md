# 在不久的将来，Chromebooks 可能会支持人类存在检测

> 原文：<https://www.xda-developers.com/chromebooks-support-human-presence-detection-near-future/>

根据 Chromium Gerritt 最近的承诺[，Chromebooks 可能很快就会支持人类存在检测和面部识别。谷歌正致力于在 Chrome OS 上添加与人感传感器相关的代码，类似于一些 Windows 笔记本电脑已经提供的功能。信息被](https://chromium-review.googlesource.com/c/chromiumos/platform2/+/2834916)[T3 9 到 5 GoogleT5 发现。](https://9to5google.com/2021/09/03/google-human-presence-sensor-chromebook-face-unlock/)

人类存在传感器并不一定保证 Chromebooks 会支持面部识别，但这两个功能往往是相辅相成的。如果你看看支持人类存在检测的 Windows 笔记本电脑，它通常是 Windows Hello 的一个插件。人感传感器的作用是让电脑在用户走近时被唤醒。然后，Windows Hello 摄像头可以识别用户并解锁 PC，所有这些都不需要用户的直接交互。这使得它甚至比指纹传感器更方便。人感传感器也可以以另一种方式工作，当您离开电脑时，它会自动锁定电脑。

在谷歌的提交中还发现了更多的信息。该功能似乎处于开发的早期阶段，但如果 Chromebook 具有人类存在检测功能，它会在系统托盘中显示一个图标。目前，图标是静态的，但它可以改变，以表明有人被检测到，甚至可能警告用户有人从后面接近他们。

谷歌正在与专用硬件合作，在其测试中运行人类存在检测，特别是来自 Lattice Semiconductor 的 CrossLink NX LIFCL-17。该公司还与蚂蚁金服合作，尽可能利用开源软件来利用硬件。

最后，测试还指向了谷歌正在测试的一些设备。谷歌发现了谷歌在代号为 [Brya](https://chromium-review.googlesource.com/c/chromiumos/overlays/board-overlays/+/3138678) 和 [Zork](https://chromium-review.googlesource.com/c/chromiumos/platform2/+/3128009) 的设备上测试这项功能的证据。Zork 是 AMD 驱动的 Chromebooks 的通用代号，但 Brya 特指采用英特尔第 12 代[“Alder Lake”处理器](https://www.xda-developers.com/intel-shares-details-alder-lake-chips-coming-this-fall/)的笔记本电脑。发现这一点的代码更改后来被标记为放弃，并替换为另一个不太具体的版本。

目前还没有明确的迹象表明具有人体感应功能的 Chromebooks 何时会出现。代码更改确实指向这是非常早期的工作，所以它可能需要一段时间才能实现。同样不清楚的是，人类存在检测的增加是否计划与类似 Windows Hello 的面部识别一起进行，尽管这似乎是最有意义的。