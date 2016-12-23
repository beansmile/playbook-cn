# 事务性邮件

我们使用 [SendGrid](http://sendgrid.com/)（Free-$400+/month）来向我们的用户发送被称为[事务性邮件](http://www.foundrygroup.com/wp/2010/04/foundry-group-invests-in-sendgrid/)的电子邮件。

典型的事务性电子邮件有：

- 确认
- 使用 3 天后对用户的跟进
- 免费试用期失效
- 向系统功能中的其他用户发消息

我们直接使用 SendGrid，而不是 Heroku 的 add-on，以避免和其他在 Heroku 上而且在同一个 IP 组内乱发邮件的用户被归到一起。
