# 代码审查

以下是审查流程。请阅读我们的 [git 协议](https://github.com/thoughtbot/guides/tree/master/protocol)来了解使用到的 git 命令。

- 从主分支创建一个本地功能分支。
- 功能开发完成并通过测试后，暂存这些改动。
- 暂存改动后，提交改动。
- 写上[良好的提交信息](http://robots.thoughtbot.com/5-useful-tips-for-a-better-commit-message)。
- 推送你的分支到远程服务器。
- 发一个 [GitHub pull request](https://help.github.com/articles/using-pull-requests/)。
- 在 [Slack](https://slack.com/) 发送一个代码审查请求。
- 作者之外的另一个队友审查 pull request。他们[遵守代码审查规范](https://github.com/thoughtbot/guides/blob/master/code-review)来避免误会。
- 他们在 GitHub 的 web 界面或者 Slack 里面评论和直接问关于代码的问题。
- 没问题了他们会在 pull request 上留言 「可以合并」。
- 交互式地变基代码。合并类似「修复空白」这样的提交到一两个有价值的提交中。编辑提交信息，表明你的意图。
- 审查新的提交。审查文件变动。合并分支到主分支。
- 删掉你的远程功能分支。
- 删掉你的本地功能分支。

测试驱动开发会让代码的缺陷在开发过程中更早曝露出来。在你的开发机上发现一个失败的测试，比在生产环境上发现要好得多。它可以让你有更加紧密的反馈循环。

代码审查在代码合并到主分支之前发生，它能带来类似的好处：

- 新代码写出来之后整个团队都会知道。
- 错误可以更早地被捕捉到。
- 代码标准更容易被建立、讨论和执行。
- 从这种风格的代码审查中得到的反馈更容易被应用。
- 更不容易忘记具体的情境（「为什么我会写这个？」）因为在作者头脑中它是鲜活的。

[原文链接](https://thoughtbot.com/playbook/developing/code-reviews)
