# 生产环境检查清单

我们发现设置一个新的生产环境或者发布一个产品时，有个简短的检查清单会非常有用：

- 我们是在[最新的 Heroku stack 上](https://devcenter.heroku.com/articles/stack)吗？
- 我们使用了并发的 web 服务器吗？请参见[如何用 Puma 部署](https://devcenter.heroku.com/articles/deploying-rails-applications-with-the-puma-web-server)。
- 需要长时间运行的进程，例如邮件发送是不是被放到后台任务中了？请参考[如何设置 Delayed Job](https://devcenter.heroku.com/articles/production-check#production-tier-database)。
- 是不是有冗余（至少两个）web 和后台进程运行。
- 我们是否启用了 SSL？参考下一节[「SSL证书」](ssl-certificates.md)。
- 即便是同一个应用，API 请求是否是向一个独立的子域名发送的（api.example.com)？这会给我们未来带来架构上的灵活性。
- Gemfile 中是否定义了[最新版本的 Ruby](https://www.ruby-lang.org/en/downloads/)？请看[如何设置](http://bundler.io/v1.11/gemfile_ruby.html)。
- [配置项是不是存在环境变量中](http://12factor.net/config)？
- 手动部署是不是安排在了团队成员都是清醒并可联系上的时候？如果万一有问题，可以及时处理。
- 部署是不是遵循了[详细注释的脚本](https://github.com/thoughtbot/guides/tree/master/protocol/rails#deploy)？
- 我们是否向远程日志服务发送日志？参见下面的[「日志收集」](https://thoughtbot.com/playbook/production/log-collection)章节。
- 我们使用 Heroku 的「标准」数据库还是更高级的？参见 [Heroku production databases](https://devcenter.heroku.com/articles/poduction-check#production-tier-database)。
- 我们备份生产数据库吗？参见 [Heroku PGBackups](https://devcenter.heroku.com/articles/heroku-postgres-backups)。
- 我们监控性能和正常运行时间吗？参见下面的[「性能监控」](https://thoughtbot.com/playbook/production/performance-monitoring)章节。
- 我们追踪错误吗？参见下面的[「错误追踪」](https://thoughtbot.com/playbook/production/error-tracking)章节。

[原文链接](https://thoughtbot.com/playbook/production/production-checklist)
