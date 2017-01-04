# 使用轻量级程序来管理任务优先级并可视化流程

多年以来，我们用过 JIRA、Pivotal Tracker、Lighthouse、Basecamp、Trajectory、Unfuddle 以及其他任务管理系统。下面以 Trello 为例详细展示整个流程，不过即便使用其他系统，整体的流程也是极其相似的。

没有两个产品是一模一样的，所以产品开发过程中的灵活性非常重要。Trello 在调整流程结果方面做得可谓「极速」。

Trello 看板是一个贴满一列列便签纸的墙壁在软件世界中的呈现。在 Trello 的术语中，墙被称为「看板」，列被称为「列表」，列中的便签纸被称为「卡片」。

![alt](http://beantalk.net/static/upload/201610/_D6F8A1LLF-BoAent1fDmgX5.jpg)

在下面的图片中，「Current」是一个示例看板。「In Progress」是一个示例列表。「Confirm Internet Explorer support」是一个示例卡片。

![alt](http://beantalk.net/static/upload/201610/HgSlxUpcLuaD7ThZnK-boLvJ.jpg)

在任何任务管理系统中，有这样一个产品开发流程视图非常重要。「Next Up」列表是唯一一个排序的列表，产品团队根据顺序得知下一步要做什么。它代表了一周的工作量。

卡片代表了一个工作故事、缺陷修复、工程任务或者一个普通的待办事项。

卡片以一个简单的想法开始，一两句话的描述。当它们在不同的看板间拖动时，人们会添加细节，（从商业角度）解释为什么我们会关注它，以及一些实现上的建议（虽然设计师和开发人员会从他们的角度来留下或者考虑接受意见，但应该从有助于项目的角度来做，而不是片面地发表意见）。

![alt](http://beantalk.net/static/upload/201610/rwjeWpxoKqt2oHdsBmUk6jvB.jpg)

一旦在「Next Up」列表中的卡片被排序并检查过，就可以针对它们进行设计和开发了。设计师或者开发人员通过「把自己的头像放在上面」来将任务指派给自己，并把卡片拖到「In Progress」列表。

在「In Progress」列表中的卡片是活跃的任务，在进行设计或者开发。规则是你不应该在两个以上的卡片上同时露面。工作在一个功能分支上完成。

当设计师或者开发人员为他们的功能分支创建一个 pull request 时，他们将卡片拖动到「Code Review」列表。评审人在评审时要「将自己的头像放到卡片上」。

每个人都有权限合并功能分支到主分支。

在 Testing 和 Staging（或者 Testing 以及 iPhone app 的 Ad Hoc build）上的卡片被部署到 Staging（或者通过 HockeyApp 分发 iPhone app），卡片的创建者和设计师来检查还原度以及用户体验。

每个人都有权限部署到 Staging。

在「Ready for Production」这个列表的卡片包括在 Staging 上被接受的卡片，它们可以被部署（但不一定发布）。

每个人都有权限部署到 Production。

在「Live（Week of [date])」列表上的卡片已经发布。每周都有自己的「Live」列表，所以我们可以知道什么时候发布了什么。

[原文链接](https://thoughtbot.com/playbook/planning/manage-priorities-with-a-lightweight-process)
