# SSL证书

[从DNSimple购买一个通配符证书](https://dnsimple.com/ssl-certificate)。通配符（*）让你可以在www.，staging.，api.,或者其他任意的子域名上使用同样的证书。

[在Heroku上添加一个DNSimple SSL证书](https://gist.github.com/croaky/e0beb6025d58eeb88db5)应该花不了你15分钟。

SSL和DNS是紧耦合的。如果我们要做任何SSL相关的工作，我们需要确保我们有更改DNS的权限，例如增加一个CNAME记录。如果我们是和客户一起工作，他们有一个部门处理DNS事项，那么约好一个避开峰值的时间来一起结对编程做好每件事。如果我们不能有条不紊地进行处理的话，有可能我们会把一个全站SSL的网站搞宕机。

[原文链接](https://thoughtbot.com/playbook/production/ssl-certificates)
