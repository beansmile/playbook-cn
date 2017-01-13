# 验收测试

验收测试是把[工作故事转化为代码](https://gist.github.com/croaky/d8699363382d86c10c54)的过程。这个代码是针对应用来运行的。测试第一次运行的时候会失败。开发人员实现应用代码直到测试通过。

当测试通过时，开发人员提交代码并附上类似以下的信息：

> 访客创建了抵押

代码在[持续集成](https://thoughtbot.com/playbook/developing/continuous-integration)（译注：Continuous Integration，英文缩写 CI）服务器上再运行一次，以确保验收测试在符合生产环境的环境下依然能运行通过。

同时，代码会被部署到 staging 环境中，开发人员和客户代表在浏览器中进行冒烟测试。

当验收测试在 CI 服务器上通过，你和其他的设计师、开发人员或者客户在 staging 上也确认工作故事完成了，那么这个功能就会随时被部署到生产服务器上。这样做就可以频繁地将新功能部署到生产服务器，迅速地将更多的价值交付给客户。

[原文链接](https://thoughtbot.com/playbook/developing/acceptance-tests)
