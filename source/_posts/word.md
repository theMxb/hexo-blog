---
title: 名词
date: 2020-07-16 08:13:00
categories:
    - 前端
tags:
    - 名词
---

# SPA

**全称：**single page application，单页应用，动态地加载部分页面或者交互模块，与传统的网站最大的区别（不同的页面之前的切换都是直接从服务端加载一整个新的页面），常见的框架 React, Vue, Angular

**优点：**资源全部由前端控制，页面部分的交互切换非常快；减少服务端压力

**缺点：**首页加载会慢，首次加载需要下载spa框架及应用程序代码，然后再渲染页面；不利于SEO



# SEO

**全称：**Search Engine Optimization，搜索引擎优化，一种通过了解搜索引擎的运作规则（如何抓取网站页面，如何索引、如何根据特定的关键字展现搜索结果排序等）来调整网站，以提高该网站在搜索引擎中某些关键词的搜索结果排名

**搜索引擎优化的技术两大类：白帽技术、黑帽技术**

> 1、在每个页面实用一个短、独特的标题，描述内容，关键字，html文件中的<title/>标签，在[Google的相关文档](https://support.google.com/webmasters/answer/79812?hl=en)中已经说明了不再使用<title/>标签作为meta，但是经常会配合description出现在搜索引擎上
>
> ```html
> <!-- 标题 --> 
> <title>个人xxx的网站</title>  
> <!-- 描述，例如百度百科的一个词条description --> 
> <meta name="description" content="通常所说的META标签，是在HTML网页源代码中一个重要的html标签。META标签用来描述一个HTML网页文档的属性，例如作者、日期和时间、网页描述、关键词、页面刷新等。...">  
> <!-- 关键字, keywords --> 
> <meta name="keywords" content="META标签 META标签作用 META标签组成 META标签属性 META标签描述设计 META标签错误 META标签标签"> 
> ```
>
> 2、站点添加相当数量的原创内容
>
> 3、实用合理大小、准确描述的汇标，而不过度实用关键字、惊叹号、或不相关的标题术语
>
> 4、网址字眼，有助于搜索引擎优化
>
> 5、所有页面可透过正常的链接来访问，而非只能透过java，javascript，adobe flash应用程序访问，使用一个专属列出该站点所有内容的网页达成（如网站地图）
>
> 6、透过自然方式开发链接：Google不花功夫在这有点混淆不清的指南上。写封邮件给网站员，告诉他：您刚刚贴了一篇挺好的文章，并且请求链接，这种做法可能为搜索引擎认可。
>
> 7、参与其他网站的网络集团（译：web ring指的是相同主题的结盟站群）——只要其他网站是独立的、分享同样题目和可比较的品质。



# SPA和SEO的冲突

SPA不利于SEO，部分搜索引擎如Google、bing等，它们的爬虫虽然支持执行js甚至是通过ajax获取数据了，但是对于异步数据的支持还不够，[Vue SSR](https://ssr.vuejs.org/zh/)中是这样说的，接下来就是解决这个场景的技术 SSR

# SSR

**全称：**Serve-Side Rendering服务端渲染，可以将SPA应用打包到服务器上，在服务器输出html，发送到浏览器，输出的html不具备交互能力，需要与SPA框架配合，在浏览器上“混合”成可交互的应用程序。只要能合理地运用SSR技术，不仅能一定程度上解决首屏慢的问题，还能获得更好的SEO。

常用框架：React - [Next](https://nextjs.org/)，Vue - [Nuxt](https://nuxtjs.org/)

**优点：**更快的响应时间，不用等待所有的JS都加载完，浏览器能直接显示比较完整的页面；可以将SEO的关键信息直接在后台就渲染成HTML，而保证搜索引擎的爬虫都能爬到关键数据

**缺点：**相对于仅仅需要提供静态文件的服务器，SSR中使用的渲染程序自然会占用更多的CPU和内存资源；一些常用的浏览器API可能无法正常使用（需要对运行环境加以判断），比如<u>window</u>、<u>document</u>、<u>alert</u>等；开发调试会有一些麻烦，因为涉及了浏览器和服务器，对于SPA的一些组件的生命周期的管理会变得复杂

# JWT

**全称**：JSON Web Token，通常称为 `JSON令牌`，`RFC 7519`中定义的用于`安全的`将信息作为`Json对象`进行传输的一种形式。

# AJAX

**全称**：Asynchronous JavaScript and XML (异步的javascript 和 xml)

AJAX不是新的编程语言，而是一种使用标准的新语法，与服务端交换数据并更新部分网页

# 吞吐率

服务器每秒处理请求数

影响因素很多，如：并发策略、I/O模型、I/O性能、CPU核数、程序本身的逻辑复杂度等

# 外接项目站点

码市
猪八戒
开源众包
智城外包网
程序员客栈
实现网
猿急送
人人开发
开发邦
电鸭社区
快码
英选
upwork
freelancer
remoteok
dribbble
toptal
ange1list

# C/S B/S

**c/s**: client server客户端与服务器

**b/s**: browser server 浏览器与服务器

