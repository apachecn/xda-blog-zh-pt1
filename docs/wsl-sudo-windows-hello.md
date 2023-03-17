# WSL Hello sudo 为 Linux 的 Windows 子系统带来了 Windows Hello 身份验证

> 原文：<https://www.xda-developers.com/wsl-sudo-windows-hello/>

Linux 的 Windows 子系统(WSL)是 Windows 10 的重要组成部分。WSL 最初是为开发人员构建 web 和云应用程序而设计的，如今它变成了一种更强大的东西，将两种截然不同的操作系统结合在一起。自 [WSL 2](https://www.xda-developers.com/microsoft-windows-10-may-2020-update-wsl-2-revamped-cortana-assistant-your-phone-calls-arm-devices/) 以来，Linux 层由微软 Hyper-V 虚拟化技术的变体提供支持，并且它配备了微软编译和支持的 Linux 内核。WSL 和底层 Windows 10 之间的集成非常灵活，人们可以很容易地从 Linux 命令行运行 Windows 工具，反之亦然。

但是乐趣并没有就此结束。修补者经常想出一些 mods，向你展示 Linux 的 Windows 子系统有多强大，如果你愿意跳出框框思考的话。如果您一直渴望一些非常棒的 WSL 调整，那么这篇文章就是为您准备的。认识一下“WSL Hello sudo”——这是一个开源实用程序，允许您使用 Windows Hello 生物认证(通过 [*Liliputing*](https://liliputing.com/2021/03/wsl-hello-sudo-brings-biometric-authentication-to-windows-subsystem-for-linux-commands.html) )在 Linux 实例中认证 [sudo 命令](https://www.xda-developers.com/linux-update-sudo-security-flaw/)。

Takaya 佐伯，一个化名为的日本软件开发者，是这个令人敬畏的项目背后的大脑。如上面的动画所示，WSL Hello sudo 可以用熟悉的 Windows Hello 界面无缝地替换密码输入提示，允许您使用面部、指纹或 PIN 来验证 sudo 请求。

WSL Hello sudo 由两个特定于操作系统的组件组成:Linux 端的一个[可插拔认证模块](https://en.wikipedia.org/wiki/Pluggable_authentication_module) (PAM)和一个负责调用 Windows Hello 的配套 Windows 应用程序。PAM 模块负责将 Linux 用户的认证请求映射到相应的 Windows 10 用户的 Windows Hello 签名。得益于这样的模块化设计，WSL Hello sudo 同时兼容 Linux 和 WSL 2 的第一代 Windows 子系统。

设置 WSL Hello sudo 相当简单。你需要做的就是[下载预编译的二进制文件](https://github.com/nullpo-head/WSL-Hello-sudo/releases)，在 Linux 的 Windows 子系统下执行`install.sh`脚本，然后经历典型的 PAM 模块配置过程。如果您在设置时有任何问题，我们建议您查看项目自述文件的[故障排除部分](https://github.com/nullpo-head/WSL-Hello-sudo#troubleshooting)。

**[WSL 你好 sudo GitHub 回购](https://github.com/nullpo-head/WSL-Hello-sudo)**