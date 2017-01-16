# 性能监控

我们使用 [NewRelic](http://www.newrelic.com/)（免费 - 100多美元 / 月）来监控我们生产级别应用的性能。

性能调试可能是开发工作中最美好的部分。因为这是一个明确的、可以量化的问题。当修复了问题时，我们会看到数据的改善。我们可以说「我们提升了 175% 的性能」。

有很多行之有效的修复性能问题的技巧。在使用 Rails + Heroku 时，有些是「免费」的：

- Amazon server clusters
- gzipping
- [Asset pipeline](http://guides.rubyonrails.org/asset_pipeline.html)
- [SQL query caching](http://guides.rubyonrails.org/caching_with_rails.html#sql-caching)

有些需要开发人员的思考：

- Database indexing
- Eager loading
- HTTP caching

页面缓存是我们用得最多的技巧，但是如果我们能缓存页面并将它们推送到 CDN，那将是最快的解决方案。

[原文链接](https://thoughtbot.com/playbook/production/performance-monitoring)
