# 您现在可以使用 Magisk 对 Galaxy S21、Galaxy S21 Plus 和 Galaxy S21 Ultra 进行 root 操作

> 原文：<https://www.xda-developers.com/samsung-galaxy-s21-series-rooted-magisk/>

# 三星的 Galaxy S21 系列现在可以用 Magisk 做根了

现在，您可以使用 Magisk 为您的 Galaxy S21、Galaxy S21 Plus 和 Galaxy S21 Ultra 设置根目录。请点击帖子中的链接获取说明。

Galaxy S21 系列代表了三星今年的最佳阵容。阵容中的三款设备都采用了来自[三星](https://www.xda-developers.com/tag/exynos-2100/)和[高通](https://www.xda-developers.com/tag/qualcomm-snapdragon-888/)的旗舰处理器、出色的相机硬件、大电池和漂亮的显示屏。最重要的是，他们运行三星最新的基于 Android 11 的 One UI 版本，该版本释放了大量新功能。虽然硬件和软件的结合使 Galaxy S21 系列对大多数买家来说都很棒，但高级用户和发烧友可能仍然需要扎根于这些设备，以释放他们的真正潜力。谢天谢地，现在你可以用最新的 Magisk Canary 版本做到这一点。

Magisk 背后的开发者、XDA 资深公认开发者和贡献者 [topjohnwu](https://forum.xda-developers.com/m/topjohnwu.4470081/) 已经成功地将 Galaxy S21 设备的 Exynos 和骁龙变种植入了 root。开发者在最近的一条推文中宣布了同样的消息，其中包括一张展示 Galaxy S21 Ultra rooted 与 Magisk 的截图。

如前所述，Magisk 在最新的 Canary 版本中获得了对 Galaxy S21 系列的支持。根据 Magisk 论坛上发布的[变更日志，该版本包括:](https://forum.xda-developers.com/t/magisk-general-support-discussion.3432382/post-84493077)

*   [常规] Magisk 和 Magisk 管理器现在合并了！
*   [应用]将应用“Magisk 管理器”重命名为“Magisk”
*   [App]支持在 Android 5.0+上隐藏具有高级技术(存根 APK 加载)的 Magisk 应用程序(以前是 9.0+)
*   [App]不允许在低于 Android 5.0 的设备上重新打包 Magisk 应用程序
*   [magis hide]修复了一个当停止 magis hide 不起作用时的 bug
*   [MagiskBoot]修复了解包 lz4_lg 压缩启动镜像时的 bug
*   [MagiskInit]支持 Galaxy S21 系列
*   [MagiskSU]修复导致 libsqlite.so 无法加载的不正确 APEX 路径

正如 [topjohnwu 指出的](https://twitter.com/topjohnwu/status/1360785783481724930)对 Exynos Galaxy S21 的支持要感谢[这个补丁](https://github.com/topjohnwu/Magisk/commit/501bc9f438de4d11d7a9530cb0ce3393c954eb6e)，它已经被合并到 Magisk Canary 分支。值得注意的是，到目前为止，只有 Exynos 和香港骁龙 Galaxy S21 设备可以解锁引导程序，因此这种根方法将只适用于这些变种。如果你想 root 你的 Galaxy S21 设备，你可以按照[这个线程](https://forum.xda-developers.com/t/magisk-root-for-the-galaxy-s21-series-b-n-0-models-only.4233567/#post-84493857)中提到的步骤开始。如果你遇到任何问题，你可以在项目的 [GitHub 库](https://github.com/topjohnwu/Magisk/issues)上提交一份错误报告。