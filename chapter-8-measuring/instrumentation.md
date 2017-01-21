# 度量

为了稍后分析指标，我们需要度量应用来记录恰当的指标。我们最关切的度量类型被称作「事件追踪」。

尽可能使用 [Segment](https://segment.com/) 来捕捉事件。它类似分析服务的[适配器模式](http://sourcemaking.com/design_patterns/adapter)。

Segment 为 web 应用提供一个 JavaScript 库，为服务端框架提供一个库，为移动应用提供一个 SDK。这让我们可以启用不同的服务，例如 Google Analytics、Amplitude、FullStory、Intercom 等等。

![alt](http://beantalk.net/static/upload/201611/2ctuEDKgHPl71dDFKI5-YAxH.jpg)

当 Segment 不支持一个后端服务时，我们可以直接使用这个服务，或者为 [Segment 开源库](https://segment.com/libraries/analytics.js)提交对应的支持。

事件追踪最难的地方是[选择事件的粒度](http://qr.ae/GBPdx)。重建度量历史是很昂贵的，而且错误的结果会杀死一个早期产品，所以：

- 当事件出现时就及时追踪
- 对于数据来说宁多勿少
- 对每个事件尽量囊括所有状态
- 从开始就记录数据

典型需要追踪的数据如下：

- 打开 App（移动应用）
- 后台应用（移动应用）
- 访问量（web）
- 创建账号
- 发起购买
- 添加内容
- 建立联系／好友
- 升级订阅
- 推荐朋友

充分使用各种事件属性，例如：

- 会话 ID
- 所有用户属性
- 环境：操作系统、应用的版本、设备硬件细节
- 当前电量、Wi-Fi、手机状态
- 会话持续时长，精确到秒数

[商业分析不必是实时的](http://mcfunley.com/whom-the-gods-would-destroy-they-first-give-real-time-analytics)，记录数据不应该让用户体验慢下来。所以，我们针对每个平台尽可能使用后台任务来执行这些任务。例如 [Delayed Job](https://github.com/collectiveidea/delayed_job) 和 [Resque](https://github.com/resque/resque)。

[原文链接](https://thoughtbot.com/playbook/measuring/instrumentation)
