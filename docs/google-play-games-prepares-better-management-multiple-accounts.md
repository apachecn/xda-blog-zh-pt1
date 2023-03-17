# Google Play Games 准备为多个帐户添加更好的管理

> 原文：<https://www.xda-developers.com/google-play-games-prepares-better-management-multiple-accounts/>

Google Play 游戏将很快允许游戏玩家在他们的多个 Google 账户之间无缝切换。目前，当你通过 [Google Play Games](https://www.xda-developers.com/google-play-games-add-home-screen-folder-games/) 使用谷歌账户登录游戏，并希望在以后更改默认账户时，没有简单的方法可以做到这一点。

你唯一且不太方便的选择是要么重新安装整个游戏，要么从应用程序设置中删除游戏数据，如果你的游戏很大，需要下载数千兆字节的游戏资源，你可能不想这么做。然而，谷歌似乎会让游戏玩家更容易退出当前账户，转而使用另一个账户。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

在 Google Play Games v2021.02.24917 中，我们发现一些字符串表明 Google Play Games 应用程序本身将允许您更改用于游戏的默认帐户，更改用于所有新游戏的默认帐户，或者更改基于每个游戏的帐户。

更改帐户将删除所有本地进度和与该帐户相关的设置，但这确实意味着您可以更容易地切换帐户，更重要的是无需从头重新安装游戏。

以下是 Google Play 游戏 v2021.02.24917 中的新字符串:

```
 <string name="games__signinsettings__change_default_account_for_all_games_dialog_description">Current default account: %1$s</string>
<string name="games__signinsettings__change_default_account_for_all_games_dialog_option_for_all_games_description">"You'll lose access to progress and settings for games you've played. We'll restart the game to apply your changes."</string>
<string name="games__signinsettings__change_default_account_for_all_games_dialog_option_for_all_games_title">" Change the default account for "<b>all games</b>" "</string>
<string name="games__signinsettings__change_default_account_for_all_games_dialog_option_only_for_new_games_description">"You won't lose access to progress and settings for games you've played. But your progress will be split between accounts."</string>
<string name="games__signinsettings__change_default_account_for_all_games_dialog_option_only_for_new_games_title">" Change the default account only for "<b>new games</b>" "</string>
<string name="games__signinsettings__change_default_account_for_all_games_dialog_option_sign_out_of_all_games_description">"You'll lose access to progress and settings for games you've played. We'll restart the game to apply your changes."</string>
<string name="games__signinsettings__change_default_account_for_all_games_dialog_option_sign_out_of_all_games_title">" Sign out of "<b>all games</b>" "</string>
<string name="games__signinsettings__change_default_account_for_all_games_dialog_title">Select an option for the new default account</string>
<string name="games__signinsettings__change_per_game_description">"If you change the account for a selected game or sign out of it, you'll lose access to past progress and settings for the game"</string>
<string name="games__signinsettings__change_per_game_dialog_description">"If you change the account you'll lose access to past progress and settings for the game"</string>
<string name="games__signinsettings__change_per_game_dialog_option_ask_every_time">@string/games__signinsettings__game_state_description_ask_every_time</string>
<string name="games__signinsettings__change_per_game_dialog_option_sign_out">Sign out</string>
<string name="games__signinsettings__change_per_game_dialog_option_use_player">Use %1$s</string>
<string name="games__signinsettings__change_per_game_dialog_title">Select an option for this game</string>
<string name="games__signinsettings__change_per_game_title">Change the account by game</string>
<string name="games__signinsettings__sign_out_of_all_games_option_dialog_description">"While you're signed out, you'll lose access to progress and settings for these games:"</string>
<string name="games__signinsettings__sign_out_of_all_games_option_dialog_sign_out_button">Sign out</string>
<string name="games__signinsettings__sign_out_of_all_games_option_dialog_title">Are you sure you want to sign out of all games?</string> 
```

目前，这一变化尚未在最新版本的 Google Play Games 应用程序中实现。我们将密切关注这一功能的进一步进展，并肯定会让你知道它何时对所有人开放。