# WhatsApp 正在测试云聊天备份的端到端加密

> 原文：<https://www.xda-developers.com/whatsapp-end-to-end-encryption-cloud-chat-backups/>

尽管 WhatsApp 为聊天提供端到端加密，但这并没有扩展到备份到 Google Drive 或 iCloud 的消息(和其他媒体)。相反，它们只受到服务器端加密的保护，如果需要的话，相应的云服务可以解密它们。如果你是一个注重隐私的人，那就不太理想了。

不久前，[有人发现【WhatsApp 正在开发一项新功能，可以让你用密码加密聊天备份。该功能最近在几天前面向测试版用户推出，但在随后的更新中被取消。](https://www.xda-developers.com/whatsapp-encrypt-chat-backups/)

据 [*WABetaInfo*](https://wabetainfo.com/whatsapp-beta-for-android-2-21-15-5-whats-new/) 报道，该功能将作为 WhatsApp 测试版 2.21.15.5 的一部分推出。它的工作原理是要求您选择一个密码来加密未来的备份，并且在恢复备份时总是需要输入密码。密码完全是私人的，不会与它通过的任何服务共享，无论是 WhatsApp、脸书、谷歌还是苹果。如果您愿意，也可以使用 64 位加密密钥来代替密码，尽管一旦丢失，您将无法恢复聊天内容。

加密密钥仅包含 a 和 f 之间的数字和小写字母。您需要安全地存储加密密钥，因为如果您丢失了加密密钥，WhatsApp 将无法帮助您恢复聊天记录。它可以防止未经授权访问您的聊天记录，甚至可以在本地备份上工作，以便您可以将它们安全地存储在您想要的任何地方，而不会有被窃取和被其他人访问的风险。

如前所述，由于连接问题，云聊天备份的端到端加密的推出已经[暂时暂停](https://wabetainfo.com/whatsapp-beta-for-android-2-21-15-7-whats-new/)，但希望它很快会再次开始推出。确保从 Google Play 或 APK 托管网站下载最新版本的 WhatsApp，这样一旦该功能可用，你就可以使用它了。