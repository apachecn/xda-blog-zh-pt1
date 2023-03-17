# 这个第三方库将 Android 12 的素材应用到任何应用程序中

> 原文：<https://www.xda-developers.com/android-12-material-you-dynamic-theming-library/>

[Material You](https://www.xda-developers.com/material-you/) 是 Google 设计语言的最新版本。对于 Material You，谷歌强调个性化，这就是为什么在 [Android 12](https://www.xda-developers.com/android-12/) 中，有一个新的动态主题化系统，它使用从你的壁纸中提取的颜色[给你的 UX 重新着色。这个代号为“monet”的动态主题系统](https://www.xda-developers.com/android-12-wallpaper-theme/)[在 Android 12 Beta 2](https://www.xda-developers.com/android-12-beta-2-features/) 中上线，但谷歌尚未记录 API/实现，提供支持库，或开放 Google Play 来发布针对 API level 31 (Android 12)的应用程序，因此绝大多数开发人员甚至没有考虑过调整他们的应用程序来支持动态主题系统。

然而，这并不意味着没有开发者在玩弄 Android 12 的主题系统。[流行自动化应用 Tasker](https://www.xda-developers.com/tasker-android-12-material-you/) 的开发者使用 Android 12 的官方 API 在其应用中演示了动态主题化支持。另一方面，另一个开发者，kdrag0n，[使用他自己的颜色提取和调色板生成算法重新创建了完整的系统](https://www.xda-developers.com/android-12-material-you-theming-system-recreated/)。Kdrag0n 分享了他的主题引擎的源代码，并正在开发一个 Jetpack Compose 和 Flutter 库，以便为旧版本操作系统构建的第三方应用程序可以实现他对“莫奈”的理解。

现在，XDA 公认的开发者 Quinny899 创建了自己的库，该库基于 kdrag0n 的自定义“monet”实现(即是基于谷歌主题引擎的*而不是*。开发人员可以将这个 MonetCompat 库集成到他们的应用程序中，以添加对基于用户壁纸的应用程序 UI 动态主题化的支持。这个库在运行 Android 5.0 及以上版本(在兼容模式下使用调色板 API)和 Android 8.1 Oreo 及以上版本的设备上正常工作。由于平台 API 的限制，该库无法从 Android 8.1 之前版本的动态壁纸中提取颜色。

至于为什么一个开发者可能想要使用这个库，Quinny899 自己在该项目的 GitHub 页面上解释道。“目前还不知道谷歌是否会在 Android 12 发布时为 Monet 提供自己的向后兼容库，所以这个库最终可能会被官方库取代。在这个项目中没有使用专有的谷歌代码，因此它被麻省理工学院许可在第三方应用程序中使用。"

第一个使用 MonetCompat 的应用当然是 Quinny899 自己的 DarQ 应用。DarQ 是一个应用程序，可以让你在每个应用程序的基础上切换 Android 的强制黑暗模式设置。它最初使用 root 访问权限来设置系统属性，但被 T2 更新为使用运行在用户电脑上的 ADB shell 脚本，放弃了 root 要求。在 DarQ 2.0 中，用户不再需要从他们的 PC 上运行 ADB 脚本，因为该应用程序现在集成了[滴](https://github.com/RikkaApps/Shizuku)。滴是一个应用程序和服务，让其他应用程序运行 shell 命令或访问具有亚行 shell 用户权限的 APIs 请将其视为超级用户管理应用程序，但用于亚行 shell 访问。在 Android 11+上，可以通过内置的无线调试功能启动滴服务，因此您不再需要一台 PC 来设置 DarQ。随着迁移到滴，DarQ 现在也使用 ProcessObserver 而不是 AccessibilityService，开发者说这让 DarQ 可以更快地检测到应用程序何时打开(从而应用强制黑暗设置)。

如果出于任何原因，你不喜欢 MonetCompat 为 DarQ 应用程序生成的颜色，你可以点击“DarQ 2.0”三次，以启用应用程序中的开发者选项。在这里，您可以选择“莫奈颜色选择器”来更改您希望应用程序使用的颜色。

### DarQ 2.0 变更日志

*   DarQ 2.0 有一个全新的设计，材料你元素和莫奈(基于壁纸)的颜色。
*   亚行的脚本现在已经不存在了，取而代之的是滴在非根设备上处理服务。如果你不知道滴是什么，就把它想象成非根设备的超级用户应用程序。每次开机在电脑上(甚至在 Android 11 及以上版本的手机上)通过 ADB 启动滴一次，任何使用滴的 app 都可以使用 ADB 服务。
*   使用滴/根服务，可访问性服务已被 ProcessObserver 取代。这比可访问性快得多，所以以前打开太快而不受支持的应用程序现在可以工作了。
*   改进了日出/日落时的自动黑暗主题，以便在不同的设备上更好地工作。
*   对试图阻止使用黑暗力量的应用程序的 Xposed 模块进行了改进，防止他们这样做。

**[DarQ XDA 论坛线程](https://forum.xda-developers.com/t/app-root-shizuku-10-27-jun-darq-per-app-selectable-force-dark-option-for-android-10.3944356/)**| |**|[GitHub 上的 MonetCompat 库](https://github.com/KieronQuinn/MonetCompat/wiki)**