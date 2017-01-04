# 每周碰面讨论成果、错误和未来计划

每周一次，通常是周一，大家在现场或者通过视频碰面一次。这会替代掉周一的站会，整个团队一起讨论成果，障碍，以及关注点。会议的目的是大家能对未来一周的任务激动不已，并充满了力量。

会议由顾问来主持。

- 理解团队对过去一周的感受以及对未来一周的预期。问来自 thoughtbot 和客户团队的每个成员，「你过去一周感觉如何？你对未来一周预期如何？」这不是一个事无巨细的报告（细节应该在每日站会中解决），而是感受每个人的脉搏。要记笔记。
- 每个成员都应该提出风险或者关注点；当每个人都说出来之后，大家一起群体协作来化解这些问题。即便有些关注点已经被提出来了，也鼓励其他人提出来；这样有助于团队排出任务的优先级，识别出那些最应该花时间来解决的问题。这是一起讨论如何改善我们共同构建的流程和产品的机会。记下来谁提出了哪些问题，以及我们如何解决这些问题。
- 庆祝成果。回顾上一周已经交付的工作，展示真实的产品，并祝贺做出了这些成果的人。
- 回顾完成之后，和团队分享会议记录，并确保回顾中提到的所有动议都被记录了下来。这样做会让团队看到进展，理解到对产品的感受是如何随时间变化的，以及从回顾中看到的产出对未来设置的目标充满信心。

回顾笔记看起来像是这样的：

Joel

- last week
    - felt like it went by extremely fast
        - first couple days, thinking through the project, understanding
        - didn't feel like we got much implemented in code
        - feel great about knowing what we're building
- this week
    - feeling confident

Ryan

- last week
    - fast-paced with understanding, overwhelmed with the complexity
    - towards the end of the week with prototyping and iteration, it helped a lot
- this week
    - feel much better than start of last week
    - brainstorming + prototype helps a lot

Yadid

- last week
    - flew by, felt like it didn't happen
    - progressed a lot
    - defining the interaction was really important
    - confident moving forward with what we decided upon
- this week
    - time is worrying
    - user study, potentially risky

Concerns

- timeline - it's a tight project (JQ, RC, YA)
- concerned with choice of technology with vanilla Rails (JQ, YA)
    - lots of state involved
- concerns around interaction and not specifically the visual design (RC)
- testing (potentially won't change outcome) (YA)
- need a staging server (JQ)
    - don't want to connect to real API
    - in dev+test we've created a fake API that we're connecting to
    - can't do that on Heroku

Addressing concerns

- Yadid to set up a staging server for the app to interact with
- Ryan to do a quick run-through with Yadid re: interactions
- Josh to look into Omar rotating on

产品所在的阶段会指导计划会议。例如：

- 调研和确定：用户界面是不是已经足够确定，可以用来开发一个最小可用版本了？
- 产品可用性：用户可以在线上部署版本中完成流程吗？
- 用户获取：这样的流程之后获取的用户数字看起来是怎么样的？

给客户讲用户故事，人们喜欢这个产品吗？展示数字。和上周相比，本周是不是有更多人在使用这个产品了？同一个人是不是用的更多了？

在所有阶段，我们应该问：

- 我们在创建正确的产品吗？
- 基于预算，我们还剩多少时间？

基于这些问题的答案，我们在任务管理系统中记录我们的计划：

- 归档两周前的「Live (Week of [date])」列表。
- 审阅产品设计优先级。将我们认为合适的任务拖动到「Next Up」
- 审查缺陷。将所有严重缺陷拖到 Next UP 并将放到队列的顶端。我们总是优先修复缺陷。
- 审阅工程和重构任务。基于以上的产品和缺陷任务，将设计师和开发人员觉得合适的任务拖到 Next UP。
- 根据优先级再次整理整个 Next Up 列表。上周位于顶端的卡片可以拖动到底部或者拖动到其他的看板或者列表。

任务管理系统是计划的正式归属地。

当信息是在电话中谈论、面谈、在没有包含全体队员的邮件中或者是一对一的聊天中时，信息就会丢失、忘记或者被误解。当有人加入或者离开问题就会扩大。

在这个会议中，试着和客户讨论，而不是获取指示。如果我们没有发现底层问题是无法谈论解决方案的。

我们被称为「强势」，我们的方式是裁剪需求，预算，以及时间表。我们经常说「no」。说「no」是不容易的。「no」也不是那么容易被接受的。客户提需求也是有原因的。

我们需要和「yes」作斗争，我们能做到这点是因为我们理解了软件开发成功和失败的历史：在 2004 年只有 34% 的软件项目被认为是成功的。好消息是这已经比 1994 年的情况好 100% 了。「主要原因是项目变得小了很多。」

很少有软件项目失败是因为做的不够多。说「no」意味着保持我们正在构造的软件足够简单。我们写的每一行代码既是资产也是负担。

当简单的软件发布后，更容易改进来满足客户的需求。复杂的软件，即便是发布后，也很难快速响应客户需求。

[原文链接](https://thoughtbot.com/playbook/planning/meet-weekly-to-discuss-successes-failures-and-plans)
