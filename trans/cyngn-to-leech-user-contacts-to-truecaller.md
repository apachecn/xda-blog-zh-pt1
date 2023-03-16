# Cyngn 将用户联系信息转移到 Truecaller

> 原文：<https://www.xda-developers.com/cyngn-to-leech-user-contacts-to-truecaller/>

在这篇文章之后，Cyngn 的 Steve Kondik 在 Google+ 上做了一个[回复。不幸的是，他未能以任何方式解决他选择集成的服务上传他人数据的事实，而是选择专注于同意请求流程。他们的用户选择加入过程是无关紧要的，因为数据被上传的人不会看到同意信息——该应用程序未经他们同意就上传了其他人的数据。](https://plus.google.com/+SteveKondik/posts/Wv6s4aRne9R)

Truecaller，一家很多人可能没听说过的公司，刚刚宣布了与 Cyngn 的合作协议，Cyngn 是 CyanogenMod 的商业部门。乍一看，这是将 Truecaller 功能集成到 Cyngn OS 拨号器中的一个很好的结合。

然而，不幸的是，Truecaller 是一家有点有趣的公司，有一些有趣的做生意的方式。他们的商业模式肯定是有问题的(甚至可能更糟)——当你使用 Truecaller 的“增强搜索”功能(这几乎是该产品的 【拉伊】 之子 d'ê tre)时，你就同意 Truecaller 可以从你的手机上收集联系信息，并与该服务的其他用户分享。

“这完全是错误的”，我听到你们敏锐的读者说。"他们肯定不能和别人分享人们的联系方式吧？"良好的...你通常是对的——从法律上讲，至少在欧洲，这是非法的。数据保护指令是一项相当长的立法，涵盖了此类问题，为了我们欧洲用户的利益，我们稍后将回来看一看它。

Truecaller 使用的“脱身之计”隐藏在他们的[服务条款](http://www.truecaller.com/terms-of-service)中，他们神奇地试图摆脱这一困境:

> 通过允许收集联系信息，您给予 Truecaller 使用该联系信息作为服务一部分的权利，并保证您拥有与我们分享该联系信息所需的任何及所有权限。您可以随时选择退出以阻止联系信息的共享。

是的，没错...你没听错。作为最终用户，您必须同意您的所有联系人都同意您将他们的数据上传到 Truecaller。他们声称有 16 亿人的电话号码可以搜索，让你搜索他们的号码。这里有一个问题——有多少人向这项服务提交了他们的联系人信息，并获得了许可？当然，你可以选择不向他们发送数据，但这没有多大用处，因为不可能真的选择不让别人分享你的数据。事实上，虽然 Truecaller 提供了一个让你从名单上除名的机会，但这首先需要你知道他们持有你的数据。

回到[欧盟数据隐私指令](http://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:31995L0046)，这里有一些有趣的相关声明:

*(a)‘个人数据’是指与已识别或可识别的自然人(‘数据主体’)相关的任何信息；可识别的人是指可直接或间接识别的人，特别是通过识别号码或一个或多个与其身体、生理、心理、经济、文化或社会身份相关的因素；"*

由于您的姓名是与您相关的信息，作为一个可识别的人，任何与您相关的数据都是“个人数据”。

*‘数据主体的同意’是指数据主体自由给出的、具体的、知情的意愿表示，数据主体通过该表示同意处理与他有关的个人数据。"*

这在法律的范围内定义了同意的含义，要求人们给出可以处理其数据的知情指示(处理包括对数据的任何形式的手动或自动操作，包括存储！)

然而，该立法最重要的部分是第 7 条，它涵盖了在何种情况下可以处理个人数据。让我们看看这些。

*成员国应规定，只有在下列情况下才可处理个人数据:*

*(a)数据主体明确表示同意；或者*

你是数据主体；不是上传的人。因此你没有同意。

*(b)为履行数据主体作为一方的合同或在签订合同前应数据主体的要求采取措施，处理是必要的；或者*

因为你不知道是否有人决定将你的数据发送给 Truecaller，你显然没有签订合同。你必须意识到这一点，并选择成为这种合同的一方。

*(c)处理是遵守控制方必须遵守的法律义务所必需的；或者*

Truecaller 没有提供此服务或收集数据的法律义务。

*(d)为了保护数据主体的重大利益，处理是必要的；或者*

您的切身利益没有受到 Truecaller 的保护，它允许任何人从您的电话号码中找到您的姓名。事实上，你的隐私(一项人权)的切身利益更有可能因此受到侵犯。

*(e)为了公共利益或行使授予财务总监或向其披露数据的第三方的官方权力而执行任务时，处理是必要的；或者*

这不符合公众利益，也没有官方权力来执行这一处理。

*(f)为了控制者或向其披露数据的第三方所追求的合法利益，处理是必要的，除非此类利益被数据主体的基本权利和自由的利益所压倒，而这些权利和自由根据第 1 (1)条需要保护。*

第 1 条要求保护"自然人的基本权利和自由，特别是他们在处理个人数据方面的隐私权"。这一条款不会帮助他们摆脱困境。

因此，我建议 Truecaller 没有法律许可处理来自其服务的非用户的任何个人数据。它从其他人那里收集的数据不是他们的数据，而是其他数据主体的个人数据。这些人(在我看来)对 Truecaller 有合法的权利。由于 Truecaller 位于欧盟成员国瑞典，数据保护指令适用于他们。

看到这种功能集成到一个定制固件中，意味着为用户提供选择和自由，这几乎是不可思议的。随着 Cyngn 试图成为“反谷歌”，也许他们应该在将最新的#bigthing 集成到他们的产品之前看看？

也许是时候让 Truecaller 的欧洲受害者聚在一起，就此事提出一个测试案例了？在我看来这相当清楚。Truecaller 没有得到他们处理数据的人的同意。如果针对 Truecaller 的行动成功，像脸书这样的公司可能是下一个，因为他们习惯于将你的联系数据“释放”到他们的服务器上(未经相关人员同意)，以建立非脸书用户的影子档案。鉴于我们已经知道脸书一直在收集、整理和汇集尽可能多的关于非服务用户(他们没有同意脸书处理他们的数据)的联系数据，也许他们在爱尔兰应该打印一份数据保护指令并阅读一下？