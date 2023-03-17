# 现在很容易绕过联发科的 SP Flash 工具认证

> 原文：<https://www.xda-developers.com/bypass-mediatek-sp-flash-tool-authentication-requirement/>

采用联发科芯片组的设备有一个 BROM(引导只读存储器)，它通常会加载预加载程序可执行文件，然后引导 Android 系统，但也包含一种称为下载模式的替代引导模式。它严格用于 OEM 服务，可用于解除设备锁定，就像[高通的紧急下载模式(EDL)](https://www.xda-developers.com/how-to-unbrick-oneplus-nord-msmdownloadtool/) 。联发科制造的一个名为“SP 闪存工具”的专有程序可以利用这个接口来强制闪存设备上的系统软件。由于低级下载模式有效地完全控制了设备的存储，包括小米和 Realme 在内的许多原始设备制造商[已经开始混淆闪烁过程](https://www.xda-developers.com/xiaomi-edl-unbrick-authorized-mi-accounts/)。由于这种做法，通过下载模式进行固件刷新只能由相应 OEM 授权的签名“下载代理”程序执行，这基本上意味着**除非获得设备制造商的许可，否则您不能刷新或解锁自己的智能手机**。

好了，XDA 了不起的开发者社区再次来拯救我们了。基于最初由 XDA 资深成员 [xyz`](https://forum.xda-developers.com/m/xyz.9667509/) 发现的[一个引导 ROM 漏洞](https://github.com/amonet-kamakiri/kamakiri)，开发者 [Dinolek](https://forum.xda-developers.com/m/6296775/) 和 [k4y0z](https://forum.xda-developers.com/m/k4y0z.7104332/) 提出了一种通用的旁路方法，它与各种各样的联发科驱动的设备兼容，否则这些设备在闪存时需要认证。该方法利用特定于 SoC 的漏洞有效载荷，拦截 SP 闪存工具发出的预闪存查询，并强行将两个关键参数(“串行链路认证”和“下载代理认证”)的值设置为假，以便在没有任何授权的情况下继续闪存过程。

* * *

值得注意的是，漏洞有效载荷需要一个专门调整的 USB 驱动程序才能成功拦截。如果你运行的是 Windows，你必须安装一个基于 libusb 的过滤驱动来覆盖默认的驱动设置。另一方面，Linux 用户需要[对内核应用特定的补丁](https://github.com/amonet-kamakiri/kamakiri/blob/master/kernel.patch)。如果你不想接触你的主操作系统，你可以使用[FireISO](https://github.com/amonet-kamakiri/fireiso/releases)——一个专门为此目的设计的可引导 GNU/Linux ISO。

当访问联发科下载模式时，你只需要关闭目标设备，按住音量增大按钮(小米手机音量减小)，然后将手机插入 PC。您应该会在设备管理器(Windows)或`dmesg | grep usb` (Linux)的输出中看到一个新的串行设备。

此时，按照这个简单的 5 步过程禁用 bootrom 保护:

1.  下载安装 [Python](https://www.python.org/downloads/) 。出现提示时，Windows 用户应该选择“将 Python X.X 添加到路径中”。
2.  使用`pip` :

    ```
     pip install pyusb pyserial json5 
    ```

    安装所需的依赖项
3.  [下载旁路实用程序](https://github.com/MTK-bypass/bypass_utility/releases)。
4.  解压存档，执行实用程序，在联发科下载模式下连接手机。您应该在日志末尾看到“保护已禁用”。
    *   视窗:

        ```
         python main.py 
        ```

    *   Linux:

        ```
         ./main.py 
        ```

5.  之后，在不断开手机的情况下，在 UART 连接模式下运行 SP Flash Tool。

就是这样！验证程序被绕过，你现在可以刷新/解锁你的手机了。如果更有经验的人希望更进一步，他们可以刷新修改过的分区备份来修复拙劣的 IMEI，但这超出了本文的范围。

以下是目前支持的 SOC 列表。理论上讲，旁路方法在其他联发科芯片组上的工作方式是相同的，但需要有人先编写一个合适的有效载荷来禁用 bootrom 保护例程。

### 支持的 SOC 列表

*   mt6261
*   mt6572
*   mt6580
*   mt6582
*   mt6735
*   mt6737
*   mt6739
*   mt6755
*   mt6757
*   mt6761
*   mt6763
*   mt6765
*   mt6768
*   mt6771
*   mt6785
*   mt6799
*   mt6873
*   mt8127
*   mt8163
*   mt8173
*   mt8695

## 结论

如果你还记得，联发科芯片组之前在近一年前被发现容易受到危险的 rootkit 的攻击[，它被黑客积极利用来获得 root 访问权限](https://www.xda-developers.com/mediatek-su-rootkit-exploit/)。考虑到这一点，不知道这家台湾芯片设计公司为什么还没有修补其芯片组中的缺陷，该缺陷允许在闪烁时击败信任链。虽然我们只看到了情况好的一面，但从安全角度来看，当你考虑到数百种不太知名的设备型号使用这些联发科芯片时，情况就更糟了。

从定制开发社区的角度来看，这种情况还有另外一个方面，我们代表了他们的利益。大多数联发科设备发现自己处于一种不可持续的组合中，即容易制造又难以复兴。最重要的是，强制授权要求确实限制了它们的售后市场发展潜力。对于联发科设备所有者来说，旁路方法只不过是一线希望，他们只想摆脱与取消绑定相关的麻烦。

对探索 bypass 方法的代码库感兴趣的人应该看看下面的 GitHub 链接。您还可以通过访问[讨论线程](https://forum.xda-developers.com/t/mod-dev-mediatek-mtk-auth-bypass-sla-daa-utility.4232377/)与开发人员互动。

**[联发科 SP Flash 工具认证绕过 GitHub 回购](https://github.com/MTK-bypass/bypass_utility)**