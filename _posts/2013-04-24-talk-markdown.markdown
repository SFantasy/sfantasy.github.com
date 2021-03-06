---
layout: post
title: "王垠与「markdown的一些问题」"
comments: true
date: 2013-04-24 14:07
categories: Essay
keywords: markdown,王垠,GFM
description: 关于王垠“markdown的一些问题”的讨论
---

王垠一直是我很敬佩、甚至于崇拜的人，不过其实也觉得他是一个很「奇怪」的人--相信很多像我这样关注过王垠的人都会有这样的想法，当然，也曾在知乎上看到过一些人对与王垠的评价，地址在[这儿](http://www.zhihu.com/question/20102511)。

前几个月的时候经常会去王垠的[新浪博客](http://blog.sina.com.cn/yinwang0)上去看看他最近写的一些文章，不过最近突然发现他又把博客迁移到新的地址了：[www.yinwang.org](http://www.yinwang.org)。有兴趣的同学可以去看看他的博文以及一些思维导图，必然受益匪浅。

「markdown的一些问题」是一篇王垠博客中的文章，之前在他的新浪博客中没有看到过。毕竟平时也都是用markdown来写作的，所以结合以下他的这篇文章来谈一谈。

### 关于「markdown的layout语法」

所谓「layout语法」其实也就是使用缩进来区分代码块，这也是Python使用的方法。虽然这种语法会带来一些不必要的麻烦，比如因为少打空格而造成的格式混乱等;但是事实上在基本熟练使用这种语法之后就根本不会有这种困扰。所以对于markdown中这种语法而言，HTML这种标记语言必然是要败在下风的。

### 特殊字符的问题

markdown中的粗体是使用`**word**`，而斜体是使用`*word*`。其实王垠博客中提出的这个问题是很低级的：原文档中出现`x*y`这样的表达式。可以想像，如果只是按照单纯的文本将`x*y`写在文档中，那就很容易发生这样的事：原来想要写的是`x*y*z`但是却写成了x*y*z。「在程序员的世界里，“乘法”显然比“强调”更加频繁。」，没错，但是事实上markdown的语法给了我们用来表示代码的标记方法，如果要书写乘法，完全可以用之，而完全避免与其他诸如“强调”的语法的冲突。

### 表达能力

这的确是markdown的一个问题：比如图片的大小的控制，markdown无法做到，所以仍旧需要求助HTML的帮助; 再比如其实我很想在段首加两个空格的……

其实还有一个关于「表达能力」的问题，不同的markdown解释器对于一些标记的表达的支持不同。就举一个例子吧，比如代码块的实现上:

    ```
	code
	```

基本上都是支持这种形式的，但是有些markdown更为高级，支持高亮:

    ```java
	System.out.println("hello");
	```

如果习惯了后者的语法，再去使用前者，会突然发现代码之前多了一个`java`字样……着实难受。


不过在我看来，使用markdown来编辑文章、评论等都是非常cool的，至少比满眼的`<>`要舒服的多。至于关于王垠最后的那句话：「也许过段时间自己设计一个格式」，我只能说拭目以待啦。

--EOF--
