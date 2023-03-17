# 记事本++ v8 更新带来了黑暗模式支持和 ARM64 版本

> 原文：<https://www.xda-developers.com/notepad-update-dark-mode-support-arm64-build/>

# 记事本++ v8 更新带来了黑暗模式支持和 ARM64 版本

最新的 Notepad++更新(v8)带来了新的黑暗模式、无干扰模式、原生 ARM64 支持等等。

Notepad++毫无疑问是最流行的 Windows 源代码编辑器之一。它提供了各种有用的功能，如选项卡式编辑、语法高亮、代码折叠等，使其成为全球用户的首选。尽管它的用户界面已经过时，Notepad++在过去的几年里仍然是粉丝们的最爱。随着它的最新更新，它一定会吸引更多的用户。

Notepad++开发者 Don Ho 发布了开源软件的 v8 版本，并带来了一些值得注意的新功能。对于初学者来说，编辑器现在有一个原生的黑暗模式。它有一个稍微更现代的用户界面，这要归功于工具栏中可选的流畅用户界面图标，这是一个新的无干扰模式，它现在也可以在 ARM64 Windows 设备上运行。除了这些新特性，Notepad++ v8 还带来了许多错误修复和改进。请在下面的部分查看完整的 changelog 以了解更多信息。

### 记事本++ v8 变更日志

*   加入黑暗模式。
*   提供 ARM64 版本。
*   用 Scintilla 静态库和 Boost RegExpr 头文件构建 Notepad++。
*   为工具栏添加新的流畅用户界面图标。
*   添加新功能“分心自由模式”
*   为黑暗模式添加新的 API NPPM _ ADDTOOLBARICON _ FORDARKMODE
*   在关闭按钮上添加一次单击动作(SHIFT-click ),关闭可停靠面板中的所有选项卡
*   增加改变选择文本前景色的能力(可选)。
*   更换后允许更换停止(可选)。
*   修复附加扩展功能在保存对话框中不起作用。
*   增加颠倒生产线顺序的能力。
*   增加了只设计当前文本样式的功能。
*   修复自动完成弹出窗口中的重复条目。
*   修正了 Python 函数列表在某些情况下不显示函数的问题。
*   批量添加/删除文件时，增强文件夹作为工作区的性能。
*   在函数列表中添加 Ada，Fortran，Fortran77 & Haskell。
*   改进搜索结果中“全部打开”命令的性能。
*   将“复制路径名”命令添加到搜索结果上下文菜单中。
*   捕捉正则表达式搜索异常并显示异常消息。
*   为大小写和单词添加 MarkAll 首选项设置。
*   修复回归:在打开/保存文件对话框中正确处理“默认目录”设置。
*   修复 UTF16 文件崩溃问题(回归)中的一个特殊字符。
*   添加“附加扩展名”复选框到另存为对话框。
*   搜索结果中的修复复制命令可用，因为没有选择。
*   在编辑区域添加填充功能。
*   使新选项卡名称可翻译。
*   改进正则表达式中的字符大小写处理。
*   修复拖出来的 UDL 文件不适用于新实例中的 UDL。
*   添加用于将指定字符串添加到应用程序标题栏的命令行参数。
*   修复忽略大小写的自动完成问题。
*   修复了正则表达式搜索中启用的“全字匹配”选项。
*   使用出现在制表符后的列键选择修复排序。
*   修复“重新加载工作区”菜单命令不工作的问题。
*   如果名称包含空格，修复 Edge 浏览器中的视图文件失败问题。
*   增加避免累积多个搜索结果的能力。
*   修复 U+FFFF 以上代码点的 UTF-16 解码/编码。
*   修复“另存为”命令从最近文件历史记录中删除原始路径的问题。
*   修复功能列表按钮工具提示混淆的问题。
*   从 Notepad++中删除 Microsoft Bing，因为它的可靠性很差。

如果你想尝试这些新功能，你可以点击[这个链接](https://notepad-plus-plus.org/downloads/v8/)下载最新的 Notepad++版本。如果您的设备上已经安装了旧版本，它应该会在几天内自动更新。