# 这是我们的playbook

**我们和各种规模的团队合作，在 iOS、Android 和 Web 平台上设计、开发并推广他们的产品。**

**这是我们的 playbook**

我们是 [thoughtbot](https://thoughtbot.com/)。我们和世界各地的上百个产品团队合作过，他们中既有自筹资金的个人创业者，也有庞大的跨国公司。我们也创建了自己的产品，同时有若干个开源项目。

这是我们的 playbook。它详细解释了我们是如何创建成功的 web 和移动产品，以及如何运营公司。书中充满了我们自身的经验以及研究其他团队的心得。

这是一份未定稿的文档，thoughtbot 中的每一位成员都可以在一个私有 GitHub 仓库中编辑它。

我们使用 Creative Commons Attribution-NonCommercial 协议来发布这份文档，你可以学习或者在自己的公司运用我们的策略。虽然这些策略对我们有用，但是哪些工具和技术适合你自己的情况，相信你比我们更清楚。

**产品设计 Sprint**

我们的项目从便签纸和草图，到最终落实到代码实现的整个过程中，都是以设计为导向的。我们使用设计 Sprint 和用户调查来理解我们客户的问题，验证产品假设，构建以用户为中心的产品。

- [产品设计 Sprints 概述](chapter-1-product-design-sprint/introduction.md)
- [阶段 0：准备](chapter-1-product-design-sprint/phase-0-prepare.md)
- [阶段 1：理解](chapter-1-product-design-sprint/phase-1-understand.md)
- [阶段 2：发散](chapter-1-product-design-sprint/phase-2-diverge.md)
- [阶段 3：汇聚](chapter-1-product-design-sprint/phase-3-converge.md)
- [阶段 4：原型](chapter-1-product-design-sprint/phase-4-prototype.md)
- [阶段 5：测试和反馈](chapter-1-product-design-sprint/phase-5-test-and-learn.md)

**选择平台**

在产品的早期阶段，我们必须确定要使用的平台。选择哪个平台取决于我们解决用户问题的方案。除了考虑对用户而言是最好之外，我们认为最佳的工具还需要有一个活跃的社区，让我们乐于使用，并且有助于创建产品然后快速迭代。

- [「移动」是指用户，而非设备](chapter-2-choose-platforms/mobile-refers-to-the-user-not-the-device.md)
- [在移动设备上原生编程至关重要](chapter-2-native-matters-on-mobile-devices.md)
- [Rails 可使 web 产品快速推向市场](chapter-2-choose-platforms/rails-gets-web-products-to-market-quickly.md)

**笔记本设置**

你的笔记本就是你的剑。不要打没准备的仗。

- [自动化你的开发环境](chapter-3-laptop-setup/automate-your-development-environment.md)
- [使用 dotfiles 共享笔记本设置](chapter-3-laptop-setup/share-configuration-with-dotfiles.md)
- [使用可扩展的编辑器](chapter-3-laptop-setup/use-an-extensible-editor.md)

**计划**

我们工作流程的一个主要目标是持续发布可以工作的小版本。我们通过频繁沟通和每周迭代来完成产品开发计划。

- [流程要因产品和团队而定](chapter-4-planning/adapt-process-to-the-products-needs.md)
- [每日站立会议可以建立信任和保持冲劲](chapter-4-planning/daily-standups-build-trust.md)
- [没有比当面沟通更有效的沟通方式](chapter-4-planning/in-person-communication.md)
- [使用轻量级程序来管理任务优先级并可视化流程](chapter-4-planning/manage-priorities-with-a-lightweight-process.md)
- [每周碰面讨论成果、错误和未来计划](chapter-4-planning/meet-weekly-to-discuss-successes-failures-and-plans.md)
- [一个高效的远程团队不是偶然的产物](chapter-4-planning/working-remotely.md)

**设计**

我们的项目常常是快速变动的。设计师要采用合适的工具和流程来应对这种情况。

- [总是携带速写本](chapter-5-designing/always-carry-a-sketchbook.md)
- [测试产品的可行性和可用性](chapter-5-designing/test-product-viability-and-usability.md)
- [什么是交互设计？](chapter-5-designing/what-is-interaction-design.md)
- [什么是用户界面设计？](chapter-5-designing/what-is-user-interface-design.md)
- [什么是视觉设计？](chapter-5-designing/what-is-visual-design.md)
- [使用HTML和CSS做线框图](chapter-5-designing/wireframing-in-html-and-css.md)

**开发**

我们的开发实践主要参考 Kent Beck 经典的 [Extreme Programming Explained: Embrace Change](http://www.amazon.com/Extreme-Programming-Explained-Embrace-Edition-ebook/dp/B000OZ0N5S)，以及 Gerald Weinberg 的 [The Psychology of Computer Programming](http://www.amazon.com/The-Psychology-Computer-Programming-Anniversary/dp/0932633420)。我们尝试后发现，在多数情况下使用其中的大部分原则改善了我们的工作质量，并提升了团队的幸福感。

- [验收测试](chapter-6-developing/acceptance-tests.md)
- [代码审查](chapter-6-developing/code-reviews.md)
- [持续集成](chapter-6-developing/continuous-integration.md)
- [结对编程](chapter-6-developing/pair-programming.md)
- [重构](chapter-6-developing/refactoring.md)
- [代码风格](chapter-6-developing/style-guide.md)
- [测试驱动开发](chapter-6-developing/test-driven-development.md)
- [版本管理](chapter-6-developing/version-control.md)

**生产环境**

我们生活在一个魔幻的新纪元，很多问题都已经有了解决方案。我们尽可能地聚焦在核心产品，尽量将可分发出去的工作交给外部服务来做。

- [域名和 DNS](chapter-7-production/domain-names-and-dns.md)
- [错误追踪](chapter-7-production/error-tracking.md)
- [主机托管](chapter-7-production/hosting.md)
- [日志收集](chapter-7-production/log-collection.md)
- [支付处理](chapter-7-production/payment-processing.md)
- [性能监控](chapter-7-production/performance-monitoring.md)
- [生产环境清单](chapter-7-production/production-checklist.md)
- [SSL 证书](chapter-7-production/ssl-certificates.md)
- [事务性邮件](chapter-7-production/transactional-email.md)

**度量**

度量的难点在于决定要追踪什么。Dave McClure 的 [AARRR 框架](http://www.slideshare.net/dmc500hats/startup-metrics-for-pirates-nov-2012) 为重要指标提供了一个高层次的概述。我们使用事件追踪等技巧来测量那些指标。

- [AARRR 框架](chapter-8-measuring/aarrr.md)
- [A/B 测试](chapter-8-measuring/ab-testing.md)
- [功能旗标](chapter-8-measuring/feature-flags.md)
- [度量](chapter-8-measuring/instrumentation.md)
- [订阅指标](chapter-8-measuring/subscription-metrics.md)

**我们的公司**

我们相信总是可以找到更好的工作方式，因此我们期待可以找到它并和分享给尽可能多的人。

- [招聘](chapter-9-our-company/hiring.md)
- [运营](chapter-9-our-company/operations.md)
- [原则](chapter-9-our-company/principles.md)
- [营销](chapter-9-our-company/sales.md)
- [分享](chapter-9-our-company/sharing.md)
- [时间](chapter-9-our-company/time.md)
