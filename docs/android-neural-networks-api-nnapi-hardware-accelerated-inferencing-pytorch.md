# Android 的 NNAPI 现在支持 PyTorch 的硬件加速

> 原文：<https://www.xda-developers.com/android-neural-networks-api-nnapi-hardware-accelerated-inferencing-pytorch/>

# Android 的神经网络 API 现在支持脸书 PyTorch 框架的硬件加速推理

Android 的神经网络 API (NNAPI)现在支持脸书 PyTorch 框架的硬件加速推理。请继续阅读了解更多信息！

机器学习在许多方面塑造了我们的现在，以至于我们甚至不再注意到它。以前不可能完成的任务现在已经变得轻而易举，使得这项技术及其好处能够更广泛地为大众所接受。很多这一切都是通过设备上的机器学习和谷歌的神经网络 API (NNAPI)实现的。现在，随着 Android 团队宣布支持一个原型功能，使开发人员能够通过脸书的 PyTorch 框架使用硬件加速推理，更多的用户将能够体验到加速神经网络及其好处。

设备上的机器学习允许机器学习模型在设备上本地运行，而不需要将数据传输到服务器，从而实现更低的延迟、更好的隐私性和更好的连接性。Android 神经网络 API (NNAPI)旨在为 Android 设备上的机器学习运行计算密集型操作。NNAPI 提供了一组 API，以从可用的硬件加速器(包括 GPU、DSP 和 npu)中获益。

NNAPI 可以通过 Android C API 直接访问，也可以通过更高级别的框架访问，比如 [TensorFlow Lite](https://www.xda-developers.com/tensorflow-lite-mobile-gpu-android/) 。根据今天的公告， [PyTorch Mobile](https://ai.facebook.com/tools/pytorch/) 宣布了一个支持 NNAPI 的新原型功能，从而使开发人员能够在 PyTorch 框架中使用硬件加速推理。这个初始版本包括对 Android 10 及以上版本上众所周知的线性卷积和多层感知器模型的支持。使用 MobileNetV2 模型进行的性能测试显示，与单线程 CPU 相比，速度提高了 10 倍。作为向完全稳定版本发展的一部分，未来的更新将包括对其他操作符和模型架构的支持，包括 Mask R-CNN，一种流行的对象检测和实例分割模型。

或许在 PyTorch 之上构建的最知名的软件是特斯拉的自动驾驶软件。虽然今天的公告没有为 Autopilot 带来任何直接消息，但它确实为数百万使用基于 PyTorch 构建的软件的 Android 用户开放了加速神经网络的好处。