# 以下是如何启动微软自己的 Linux 发行版:CBL 水手

> 原文：<https://www.xda-developers.com/boot-cbl-mariner-microsoft-linux-distribution/>

距离微软[发布其 Linux Windows 子系统的第二个版本](https://www.xda-developers.com/microsoft-announces-windows-terminal/)已经有几年了，现在运行时已经足够成熟，可以[用 GUI 运行 Linux 应用程序](https://www.xda-developers.com/run-gui-linux-apps-windows-10-wsl/)。旅程的下一步不是别人，正是 Android 的 [Windows 子系统](https://www.xda-developers.com/wundows-subsystem-android-benchmarks-solid-performance/)，它将让你[在 Windows 11](https://www.xda-developers.com/windows-11-android-apps/) 下运行 Android 应用。微软对 Linux 的热爱不止于此，因为该公司也一直在维护一个成熟的 Linux 发行版。该发行版被称为 CBL-马里纳(其中 CBL 代表 Linux 操作系统),由微软的 Linux 系统小组开发，该小组开发了用于 WSL 2 的 Linux 内核。

> #### “CBL 水手是微软的云基础设施和边缘产品和服务的内部 Linux 发行版。CBL-水手旨在为这些设备和服务提供一个一致的平台，并将增强微软保持 Linux 更新的能力。”
> 
> #### -微软

值得注意的是，CBL 水手不是一个传统的以用户为中心的 Linux 发行版，它有一个奇特的 GUI。相反，它只有支持和运行容器所需的基本包。包管理系统是基于 RPM 的，它同时使用了`dnf`和`tdnf` ( [小 DNF](https://github.com/vmware/tdnf) )。该发行版还支持基于映像的更新机制，使用 [RPM-OSTree](https://rpm-ostree.readthedocs.io/en/stable/) 进行原子服务和回滚。至于安全性，CBL 水手号附带了一个加固的内核、签名更新、ASLR、基于编译器的加固和防篡改日志等许多其他功能。

* * *

## 如何启动 CBL 水手使用官方 ISO

尽管微软早在 2020 年就发布了该操作系统，但该公司最初并没有提供预编译的 ISOs。GitHub 上有源代码[，人们希望](https://github.com/microsoft/CBL-Mariner)[自己构建 ISO](https://blog.jreypo.io/2021/07/09/a-look-into-cbl-mariner-microsoft-internal-linux-distribution/) 。这种情况最近有所改变，因为微软现在在其服务器上托管官方的 CBL-水手 ISO 版本。

虽然有经验的用户仍然可以从 CBL-水手软件包库中预编译的 rpm 创建可引导的 VHDX(或 VHD)映像，但也可以获取 ISO 格式的安装盘映像，并在虚拟化平台或真实 PC 上轻松安装操作系统。

### 步骤 1–获取 ISO

CBL 水手 ISO 是 UEFI 兼容的，可以在任何现代 x86-64 PC 上引导。最新版本的 ISO 可从以下链接下载:

**[下载 CBL 水手 ISO](https://aka.ms/mariner-1.0-x86_64-iso)**

如果您想自己构建 ISO，请执行以下操作:

1.  使用 git 克隆 CBL-水手 GitHub repo:

    ```
     git clone https: 
    ```

2.  切换到工具箱文件夹:

    ```
     cd CBL-Mariner/toolkit 
    ```

3.  执行 ISO 编译命令:

    ```
     sudo make iso REBUILD_TOOLS=y REBUILD_PACKAGES=n CONFIG_FILE=./imageconfigs/full.json 
    ```

4.  产生的 ISO 可以在`../out/images/full`中找到。

### 步骤 2–准备目标平台

如前所述，CBL 水手并不意味着是一个日常驱动你的电脑操作系统。最好将其安装在虚拟机管理程序平台上。在 Windows 上，您可以使用微软自己的 Hyper-v。[Oracle VM VirtualBox](https://www.virtualbox.org/)是另一个跨平台解决方案，可以在 Windows、Linux 以及 macOS 上使用。根据主机操作系统，您也可以选择合适的 VMware 或 [Parallels](https://www.xda-developers.com/parallels-17-mac-review/) 虚拟化产品。

在本教程中，为了方便起见，我们将使用 Hyper-V。

1.  由于 Hyper-V 是作为一个可选功能内置到 Windows 中的，我们需要先[启用它](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v)。家庭和家庭单一语言 SKU 不正式支持 Hyper-V，但有可能使用[本教程](https://www.xda-developers.com/how-to-install-hyper-v-windows-11-home/)在那些版本上启用该功能。
2.  打开 Hyper-V Manager 应用程序，选择*操作- >新建- >虚拟机*。给你的虚拟机起个名字，然后按*下一步>T3。*
3.  选择*第 1 代* (VHD)或*第 2 代* (VHDX)，然后按*下一个>* 。
4.  如果需要，更改内存大小，然后按下*下一个>T1。*
5.  选择一个虚拟交换机，然后按*下一个>T1。*
6.  选择*创建虚拟硬盘*，为您的 VHD(X)选择一个位置，并设置您想要的磁盘大小。然后按下*下一个>T3。*
7.  选择*从可引导镜像文件*安装操作系统，并浏览至您的 CBL 水手 ISO。
8.  按*结束*。

如果您已经创建了第 2 代虚拟机，那么您必须配置几个附加设置:

1.  在 Hyper-V 管理器中右键单击您的虚拟机。
2.  选择*设置...*选项。
3.  选择*安全*，在*模板*下:选择*微软 UEFI 认证机构*。
4.  选择*固件*并调整引导顺序，使 DVD 优先，硬盘其次。
5.  选择*应用*应用所有更改。

### 步骤 3–安装操作系统

现在我们已经准备好了平台，我们准备在虚拟机上安装 CBL 水手。

1.  右键单击您的虚拟机并选择*连接...*开始引导的选项。
2.  选择*开始*。
3.  安装应用程序将给出以文本或图形模式继续的选项。在本教程中，我们将选择后者。
4.  有两种安装类型:核心安装和完全安装。
5.  在选择您想要的风格后，它会询问您典型的参数，如用户名、分区等。
6.  安装完成后，选择重新启动以重新启动机器。安装 ISO 将自动弹出。

### 步骤 4–启动操作系统

一旦安装阶段结束，虚拟机将重新启动，并随后开始从虚拟硬盘引导新安装的操作系统。出现提示时，使用通过安装程序应用程序提供的用户名和密码登录到您的 CBL 水手实例。

* * *

就是这样！您现在可以添加额外的包，如 SSH 服务器，并根据您的需要定制 VM 实例。更多关于它的安全特性，请看一下 [CBL 水手的 GitHub 安全特性列表](https://github.com/microsoft/CBL-Mariner/blob/1.0/toolkit/docs/security/security-features.md)。