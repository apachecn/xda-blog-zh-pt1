# 认识一下 Raspberry Pi Pico:一款 4 美元的 ARM 微控制器

> 原文：<https://www.xda-developers.com/raspberry-pi-pico-arm-microcontroller/>

Raspberry Pi 基金会今天宣布了该公司的第一款微控制器 Raspberry Pi Pico。像其他树莓 Pi 产品一样，新的树莓 Pi Pico 价格低廉，仅售 4 美元，但它采用了基金会的第一个定制芯片:RP2040。

[在设计 RP2040](https://www.raspberrypi.org/blog/raspberry-pi-silicon-pico-now-on-sale/) 的时候，树莓派基金会给自己定了三个目标。他们希望芯片具有处理整数工作负载的高性能，具有支持大多数外部设备的灵活 I/O 选项，并且成本低廉，以降低准入门槛。他们设计的尺寸为 2 平方毫米，采用 40 纳米工艺节点制造，具有双核 ARM Cortex-M0+处理器和 264KB 片内 RAM。7x7 毫米 QFN-56 封装中还包含多个 I/O 选项、2MB 闪存、支持 1.8-5.5V 输入电压的电源芯片、一个按钮和一个 LED。

**RP2040 规格**

*   双核 Arm Cortex-M0+ @ 133MHz
*   264KB(还记得千字节吗？)的片内 RAM
*   通过专用 QSPI 总线支持高达 16MB 的片外闪存
*   DMA 控制器
*   插值器和整数分频器外设
*   30 个 GPIO 引脚，其中 4 个可用作模拟输入
*   2×UART、2 × SPI 控制器和 2 × I2C 控制器
*   16 × PWM 通道
*   1 × USB 1.1 控制器和 PHY，支持主机和设备
*   8 × Raspberry Pi 可编程 I/O (PIO)状态机
*   支持 UF2 的 USB 大容量存储引导模式，用于拖放编程

Raspberry Pi Pico 可在 C/C++和 MicroPython 中编程，Raspberry Pi Foundation 正在提供完整的 C SDK、基于 GCC 的工具链和 Visual Studio 代码集成。有趣的是，如果你有兴趣在 Pico 上运行任何机器学习程序，甚至还有一个 TensorFlow Lite 的[端口可用。](https://github.com/raspberrypi/pico-tflmicro)

售价 4 美元，配有 RP2040 芯片的 Raspberry Pi Pico 有很多功能。如果你想在家里建立一个简单的项目来控制你的电器，Pi Pico 似乎是一个简单而廉价的进入微控制器编程的方法。

您可以从 Raspberry Pi 基金会的网站查看该板的完整规格、数据表、引脚排列图、片上启动 ROM 和其他文档[。覆盆子 Pi 基金会也](https://www.raspberrypi.org/documentation/pico/getting-started/)[出了一本书](https://www.raspberrypi.org/products/micropython-pico/)来教初学者如何在新的 Pi Pico 上开始使用 MicroPython。从今天开始，您可以从所有 Raspberry Pi 认可的经销商处购买 Raspberry Pi Pico 微控制器和这本书。如果你是 *HackSpace* 杂志的订户，你会得到一份免费的 Pico】二月号。

### 树莓派皮可

Raspberry Pi Pico 是一款 4 美元的微控制器板，采用 Raspberry 内部基于 ARM 的 RP2040 芯片。它可以用 C 和 MicroPython 编程，具有 I2C、SPI 和 PIO 等 I/O 选项。

**Affiliate Links**

Raspberry Pi

[View at Raspberrypi.org](https://www.raspberrypi.org/products/raspberry-pi-pico/)

或者，您也可以从 Adafruit、Arduino、Pimoroni 或 Sparkfun 购买一款采用 RP2040 芯片平台的低成本电路板。