# 你需要知道的关于 RIAA DMCA 关闭 YouTube-DL

> 原文：<https://www.xda-developers.com/youtube-dl-riaa-dmca/>

美国唱片业协会(RIAA)，代表美国唱片业的贸易组织，[上周五为多个包含 YouTube-DL 代码的 GitHub 存储库提交了一份 DMCA 下架通知](https://github.com/github/dmca/blob/master/2020/10/2020-10-23-RIAA.md)。YouTube-DL 是一个开源 Python 库，用于从 YouTube 和其他视频托管站点下载视频和/或音频。该库被整合到许多不同的项目和应用程序中，如 XDA 上的 [GetTube](https://forum.xda-developers.com/android/apps-games/app-gettube-youtube-downloader-t3217010) 和 [arkTube](https://www.xda-developers.com/arktube-is-a-light-weight-feature-filled-youtube-downloader/) 以及流行的开源 [NewPipe 应用程序](https://www.xda-developers.com/tag/newpipe/)。

RIAA 起诉 DMCA，指控 YouTube-DL 违反了 DMCA 关于规避版权保护系统的规定( [section 1201](https://www.law.cornell.edu/uscode/text/17/1201) )。作为证据，RIAA 引用了 YouTube-DL 源代码中的评论，这些评论告诉用户如何针对其成员拥有版权的视频测试该程序。链接版权材料的测试旨在确保图书馆可以下载正常视频、有年龄限制的视频和名称中包含美元符号的视频。用于测试的这 3 个视频是 Icona Pop、Justin Timberlake 和 Taylor Swift 的音乐视频。

“事实上，YouTube-DL 源代码中的评论清楚地表明，源代码是为了绕过 YouTube 的技术措施而设计和销售的，以便未经授权访问我们成员的版权作品，”RIAA 在诉状中写道。

尽管这些视频只是作为开发者的测试，而不是作为样本使用，但 RIAA 声称，整个 YouTube-DL 项目明显是为了规避其成员的版权保护，从而使整个库的分发非法。当然，YT-DL 的开发者辩称，该库的唯一目的不是规避 RIAA 会员拥有的视频的版权保护。YT-DL 显然是被盗版者使用的，但它也是档案管理员、研究人员、记者等的有用工具。，可用于下载 CC 许可的视频或公共领域的视频，如政府视频。一些创作者也依靠该工具下载他们自己的视频。

虽然 DMCA 是美国法律，但 RIAA 似乎也在对欧洲的项目开发商采取行动。撤下通知援引了德国汉堡地区法院的一项裁决，称同样的规定适用于该国。即使 RIAA 的主张是没有法律依据的——TechDirt 指出，美国最高法院在[索尼诉环球](https://en.wikipedia.org/wiki/Sony_Corp._of_America_v._Universal_City_Studios,_Inc.)一案中裁定，具有实质性非侵权用途的工具本身并不侵权——这个问题需要通过 RIAA 的让步或 YT-DL 作者提交反通知来解决，然后 RIAA 将提起诉讼。对于一个社区运营的开源项目来说，诉讼很难管理，但非营利数字权利组织电子前沿基金会(EFF)暗示它可以参与进来。

值得一提的是，GitHub 别无选择，只能在这场纠纷持续期间遵守 DMCA 的撤下通知，因为如果他们不遵守，可能会被追究法律责任。于是，18 个带有 YouTube-DL 代码的 GitHub 库被拿下，包括主库。虽然主库已经在其他 GitHub 库上分叉[，在](https://github.com/blackjack4494/yt-dlc)[其他代码共享网站](https://gitlab.com/ytdl-org/youtube-dl)上重新托管，和/或由开发者私下和公开存档，但 RIAA 可以向这些重新托管的代码发送额外的撤销通知。尚不清楚删除有问题的测试案例和版权视频链接是否足以让 YouTube-DL 逃脱 RIAA 的投诉。尽管如此，我们可能会继续看到原始项目的分叉出现，侵权内容的链接被开发者自己上传的内容或根据更开放的条款许可的内容所取代，如知识共享许可。

对于使用 YouTube-DL 的项目来说，当主要的 YT-DL repo 关闭时，挑战将是更新他们的应用程序下载器代码以保持工作。众所周知，YouTube 经常改变事情，这直接或间接地破坏了与 YouTube-DL 的兼容性。然而，YouTube-DL 的开发者最终会推出修复程序，让它再次工作。然而，由于不再有一个开发它的中央存储库，开发者将更难合作和共享修复。YT-DL 开发人员可以用其他方法解决这个问题，比如制作一个私人 GitLab 服务器，但是如果 RIAA 继续采取行动，这个项目的未来仍然不明朗。

*特色图片:YouTube-DLG，youtube-dl 的前端图形用户界面*