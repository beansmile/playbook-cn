# SSL 证书

[从 DNSimple 购买一个通配符证书](https://dnsimple.com/ssl-certificate)。通配符（*）让你可以在 `www.`、`staging.`、`api.` 或者其他任意的子域名上使用同样的证书。

[在 Heroku 上添加一个 DNSimple SSL 证书](https://gist.github.com/croaky/e0beb6025d58eeb88db5)应该花不了你 15 分钟。

SSL 和 DNS 是紧耦合的。如果要做任何 SSL 相关的工作，我们需要确保有更改 DNS 的权限，例如增加一个 CNAME 记录。如果我们是和客户一起工作，他们有一个部门处理 DNS 事项，那么约好一个避开峰值的时间来一起结对编程做好每件事。如果我们不能有条不紊地进行处理的话，有可能会把一个全站 SSL 网站搞宕机。

[原文链接](https://thoughtbot.com/playbook/production/ssl-certificates)
