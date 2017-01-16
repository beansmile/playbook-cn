# 日志收集

大部分应用将有用的调试信息写入日志。在 Heroku，它们默认去向标准输出，最终都被忽视了。

我们通常使用 [Logentries](https://logentries.com/) 来接受来自 Heroku 或者其他来源的日志。一旦日志被发送到 Logentries，你就可以搜索之前的日志，并且可以设置针对 Rails 栈之外的错误报警，例如内存不足错误。

如果我们要在客户项目中使用 Logentries，最好的解决方案是客户创建一个 Logentries 账号并加一个相关的 thoughtbot 成员。如果客户不想创建账号，或者创建账号的过程过于冗长，我们就在 thoughtbot 的 Logentries 账号创建一个新项目，然后在合约结束后再删除它。

我们没有使用 Heroku Logentries addon，因为它会自动创建一系列警报并自动发送给我们在 Heroku 上的每一个管理员。

要在 Heroku 设置 Logentries，请参考 [instructions for setting up a syslog drain](https://logentries.com/doc/heroku/#syslog_drain)。

[原文链接](https://thoughtbot.com/playbook/production/log-collection)
