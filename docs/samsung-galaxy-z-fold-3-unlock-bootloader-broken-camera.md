# 三星 Galaxy Z Fold 3 的摄像头在解锁 bootloader 后损坏

> 原文：<https://www.xda-developers.com/samsung-galaxy-z-fold-3-unlock-bootloader-broken-camera/>

[三星 Galaxy Z Fold 3](https://www.xda-developers.com/samsung-galaxy-z-fold-3/) 和[三星 Galaxy Z Flip 3](https://www.xda-developers.com/samsung-galaxy-z-flip-3/) 代表了三星能够为其消费者提供的最佳可折叠技术。不用说，如果你现在想买一部高端智能手机，最新的 Galaxy Z 系列肯定会把[列在你的清单](https://www.xda-developers.com/galaxy-z-flip-3-z-fold-3-pre-orders/)中，作为一个可能的购买选择。虽然硬件和软件组合使这些设备对大多数买家来说都很棒，但高级用户和发烧友可能仍然需要解锁引导加载程序并启动这些设备，以释放他们的真正潜力。不幸的是，三星已经使得在不触发安全标志的情况下[获得 root 访问权限](https://www.xda-developers.com/root/)变得极其困难，现在韩国 OEM 为售后市场的发展引入了又一个路障。在最新的举措中，三星在你解锁 bootloader 后禁用了 Galaxy Z Fold 3 上的摄像头。

**[三星 Galaxy Z Fold 3 回顾(上)——科技的未来，在我们眼皮底下展开](https://www.xda-developers.com/samsung-galaxy-z-fold-3-review/)**

Knox 是三星设备上的安全套件，对设备的任何修改都会使其跳闸，使您的保修无效，并永久禁用 Samsung Pay。现在，失去所有与 Knox 相关的安全功能是一回事，但不得不处理一个坏掉的摄像头是许多人不愿意做出的权衡。但如果你想解锁 Galaxy Z Fold 3 上的引导程序，这正是你必须处理的问题。

According to XDA Senior Members [白い熊](https://forum.xda-developers.com/m/i.4237286/) and [ianmacd](https://forum.xda-developers.com/m/ianmacd.7187684/), the final confirmation screen during the bootloader unlock process on the Galaxy Z Fold 3 mentions that the operation will cause the camera to be disabled. Upon booting up with an unlocked bootloader, the stock camera app indeed fails to operate, and all camera-related functions [cease to function](https://forum.xda-developers.com/posts/85522359), meaning that you can't use facial recognition either. Anything that uses any of the cameras will time out after a while and give errors or just remain dark, including third-party camera apps.

##### *感谢 XDA 资深会员 [ianmacd](https://forum.xda-developers.com/m/ianmacd.7187684/) 提供的图片！*

目前还不清楚为什么三星选择了过去索尼走过的路，但实际问题在于，许多人可能会忽略警告并解锁引导加载程序，而不知道这一新的限制。重新锁定 bootloader 确实能让相机重新工作，这说明更多的是软件层面的障碍。使用 root 访问权限，可以检测和修改引导加载程序发送给操作系统的负责参数，从而绕过这一限制。然而，根据 *ianmacd* , [Magisk](https://www.xda-developers.com/how-to-install-magisk/) 在其默认状态下不足以绕过障碍。

**[三星 Galaxy Z 折 3 XDA 论坛](https://forum.xda-developers.com/f/samsung-galaxy-z-fold3.12349/)**

Galaxy Z Flip 3 可能也有类似的限制，但这种情况尚未得到证实。我们将随时向您更新三星引导加载程序解锁政策的任何变化。

 <picture>![The Galaxy Z Fold 3 may be a year old, but it's still very capable, and right now on Amazon, it can be had for below $1,000, making it quite a good deal. ](img/be980991d336ee214d081964c43bd3f2.png)</picture> 

Samsung Galaxy Z Fold 3

##### 三星 Galaxy Z Fold 3

Galaxy Z Fold 3 是三星最新、最棒的可折叠手机。与之前的型号相比，它带来了几项改进，包括高刷新率显示器、屏幕下摄像头和顶级硬件。