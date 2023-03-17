# Android Auto 可能很快就会被设置为自动启动，即使你的手机被锁定

> 原文：<https://www.xda-developers.com/android-auto-could-soon-be-set-to-start-automatically-even-if-your-phone-is-locked/>

# Android Auto 可能很快就会被设置为自动启动，即使你的手机被锁定

Android Auto 的最新更新表明，它可能很快允许你设置应用程序自动启动，即使手机被锁定。

Android Auto 是谷歌对“我如何将手机连接到汽车”这个问题的回答。该应用程序本质上允许您在驾驶时访问一组有限的优化功能，主要目标是平衡驾驶员的注意力、连接性和娱乐性。但要真正连接到 Android Auto，你需要将智能手机连接到汽车的信息娱乐单元，要么通过有线连接，要么通过无线连接。谷歌显然正在让连接 Android Auto 变得更加方便，让用户无需解锁智能手机就可以连接。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

我们在 [Android Auto 5.9](https://www.apkmirror.com/apk/google-inc/android-auto/android-auto-5-9-6046-release/) 中发现了以下新字符串:

```
 <string name="settings_connection_allowed_while_locked_description">Even when your phone is locked</string>
<string name="settings_connection_allowed_while_locked_title">Start Android Auto automatically</string> 
```

目前，如果你将手机连接到汽车并解锁手机，Android Auto 应用程序会自动启动(假设你的手机上已经安装了该应用程序，并且你的主机支持 Android Auto)。我们知道一些设备在与解锁的手机连接时无法自动启动 Android Auto。虽然应用程序中的提示没有提到这一点，但这个新设置可能是为了补救这些连接失败的情况。如果该功能完成实施，当您连接智能手机时，该应用程序应该会自动启动，而不需要您在切换设置时解锁手机。

我们不知道这个功能是用于有线连接还是无线连接，或者两者都是。我们将不得不等待谷歌推出的变化，以了解更多。