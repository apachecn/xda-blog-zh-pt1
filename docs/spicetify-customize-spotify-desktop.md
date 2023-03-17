# Spicetify 可以让你定制你的 Spotify 桌面应用——以下是使用方法

> 原文：<https://www.xda-developers.com/spicetify-customize-spotify-desktop/>

如果你喜欢一直听音乐，你可能会使用 Spotify 这样的音乐流媒体应用程序。虽然我对 Spotify 从来没有太多抱怨，但最近对桌面和网络客户端的更新[看到了对其 UI 的彻底检查](https://www.xda-developers.com/spotify-redesign-desktop-and-web-player/)已经惹恼了很多*人*。如果你可以根据自己的喜好*定制用户界面会怎么样？如果你可以挑选你想添加的特性会怎么样？进入 Spicetify，这是一个命令行界面应用程序，允许您自定义 Spotify 桌面客户端。*

**该应用程序不隶属于 Spotify。Spicetify 已经存在很多年了，虽然我还没有看到任何人因为使用这个应用程序而被禁止，但是使用它要自担风险。**

* * *

## 如何安装和使用 Spicetify

首先，本教程面向 Windows 用户，你需要使用从 Spotify 下载的官方 Spotify 桌面客户端，而不是从 Windows 商店下载。如果你从 Windows 商店安装了 Spotify，你需要卸载它，然后[从官方网站](https://www.spotify.com/us/download/windows/)重新安装。如果你使用 Linux 或 macOS，你可以看看 GitHub 官方页面上的[，了解更多关于如何在你的机器上安装它的信息。如果你使用的是 Windows，那么请继续阅读！](https://github.com/khanhas/spicetify-cli)

### 步骤 1:使用 PowerShell 安装

到目前为止，安装 Spicetify 最简单的方法是使用 Windows PowerShell。只需运行以下命令。

```
 Invoke-WebRequest -UseBasicParsing "https://raw.githubusercontent.com/khanhas/spicetify-cli/master/install.ps1" | Invoke-Expression 
```

如果您看到类似上面的输出，您就可以进入下一步了！

### 步骤 2:设置香料

一旦安装了 Spicetify，您仍然需要将其配置为指向您当前安装的 Spotify。使用以下命令生成默认配置文件。这将找到您当前安装的 Spotify。

```
 spicetify 
```

现在运行以下命令，将默认的 Spicetify 主题和补丁应用到您的 Spotify 客户端。

```
 spicetify backup apply enable-devtool 
```

如果您看到类似上面的输出，那么这意味着您已经准备好了。如果你启动 Spotify，你应该会看到应用了 Spicetify 的默认灯光主题。

### 步骤 3:安装自定义主题

现在你已经设置好了，是时候安装自定义主题了！这里有一个[神奇的 GitHub 库](https://github.com/morpheusthewhite/spicetify-themes)，里面装满了你可以安装的自定义主题。在 Windows 上，你可以导航到 C:/Users/ <你的用户名> /。找到你需要保存你的主题和扩展的地方。如果要安装自定义主题，请导航到 themes 文件夹，创建一个以要安装的主题命名的新文件夹，并将 color.ini 和 user.css 文件保存在该文件夹中。

接下来，导航回。spicetify 文件夹并打开 config.ini 文件。将 current_theme 从 SpicetifyDefault 更改为您创建的主题文件夹的名称。对我来说，我把它的值改成了“初等”。准备好之后，运行下面的命令。

```
 spicetify apply 
```

Spotify 现在应该会重新启动，如果成功的话，你会看到你的新主题被应用了！

### 步骤 4:安装扩展和应用程序

Spicetify 不仅仅是关于主题的——你也可以安装扩展！你把它们安装在 C:/Users/ <你的用户名> /中。spicetify/extensions，你可以在这里查看官方支持的扩展的完整列表。还有一个 Reddit 应用程序，它可以在任何给定的子编辑中获取前 100 个 Spotify 帖子。它甚至可以获取 YouTube 上的帖子，并在 Spotify 上播放。虽然我在让它工作时遇到了一些麻烦(因为 Spotify 制作的 GLUE CSS 无法加载)，但还是值得一试，看看它是否对你有用！

* * *

## 你完了！

如果您遵循了上面的所有步骤，那么您应该已经完成了 Spicetify 的配置并准备好了。这是一个有点复杂的过程，但一旦你让它工作，这是一个很好的方式来定制你自己喜欢的 Spotify 桌面客户端。如果你发现任何好的主题、应用或扩展，请在下面的评论中告诉我们！