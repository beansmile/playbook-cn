# 主机托管

我们使用[Heroku](http://heroku.com/)。它是一个构建在Amazon的云平台上的PaaS平台。它非常易用，无论是我们的应用只是一个玩具项目，还是高并发高负载应用，它都能应付自如。

像Rails一样。Heroku使用约定，这样它就可以做一些我们不要费神的决定。像web服务器和应用服务器这些都无需我们费神了。

他们就像是我们外包的运维团队。我们可以花时间在产品上而不是解决基础设施的问题上，这些时间和购买基础版的 Amazon Web Services省下来的钱比起来是值得的。

云服务提供更低的运营成本，尤其是刚开始容量比较低的时候。忘记那些昂贵服务器的沉没成本。

云服务使得我们客户可以用以前不可能的方式开始运营生意，不用投入大量的前期成本。

如果我们需要提供上传功能，例如用户头像，我们上传到[Amazon S3](http://aws.amazon.com/s3/)。

我们还将图片、CSS以及Javascript资源存储到CDN上，例如[Fastly](http://www.fastly.com/) 或者 [Cloudflare](https://www.cloudflare.com/)。

[原文链接](https://thoughtbot.com/playbook/production/hosting)
