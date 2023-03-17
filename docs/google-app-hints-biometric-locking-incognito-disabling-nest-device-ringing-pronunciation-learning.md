# 谷歌应用程序提示语音学习，隐姓埋名的生物识别锁，等等！

> 原文：<https://www.xda-developers.com/google-app-hints-biometric-locking-incognito-disabling-nest-device-ringing-pronunciation-learning/>

谷歌应用程序被宣传为“更智能的移动搜索方式”，但该应用程序已经发展到如此之多。虽然搜索仍然是一个很好的焦点，但还有其他功能，如个性化订阅、通知、[和更多](https://www.xda-developers.com/google-app-preps-assistant-memory-and-at-a-glance-media-recommendations/)。谷歌似乎有心情让这款应用服务于更多用途，因为最新的谷歌应用测试版包含一些功能提示，例如用生物识别锁定匿名会话，当你不在家时禁止 Nest 设备响铃，甚至教你发音。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

谷歌应用 11.39.7 测试版包含了相当多的新字符串，我们在下面会提到。

## 用于嵌套设备智能戒指

新法规建议，Nest 智能家居设备可以选择禁用铃声功能。

```
 <string name="assistant_settings_call_smart_ring">Smart Ring</string>
<string name="assistant_settings_call_smart_ring_description">Nest devices will only ring when you are at %1$s</string> 
```

我们认为，当你不在某个地方，大概是在你家的时候，这个功能会让用户选择禁用 Nest 设备的铃声。

* * *

## 在谷歌应用中使用生物特征锁定匿名

谷歌应用已经有了一个隐名模式，在账户切换菜单中标记为“无账户使用”。谷歌也一直在开发一款应用内匿名浏览器，尽管据我所知该功能还没有上线。根据新的字符串，谷歌似乎正在增加一个选项，为这种匿名模式启用生物识别锁定和解锁。

```
 <string name="googleapp_incognito_biometric_prompt_subtitle">Confirm biometrics to continue</string
<string name="googleapp_incognito_biometric_prompt_title">Resume Incognito session?</string>
<string name="googleapp_incognito_enable_biometrics_dialog_msg">{count, plural, =1{When enabled, you’ll need to use biometrics to continue your previous Incognito sessions after one minute of inactivity.} other{When enabled, you’ll need to use biometrics to continue your previous Incognito sessions after 
<string name="googleapp_incognito_enable_biometrics_dialog_title">Use biometrics to resume Incognito sessions?</string>
<string name="googleapp_incognito_enable_biometrics_enable_btn_text">Enable</string>
<string name="googleapp_incognito_enable_biometrics_exit_btn_text">Exit Incognito mode</string>
<string name="googleapp_incognito_enable_biometrics_not_now_btn_text">Not now</string>
<string name="googleapp_incognito_offramp_internal_button">Turn off</string>
<string name="googleapp_incognito_offramp_internal_message">"You'll need to turn off Incognito mode for this. Your Incognito session will be cleared and you'll return to the app home screen."</string>
<string name="googleapp_incognito_offramp_internal_title">Turn off Incognito mode?</string> 
```

本质上，有了这个即将到来的选项，你可以匿名浏览，然后在一段时间不活动后锁定会话。要解锁会话，您需要验证您的生物特征，可能是您的指纹或面部解锁，这取决于您在设备上的设置。

* * *

## 语音学习

谷歌似乎也在致力于教用户如何发音。

```
 <string name="pronunciationlearning_app_logo_description">Logo of Pronunciation Learning App</string
<string name="pronunciationlearning_app_title">Speaking practice mode</string>
<string name="pronunciationlearning_content_box_title">English</string>
<string name="pronunciationlearning_correct_phoneme_title">"Correct pronunciation"</string>
<string name="pronunciationlearning_exit_button_description">Exit</string>
<string name="pronunciationlearning_expected_text_title">Try saying</string>
<string name="pronunciationlearning_feedback_text_title">Feedback</string>
<string name="pronunciationlearning_good_job_text">Good job!</string>
<string name="pronunciationlearning_input_text_hint">Try typing “How are you?”</string>
<string name="pronunciationlearning_start_practice_text">Practice</string>
<string name="pronunciationlearning_startover_text_button">Start over</string>
<string name="pronunciationlearning_tts_description">Hear text pronunciation</string>
<string name="pronunciationlearning_user_phoneme_title">"Sounds like you said"</string> 
```

根据目前可见的字符串，即将到来的“口语练习模式”似乎仅限于英语，但人们可以希望看到该功能在未来扩展到更多的语言。从我们收集的信息来看，该功能将展示一个单词，并要求用户重复一遍，同时提示播放正确的发音。还有一个文本输入的提示，尽管我们不确定打字如何适应语音教学的主题。

* * *

尚不清楚这些功能何时/是否会为谷歌应用的用户上线。这可能需要几天，几周，甚至几个月。我们将尝试并激活这些功能来展示它们，但与此同时，我们将密切关注它们的正式推出。