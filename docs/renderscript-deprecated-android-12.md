# Android 12 反对 GPU 计算任务的 RenderScript API

> 原文：<https://www.xda-developers.com/renderscript-deprecated-android-12/>

# Android 12 反对 GPU 计算任务的 RenderScript API

谷歌宣布，即将发布的 Android 12 版本将淘汰 RenderScript，这是一种用于运行计算密集型代码的 API。

谷歌在 Android 3.0 Honeycomb 中引入了 RenderScript API，用于需要在 CPU 或 GPU 上运行高性能工作负载的应用程序，而不使用 NDK 或 GPU 专用的 API。随着 NDK 工具的改进，使用 OpenCL 的 GPU 计算，Vulkan API 的引入，以及在 Android SDK 和 NDK 代码之间共享位图硬件缓冲区的能力，谷歌决定在 [Android 12](https://www.xda-developers.com/android-12/) 中弃用 RenderScript APIs。

正如在 Android 开发者博客上解释的那样，谷歌不再推荐对性能要求很高的任务使用 RenderScript。相反，需要在 GPU 硬件上运行的高性能工作负载应该迁移到跨平台的 Vulkan API。谷歌提供了一个[样本应用](https://github.com/android/renderscript-samples/tree/main/RenderScriptMigrationSample/)，展示了两个 RenderScript 脚本及其 Vulkan 等价物。如果您的应用程序需要在旧设备上工作，您可能需要管理两条代码路径:一条使用 RS 用于旧设备，另一条使用 Vulkan 用于新设备。

对于那些将 RS 用于其高性能图像操作功能集的应用程序，如 blur，谷歌[提供了一个 Android 库](https://github.com/android/renderscript-intrinsics-replacement-toolkit)，取代了大多数被否决的内部函数。虽然这些 API 将继续在 Android 12 上运行，但谷歌表示，在针对该版本编译 RS 代码时会发出警告。