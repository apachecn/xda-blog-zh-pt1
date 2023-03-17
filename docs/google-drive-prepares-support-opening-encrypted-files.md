# Google Drive 准备增加打开加密文件的支持

> 原文：<https://www.xda-developers.com/google-drive-prepares-support-opening-encrypted-files/>

**更新 1 (11/10/2020 @ 11:28 ET):** 一名线人透露了更多关于 Google Drive 文件加密/解密功能的信息。[点击这里了解更多信息。今天早些时候发表的这篇文章保留在下面。](#update1)

谷歌似乎正准备推出一项功能，允许用户下载和打开加密文件。在 Android 版本 2.20.441.06.40 的 Google Drive 的代码串中发现了关于即将推出的功能的提示。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

以下是我们发现的新字符串:

```
 <string name="dialog_download_and_decrypt_button">Download and decrypt</string>
<string name="dialog_download_and_decrypt_message">Download this file to view it</string>
<string name="dialog_download_and_decrypt_title">"Can't open file"</string>
<string name="dialog_editor_file_encrypted_message">"You'll be able to open encrypted files soon"</string>
<string name="dialog_editor_file_encrypted_title">Upcoming feature</string>
<string name="action_card_download_and_decrypt">Download and decrypt</string> 
```

其中一个字符串提到可以直接在 Drive 中打开加密文件，另一个字符串提到这将是一个即将推出的功能。其他字符串提到下载和解密文件的能力。

除了新字符串中的内容，没有更多信息可以继续，比如 Drive 用户是否可以直接在网络上或谷歌的应用程序中加密文件。

云存储是备份数据和从任何设备访问数据的好方法。然而，Google Drive 不提供原生加密功能，尽管有支持加密和解密的插件。加密文件和其他文档是保护这些文件免受窥探的一个好方法，无论是帐户泄露还是其他安全问题。看到原生加密添加到谷歌驱动器将是一个很好的方式来进一步保护您的敏感信息。

如果没有加密功能，你可以采取很多措施来保护你在 Google Drive 上的信息安全，包括使用强密码和启用双重身份验证。如果你想加密你上传的文件，有一些应用程序，如 [Boxcryptor](https://www.boxcryptor.com/en/encryption/) ，它集成了 Google Drive。

字符串表明解密功能正在工作中，也许我们很快就会看到一些东西。谷歌最近在其 Google One 服务中增加了一个付费 VPN 功能，所以无论什么样的加密功能都有可能隐藏在付费墙之后。

## 更新 1:更多细节和截图

在我们发表这篇文章后不久，Android 开发人员和逆向工程师 Alessandro Paluzzi 透露了这项即将推出的功能的更多细节。在一条推文中，他透露 Google Drive 应用程序将让你加密保存在设备上的文档(即标记为离线可用的文档)。更改此设置将从您的设备上删除该文件的任何副本。