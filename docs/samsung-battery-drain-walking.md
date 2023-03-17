# 您的 Galaxy S21 Ultra 的电池可能会因为走动而耗尽

> 原文：<https://www.xda-developers.com/samsung-battery-drain-walking/>

一些三星智能手机可能正在遭受一种奇怪的错误，每当你四处走动时，它就会耗尽电池。原因未经证实，但在我们的论坛上发现，[它可能是由相机唤醒锁引起的](https://forum.xda-developers.com/t/cameraservice_worker-partial-wakelock.4234161/)，当手机在运动时，相机唤醒锁会阻止手机的相机传感器发出嘎嘎声。我的同事 Zachary Wander 调查了这是否是他自己的三星 Galaxy Note 20 Ultra 电池耗尽问题的原因，但更多的用户报告说 Galaxy S21 Ultra 出现了电池耗尽问题。

光学图像稳定用于拍照，特别是在弱光下，以防止手机相机的传感器抖动太多，并持续收集光线。OIS 在相机外壳内移动相机，这意味着几乎每部装有 OIS 的手机都会在震动时发出嘎嘎声。看起来，作为 OIS 使用的抖动检测的一部分，相机应用程序可能会在检测到运动时唤醒设备(通过[](https://www.sammobile.com/news/walking-around-may-be-draining-galaxy-s21-ultra-battery)**)*。正如 Zachary Wander 在他的 Twitter 帖子中提到的[，三星似乎没有在设备运动时释放保持相机传感器的唤醒锁，导致后台电池耗尽。](https://twitter.com/Wander1236/status/1404815770140524552)*

 *一些可能受到影响的手机包括 Galaxy S21 Ultra 和 Galaxy Note 20 Ultra，但其他手机也可能受到影响。也有可能这个问题实际上与相机在运动中保持稳定无关，电池耗尽问题背后有一个完全不同的原因。

原因可能是什么还不知道，如果你受到影响，我们看到的避免这种电池消耗的唯一方法是尽可能少地移动你的手机。当你在家里走动时，把它放在桌子上似乎是避免不必要的电池消耗的最佳方式，这显然不是任何人的理想解决方案。希望三星可以很快解决这个问题，因为这不是该公司第一次在软件更新中引入问题。

我们已经联系了三星，看看他们是否意识到这个问题，如果有回音，我们会更新这篇文章。如果你想知道你的手机是否受到影响，你可以在 GSam 电池监控器或 [BetterBatteryStats](https://forum.xda-developers.com/t/app-2-2-05-oct-v2-4-betterbatterystats.1179809/) 等应用中寻找 cameraservice_worker wakelock。对于一些用户来说，这种唤醒锁已经导致电池在 7 小时内耗尽 20%以上，所以如果它影响到你的设备，它可能会很明显。遗憾的是，没有 root 用户就无法切换这项服务，但即使你可以，也建议你不要这样做，因为这可能会产生意想不到的后果。

*特色图片:三星 Galaxy S21 Ultra*

*本文于美国东部时间 16:00 更新，增加了关于唤醒锁的更多信息。**