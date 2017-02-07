# 交易处理

对于信用卡和借记卡收款，我们使用 [Stripe](http://stripe.com/)。它是一个支付网关，也提供商家账号。我们也用它来实现订阅模式收款。

Stripe 的收费和使用方式有关。信用卡交易成功之后收费 2.9% + 30 美分。没有开户费，月费或者信用卡存储费。

向用户的银行账号付款时我们使用 [Plaid](https://plaid.com/)。

[原文链接](https://thoughtbot.com/playbook/production/payment-processing)
