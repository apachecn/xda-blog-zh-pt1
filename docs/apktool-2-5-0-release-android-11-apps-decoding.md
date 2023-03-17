# Apktool v2.5.0 增加了对为 Android 11 构建的解码应用程序的更好支持

> 原文：<https://www.xda-developers.com/apktool-2-5-0-release-android-11-apps-decoding/>

# Apktool v2.5.0 增加了对为 Android 11 构建的解码应用程序的更好支持

Apktool，曾经流行的 Android APK 逆向工程工具，已经到了 2.5.0 版本，有很多修复和 Android 11 相关的改进。

如果您对逆向工程 Android 应用程序感兴趣，那么“Apktool”这个名字应该听起来耳熟。由 Connor Tumbleson(又名 XDA 公认的开发者)维护，这个开源工具允许你反汇编 Android 应用程序二进制(被称为 APK)文件，改变一些东西，并重建它们。在经历了一段[开发停顿](https://www.xda-developers.com/apktool-2-4-release/)之后，Apktool 现在已经更新到 2.5.0 版本，新的标题特性是“Android 11 支持”

为了在 Android 11 上显著简化事情，Apktool 的 [smali/baksmali 后端](https://github.com/JesusFreke/smali)需要升级。最新的版本不仅解决了这个问题，还提供了必要的框架更新。错误记录模块也进行了改进，这样用户就可以在更短的时间内完成更多的工作，而不用担心破译神秘的错误信息。此外，此次更新还为 Android 资产打包工具(aapt/aapt2)带来了大量补丁，以提高 macOS 兼容性，并将编译期间崩溃的可能性降至最低。

您可以查看以下更新的完整变更日志:

*   [ [#2399](https://github.com/iBotPeaches/Apktool/issues/2399) ， [#2397](https://github.com/iBotPeaches/Apktool/issues/2397) ， [#2369](https://github.com/iBotPeaches/Apktool/issues/2369) ， [#2167](https://github.com/iBotPeaches/Apktool/issues/2167) ] Android 11 支持。
*   [ [#2006](https://github.com/iBotPeaches/Apktool/issues/2006) ， [#1718](https://github.com/iBotPeaches/Apktool/issues/1718) ]将 smali/baksmali 升级到 v2.4.0
*   [ [#2110](https://github.com/iBotPeaches/Apktool/issues/2210) ， [#2053](https://github.com/iBotPeaches/Apktool/issues/2053) ]弃用 32 位操作系统。
*   [ [#2251](https://github.com/iBotPeaches/Apktool/issues/2251) ]修复二进制名称冲突导致的线程崩溃。
*   [ [#2323](https://github.com/iBotPeaches/Apktool/issues/2323) ]在`resources.arsc`上固定压缩。
*   [ [#2333](https://github.com/iBotPeaches/Apktool/issues/2333) ]修复压缩时空文件崩溃的问题。(感谢佩雷特)
*   [ [#2328](https://github.com/iBotPeaches/Apktool/issues/2328) ， [#2364](https://github.com/iBotPeaches/Apktool/issues/2364) ]修复 aapt2 的调试模式处理。(感谢 Comnir)
*   [ [#2386](https://github.com/iBotPeaches/Apktool/issues/2386) ， [#2217](https://github.com/iBotPeaches/Apktool/issues/2271) ， [#2119](https://github.com/iBotPeaches/Apktool/issues/2119) ]修复处理名称中带有`$`的 XML 文件。
*   [ [#2300](https://github.com/iBotPeaches/Apktool/issues/2300) ]修复 NPE 在反汇编没有资源匹配 resId 的清单时的问题。
*   [ [#2438](https://github.com/iBotPeaches/Apktool/issues/2438) ， [#1903](https://github.com/iBotPeaches/Apktool/issues/1903) ]修复 aapt2 的伪属性 bool(false)为 ref(null)。
*   [ [#2317](https://github.com/iBotPeaches/Apktool/issues/2317) ， [#2188](https://github.com/iBotPeaches/Apktool/issues/2188) ， [#1859](https://github.com/iBotPeaches/Apktool/issues/1859) ]修复混淆清单中的非标准名称空间。
*   [ [#1945](https://github.com/iBotPeaches/Apktool/issues/1945) ， [#2146](https://github.com/iBotPeaches/Apktool/issues/2146) ]修复 NPE 在寻找缺失资源的参照时的问题。
*   [ [#2343](https://github.com/iBotPeaches/Apktool/issues/2343) ]修复框架目录无法写入时的错误消息。
*   [ [#2411](https://github.com/iBotPeaches/Apktool/issues/2411) ]为`classes[1-3].dex`增加测试
*   [ [#1913](https://github.com/iBotPeaches/Apktool/issues/1913) ]增加了新的列表框架命令。
*   [ [#2368](https://github.com/iBotPeaches/Apktool/issues/2368) 增加了对`compileSdkVersion`的支持。
*   更新了响应代码，以便在传递无效参数时正确地非零。(感谢 Giszmo)
*   更新了许可证标题，以反映项目的开始日期并删除 javadoc 样式。(感谢 friederbluemle)
*   增加了对 Windows 助手脚本中`JAVA_HOME`变量的支持。(感谢 vldmrrr)
*   增加了对 SDK 代码名称“S”的支持
*   升级到 gradle 6.4.1
*   用 GitHub 动作替换了 TravisCI

如果您还没有更新，请使用下面的链接下载最新版本，并查看[安装说明](https://ibotpeaches.github.io/Apktool/install/)了解更多详细信息。在我们的论坛上还有一个[专用支持线程](https://forum.xda-developers.com/t/util-apktool-tool-for-reverse-engineering-apk-files.1755243/)来获取更多信息。

**下载 apk tool:[GitHub](https://github.com/iBotPeaches/Apktool/releases/latest)| |[bit bucket](https://bitbucket.org/iBotPeaches/apktool/downloads/)**

* * *

**来源:[康纳·唐伯森的博客](https://connortumbleson.com/2020/12/02/apktool-v2-5-0-released/)**