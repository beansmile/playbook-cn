# 持续集成

Martin Fowler 曾经[详细介绍过](http://martinfowler.com/articles/continuousIntegration.html)持续集成。要点是：

- 每个开发人员都在他自己的机器上跑测试套件。
- 当他们提交代码到代码控制仓库时，会「集成」其他人提交的代码，重新运行一次测试。

这有助于保证不会有依赖特定开发人员机器才能通过的测试。代码在部署到生产服务器之前，还要在生产环境再运行一次测试，这次它运行在 CI 服务器或者服务上。

当构建失败时，会通过 Slack 和 email 通知我们。点击链接我们可以看到一个回溯报告，它给我们提示如何来「修复这个构建」。

当我们修复并提交到版本控制系统之后，我们将会从 Slack 和 email 得到一个「成功构建」的通知。

一个可靠的测试套件对于 web 应用来说绝对必要的。但是，测试套件的问题是它会不断变大的同时也会变得更慢。

CI 通过并行运行测试来解决这个痛点。通过使用 CI 我们将原本需要 45 分钟运行完毕的测试缩减到 2 分钟内完成。

我们用过 CruiseControl、Integrity、Hudson (now called Jenkins) 以及其他 CI 库过来构建我们自己的 CI。结果是花费了很多宝贵的时间。

现在我们对开源项目使用 [Travis CI Free](http://travis-ci.org/) 。我们在私有仓库使用 [Travis CI Pro](https://www.travis-ci.com/)，因为它的 UI 一致，配置简单，并且和 GitHub 紧密结合。

[GitHub post-receive hooks](https://help.github.com/articles/post-receive-hooks) 会触发 CI 运行。我们 GitHub 仓库主要集成的钩子有：

- 用于 CI 的 Travis
- 用于代码质量和安全检查的 [Code Climate](https://codeclimate.com/)
- 用来强化代码风格规范的 [Hound](https://houndci.com/)
- 用来集成聊天室通知的 Slack

[原文链接](https://thoughtbot.com/playbook/developing/continuous-integration)
