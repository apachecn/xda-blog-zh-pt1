# Google Play 游戏可能很快会让你在游戏中添加一个主屏幕文件夹

> 原文：<https://www.xda-developers.com/google-play-games-add-home-screen-folder-games/>

谷歌正致力于为 Play Games 应用添加一个新功能,让你可以从主屏幕上访问所有已安装的游戏。我们在最新的 Google Play 游戏更新中发现了新的代码字符串，这些代码字符串突出显示了该功能在未来的更新中推出后将如何工作。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

Google Play Games v 2021.01.24213 刚刚开始在 Play Store 上推出。我们解码了 APK，发现了以下新字符串:

```
 <string name="games__gamefolder__add_to_home_screen_prompt_add_folder">Add folder</string>
<string name="games__gamefolder__add_to_home_screen_prompt_continue">Continue</string>
<string name="games__gamefolder__add_to_home_screen_prompt_message">Find all your games in one place on the Android Home screen (beta feature)</string>
<string name="games__gamefolder__add_to_home_screen_prompt_setting_label">Add the Games folder to the Home screen (beta)</string>
<string name="games__gamefolder__add_to_home_screen_prompt_title">Let Google Play organize your games for you</string>
<string name="games__gamefolder__added_to_home_screen_confirmation_message">All set. Games folder is now on your Home screen.</string>
<string name="games__gamefolder__game_hidden_snackbar_message">Game is now hidden. To show it, go to Play Games settings.</string>
<string name="games__gamefolder__game_of_the_week">Game of the week</string>
<string name="games__gamefolder__games_folder_beta_notice">Beta feature</string>
<string name="games__gamefolder__name">Games</string>
<string name="games__gamefolder__open_play_games_content_description">Open Play Games app.</string>
<string name="games__gamefolder__show_game_folder_in_app_drawer_setting_label">Show the Games folder in the app list (beta)</string>
<string name="games__gamefolder__showing_games_folder_announcement">Showing \"Games folder\" page.</string> 
```

字符串表明，即将推出的功能将允许您在主屏幕上添加一个新的 Play Games 文件夹。该应用程序会自动将安装在您设备上的所有游戏填充到该文件夹中，让您可以在一个方便的位置轻松访问游戏。除了前面提到的字符串，我们还发现了将用于 Play Games 文件夹的图标。看起来是这样的:

此外，我们设法手动启动活动，当您点击游戏文件夹时将会触发该活动。正如你在所附的截图中看到的，这个游戏文件夹不同于你可以添加到主屏幕启动器的其他文件夹。游戏文件夹实际上是在 Google Play Games 应用程序中打开一个活动，而不是像普通文件夹一样在弹出窗口中显示应用程序图标。此活动不是全屏幕的，因此当您打开主屏幕时，不会离开主屏幕。然而，点击右上角的箭头图标确实会将你重定向到 Google Play Games 应用程序。

如果你想知道为什么你会想要这个特性，答案很简单。很方便。虽然你可以在自己选择的主屏幕启动器中创建自己的文件夹，并将游戏添加到其中，但大多数启动器要求你手动完成这一操作，因为它们无法自动将游戏分类到游戏文件夹中。每当你安装一个新游戏时，你必须手动将它添加到文件夹中。新的 Google Play Games 文件夹可以自动完成这一过程，因为该应用程序可以通过访问 [Google Play](https://www.xda-developers.com/tag/google-play-store/) 数据来轻松检测哪些应用程序是游戏。这使得即将推出的 Google Play Games 文件夹比普通文件夹更方便。

截至目前，谷歌尚未发布任何关于新 Play Games 文件夹的官方信息。但由于与该文件夹相关的代码已经出现在 Google Play Games 应用程序中，我们预计它将在未来几周内向用户推出。一旦新文件夹开始向用户推出，我们将立即更新这篇文章。