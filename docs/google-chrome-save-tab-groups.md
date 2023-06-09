# Chrome 将允许你保存标签组，这样你就不必重新创建它们

> 原文：<https://www.xda-developers.com/google-chrome-save-tab-groups/>

# Chrome 将允许你保存标签组，这样你就不必重新创建它们

谷歌正在努力改善 Chrome 的标签组体验。Chromium Gerrit 上的一个新补丁表明，Chrome 将允许用户保存标签组。

对于那些每天必须处理几十个标签的人来说，Chrome 的[标签组](https://www.xda-developers.com/google-chrome-tab-groups/)功能是一个救星。这是减少浏览器混乱、保持一切整洁有序的好方法。但与此同时，每次重新启动 Chrome 时，都必须从头开始重新创建标签组，这可能很麻烦。谢天谢地，这个问题已经引起了 Chrome 团队的注意。

正如 Reddit 用户 *u/Leopeva64* 发现的[，该团队正在努力改善 Chrome 中的标签组体验。它最近在 Chromium Gerrit 中添加了](https://www.reddit.com/r/chrome/comments/obipdm/google_is_already_working_on_one_of_the_most/?context=3)[一个新的 commit](https://chromium-review.googlesource.com/c/chromium/src/+/2998406) ，这表明 Chrome 将允许你在未来保存标签组。这里的想法是通过不必手动重新创建已经成为日常工作流程一部分的选项卡组来节省时间和精力。提交的描述指出:

> 为 TabGroupsSave 添加一个标志，允许用户将他们的选项卡组保存到他们的书签栏中。

这个补丁有几个尚未修复的错误。对这些错误的描述揭示了这个新选项将如何工作。例如， [issue 122391](https://bugs.chromium.org/p/chromium/issues/detail?id=1223911) 表示当您右键单击选项卡组的标题时出现的气泡 UI 中将添加保存选项卡的选项。对[另一个问题](https://bugs.chromium.org/p/chromium/issues/detail?id=1223921)的描述表明也有可能将选项卡组固定为“类似于扩展”

这一切都还在进行中，还没有最终确定。我们将密切关注这一功能的进一步发展，如果我们了解到任何新的情况，我们会让您知道。Chrome 可能不会很快提供保存标签组的功能，但你可以尝试一个名为 [Tabox](https://chrome.google.com/webstore/detail/tabox-save-and-share-tab/bdbliblipiempfdkkkjohnecmeknnpoa?hl=en) 的扩展来做同样的事情。该扩展允许您将所有打开的选项卡和组保存到一个集合中。每个集合可以有多个选项卡组。您还可以使用 Google Drive 对您的收藏进行颜色编码，以便于分类和在多个设备之间同步。