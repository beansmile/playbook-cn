# 日志收集

大部分应用将有用的调试信息写入日志。在Heroku，它们默认去向标准输出，最终都被忽视了。

我们通常使用[Logentries](https://logentries.com/)来接受来自Heroku或者其他来源的日志。一旦日志被发送到Logentries，你就可以搜索之前日志，并且可以设置针对Rails栈之外的错误报警，例如内存不足错误。

如果我们要在客户项目中使用Logentries，最好的解决方案是客户创建一个Logentries账号并加一个相关的thoughtbot成员。如果客户不想创建账号，或者创建账号的过程过于官僚冗长，我们就在thoughtbot的Logentries账号创建一个新项目，然后在合约结束后再删除它。

我们没有使用Heroku Logentries addon，因为它会自动创建一系列警报并自动发送给我们在Heroku上的每一个管理员。

要在Heroku设置Logentries，请参考[instructions for setting up a syslog drain.](https://logentries.com/doc/heroku/#syslog_drain)

[原文链接](https://thoughtbot.com/playbook/production/log-collection)
