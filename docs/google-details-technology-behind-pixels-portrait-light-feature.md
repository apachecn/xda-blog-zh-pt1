# 谷歌详细介绍了 Pixel 人像灯功能背后的技术

> 原文：<https://www.xda-developers.com/google-details-technology-behind-pixels-portrait-light-feature/>

在经历了几次泄露和传言之后，谷歌终于在今年 9 月初发布了 Pixel 5 和 Pixel 4a 5G。正如预期的那样，这些设备配备了一系列新的谷歌摄像头功能，使其有别于市场上的其他安卓手机。这些功能包括用于视频无抖动平移的电影平移、锁定和主动稳定模式、人像模式下的夜视支持以及自动调整人像拍摄照明的人像灯光功能。发布几周后，谷歌通过谷歌照片更新为[老款 Pixel 设备](https://www.xda-developers.com/google-pixel-5-portrait-light-feature-rolls-out-older-pixel-phones/)发布了大部分这些功能。现在，该公司分享了一些关于人像灯功能背后的技术细节。

根据该公司最近的一篇博文,人像灯功能的灵感来自人像摄影师使用的离机灯。它通过模拟可以添加到场景中的可重新定位的光源来增强人像拍摄。自动添加时，人工光源会使用机器学习自动调整方向和强度，以补充照片的现有照明。

正如谷歌解释的那样，该功能利用了新的机器学习模型，这些模型是使用在[灯光舞台](https://augmentedperception.github.io/therelightables/)计算照明系统中捕获的多样化照片数据集进行训练的。这些模型支持两种算法能力:

*   自动定向光放置:基于机器学习算法，该功能自动放置人工光源，与专业摄影师在现实世界中放置相机外光源的方式一致。
*   合成后捕捉重新照明:基于人像拍摄中现有光线的方向和强度，机器学习算法添加了看起来真实自然的合成光线。

对于自动定向光放置，谷歌训练了一个机器学习模型来估计一个[高动态范围](https://en.wikipedia.org/wiki/High-dynamic-range_imaging)，基于输入肖像的场景的全向照明轮廓。这种新的[光照估计模型](https://augmentedperception.github.io/facelight/)可以发现场景中来自所有方向的所有光源的方向、相对强度和颜色，将人脸视为一个[光探头](https://www.pauldebevec.com/Probes/)。它还使用 [MediaPipe 面网格](https://google.github.io/mediapipe/solutions/face_mesh.html)估计对象的头柱。基于上述数据，算法然后确定合成光的方向。

一旦建立了合成照明的方向和强度，下一个机器学习模型就会将合成光源添加到原始照片中。第二个模型使用数百万对肖像进行训练，包括有无额外灯光。该数据集是通过使用 Light Stage 计算照明系统拍摄 70 个不同的人而生成的，该系统是一个球形照明装置，包括 64 个具有不同视点的摄像机和 331 个单独可编程的 LED 光源。

70 名受试者中的每一个都是在被 331 个发光二极管中的每一个一次一盏灯(OLAT)照明时被拍摄的。这产生了它们的[反射场](http://www.pauldebevec.com/Research/LS)，即它们的外观被球形环境的离散部分照亮。反射场对受试者的皮肤、头发和衣服的独特颜色和反光属性进行了编码，并确定了每种材料在照片中的光泽或暗淡程度。

然后，这些 OLAT 图像被线性添加在一起，以呈现对象的真实图像，就像它们出现在任何基于[图像的照明环境](https://en.wikipedia.org/wiki/Image-based_lighting)中一样，正确地呈现了复杂的光传输现象，如[次表面散射](https://en.wikipedia.org/wiki/Subsurface_scattering)。

然后，谷歌没有训练机器学习算法直接预测输出 relit 图像，而是训练模型输出低分辨率的[商图像](https://wwwee.ee.bgu.ac.il/~rrtammy/Publications/qimage-cvpr99.pdf)，该商图像可以应用于原始输入图像，以产生所需的输出。该方法在计算上是高效的，并且仅鼓励低频照明变化，而不影响直接从输入图像转移的高频图像细节，以保持质量。

此外，谷歌训练了一个机器学习模型，以模拟光源从相对粗糙的表面反射的光学行为。为了做到这一点，该公司训练该模型在给定输入照片的情况下估计表面法线，然后应用[朗伯定律](https://en.wikipedia.org/wiki/Lambert%27s_cosine_law)计算出所需照明方向的“光可见性地图”。然后，将该光可见度图作为输入提供给商图像预测器，以确保使用基于物理学的见解来训练该模型。

虽然这一切看起来似乎是一个漫长的过程，需要 Pixel 5 的中端硬件花费相当多的时间来处理，但谷歌声称，人像灯功能已经过优化，可以在移动设备上以交互式帧率运行，总模型大小不到 10MB。