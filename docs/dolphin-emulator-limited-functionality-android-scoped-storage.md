# Dolphin 模拟器开发人员警告说，由于 Android 的范围存储变化，功能有限

> 原文：<https://www.xda-developers.com/dolphin-emulator-limited-functionality-android-scoped-storage/>

Android 的范围存储规则一直是应用程序开发者争论的焦点。虽然作用域存储无疑需要减少应用程序对用户私人文件的访问，但它的实现从根本上改变了应用程序访问手机内部存储的方式，在此过程中为各种应用程序带来了一些限制。例如，Dolphin Emulator 是任天堂 GameCube 和 Wii 最受欢迎的开源模拟器，该模拟器的开发者现在警告说，由于 Android 11 中引入的范围存储变化，该模拟器将提供有限的功能。

在 Dolphin[2020 年 12 月和 2021 年 1 月的进度报告](https://dolphin-emu.org/blog/2021/02/11/dolphin-progress-report-december-2020-and-january-2021/#50-13386-use-storage-access-framework-scoped-storage-for-the-gamelist-on-android-by-josjuice:~:text=5.0%2D13386)中，开发者强调了 Android 的范围存储变化将如何限制模拟器的功能。它指出，由于存储访问框架 API 的[性能不佳，游戏列表加载时间增加了十倍以上。虽然这不会影响实际的仿真性能，但会影响用户体验。此外，API 的局限性将迫使开发者放弃一些功能，比如为 Wii NAND 定制路径。](https://www.xda-developers.com/android-q-storage-access-framework-scoped-storage/)

这是不幸的，因为我们的许多用户喜欢利用多个 NANDs，由于 Wii 的严格空间限制，仿真不能轻易绕过。目前，我们正计划使用一个单一的预设 Wii NAND 目录来绕过对作用域存储的需求。虽然这意味着没有性能问题，但它确实意味着 Android 用户将被锁定使用单一的 Wii NAND。报告补充道:“它还必须使用设备的内部存储，”。

这些变化将对安卓电视用户产生更加不利的影响。报告指出，虽然 Dolphin 模拟器的文件选择器在一些设备上工作，但模拟器用来选择游戏目录的文件夹选择器[在 Android TV](https://commonsware.com/blog/2017/12/27/storage-access-framework-missing-action.html) 上完全损坏。由于这一点，运行 Android 11 的 Android 电视设备将完全无法使用 Dolphin 的游戏列表功能。然而，运行旧版本 Android 的设备将继续使用旧版本的文件夹选择器。像 NVIDIA 的 [SHIELD TV](https://www.xda-developers.com/tag/nvidia-shield-tv/) 这样运行 Android 9 或更老版本的设备不会受到这些变化的影响，Dolphin 的游戏列表将继续正常工作，直到它们更新到 Android 11。

此外，由于 Dolphin Emulator 目前针对的是 Android 10 SDK，因此其开发人员已经慢慢实现了对存储访问框架 API 的支持，而不会被迫在可能导致问题的领域使用它。但到 2021 年 11 月，开发者将被迫遵守存储访问框架 API，以便发布 Google Play 的更新，这将彻底改变 Android 11 用户的情况。令人欣慰的是，虽然这些变化会在一些方面对用户体验产生负面影响，但核心仿真体验不会受到影响。

正如您所料，这些问题不仅限于模拟器。第三方文件管理器也受到范围存储变化的影响，Google now [要求开发者提交一个表单](https://www.xda-developers.com/google-file-manager-devs-submit-form-broad-file-storage-access-android-11/)以获得 Android 11 中广泛的文件存储访问。即使拥有广泛的文件存储访问权限，文件管理人员也不再能够访问某些外部存储目录。因此，修改 Android 游戏不再那么容易了。