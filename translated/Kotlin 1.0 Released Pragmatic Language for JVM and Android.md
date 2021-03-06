---
title: "[译]Kotlin 1.0 Released: Pragmatic Language for JVM and Android"
date: 2016-02-15 16:57:00
author: Andrey Breslav
tags:
keywords:
categories: 官方动态
reward: false
reward_title: Have a nice Kotlin!
reward_wechat:
reward_alipay:
source_url: https://blog.jetbrains.com/kotlin/2016/02/kotlin-1-0-released-pragmatic-language-for-jvm-and-android/
translator:
translator_url:
---

就是这个。 1.0在这里
这是一个漫长而令人兴奋的道路，但我们终于达到了第一个大1.0，我们正在为您发布新的标志而庆祝发行：

{% raw %}
<p><center><img alt="Kotlin" class="alignnone size-full wp-image-3688" data-recalc-dims="1" margin-left="auto" margin-right="auto" src="https://i0.wp.com/blog.jetbrains.com/kotlin/files/2016/02/1_0_Banner.png?resize=640%2C320&amp;ssl=1"/></center></p>
{% endraw %}

<em>请参阅有关<a href="https://www.reddit.com/r/programming/comments/45wcnd/kotlin_10_released_pragmatic_language_for_jvm_and/"> Reddit </a>和<a href =“https：//新闻的讨论。 ycombinator.com/item?id=11103087">黑客新闻</a> </em>

{% raw %}
<p><span id="more-3507"></span></p>
{% endraw %}

## 什么是Kotlin？

Kotlin是JVM和Android的实用编程语言，结合了OO和功能特性，专注于<strong>互操作性</strong>，<strong>安全</strong>，<strong>清晰度</strong>和<strong>工具</strong>支持。
作为通用语言，Kotlin <strong>可以在Java工作的任何地方使用</strong>：服务器端应用程序，移动应用程序（Android），桌面应用程序。它适用于所有主要的工具和服务，如

* IntelliJ IDEA，Android Studio和Eclipse
* Maven，Gradle和Ant
* 春天靴（Kotlin支持今天发布！）
* GitHub，Slack甚至Minecraft

Kotlin的关键重点之一是互操作性和无缝支持<strong>混合Java + Kotlin项目</strong>，使采用更容易，从而减少了样板代码和更多的类型安全性。此外，Kotlin拥有一个<strong>广泛的标准库</strong>，使日常任务变得容易和顺利，同时保持字节码足迹 [低](http://www.methodscount.com/?lib=org.jetbrains.kotlin%3Akotlin-stdlib%3A1.0.0-rc-1036) （去做）。当然，任何Java库也可以在Kotlin中使用</strong>;反之亦然。
## 务实的意思是什么？

了解自己的核心价值观对于任何长期的项目都至关重要。如果我选择一个字来描述Kotlin的设计，那就是<strong>实用主义</strong>。这就是为什么在早期我们说Kotlin对发明或研究并不多。我们最终发明了很多东西，但这并不是项目的重点。当然，我们正在构建一个防止错误</strong>的<strong>类型系统，以及促进代码重用</strong>的<strong>抽象机制。但是，我们（务实）的方式是通过<strong>专注于用例</strong>使语言成为<strong>良好工具</strong>。
特别地，这种方法使我们立即引入与现有代码和基础架构的互操作性至关重要的概念。重新编写世界正确的方式</em>，从头开始 - 从来没有想过？我做了很多次:)而且，如果不是针对Java互操作，Maven集成，Android兼容性，Kotlin将会更容易设计和开发。在许多方面肯定会更加优雅。但优雅，虽然高度赞赏，但不是这里的主要目标，<strong>主要目标是有用的</strong>。而我们的用户不得不重新学习，重新创造，从头开始重新做，越能重复使用，越好。
那么，为什么Kotlin没有自己的软件包管理器或者自己的构建系统？</em> <br/>

 - 因为已经有Maven和Gradle，并且重新使用大量的插件对许多项目来说至关重要

 - 为什么我们投入大量时间和精力来制作JDK兼容的收藏界面？从零开始重新设计收藏集的容易程度越来越大？</em>

 - 由于吨和吨的Java代码与JDK集合一起工作，并且在边界上转换数据将是一个痛苦

 - 为什么Kotlin支持Java 6字节代码？</em> <br/>

 - 因为很多人还在运行Java 6（Android，最引人注目的是Android，而不是Android）。
对于我们来说，实用主义是关于<strong>创建用户体验</strong>，而不是单独的语言或图书馆。许多语言设计决策是在诸如“这不妨碍增量编译”之类的限制下进行的，“如果这增加了APK方法计数会怎么样？”，“IDE将如何突出显示此类型？”和许多更像这些。因此，我们为我们的<strong>工具以及语言</strong>感到自豪。
## 它是否足够成熟并准备生产？

是。而且已经有相当一段时间了。在JetBrains，我们不仅实施了编译器和工具，而且在过去两年中也在相当广泛的规模中使用Kotlin <strong>在现实生活中的项目</strong>。除了JetBrains，还有不少公司已经在生产中使用Kotlin </strong>了一段时间了。
事实上，我们花了很长时间才达到1.0的原因之一是因为我们特别注意在实践中验证我们的设计决策。这是有必要的，因为向前推进编译器将是<strong>向后兼容</strong>，未来版本的Kotlin不能破坏现有的代码。因此，无论我们做出什么选择，我们都需要坚持下去。
达到这个里程碑是我们在没有早期采纳者</strong>的有价值的<strong>帮助之前不可能做到的。我们要感谢你们每一个人的勇气，精力和热情！
## 谁在后面的Kotlin？

首先，Kotlin是开源语言

* 根据Apache 2.0开发GitHub开源许可证;
* 有超过100个贡献者日期。

JetBrains是Kotlin目前的主要支持者：我们投入了大量精力开发出来，而我们致力于长期的项目</strong>。我们将自己的需求写在我们自己的产品中。我们很高兴地说，到目前为止，<strong>接近10 JetBrains产品</strong>，其中包括IntelliJ IDEA， [JetBrains车手](https://blog.jetbrains.com/dotnet/2016/01/13/project-rider-a-csharp-ide/) ，JetBrains帐户和电子商店，YouTrack以及我们的一些较小的IDE和一些内部项目正在使用Kotlin。所以<strong>这里留下来</strong>！
自2012年以来，Kotlin的发展非常开放：一直与社区进行交流，收集和解决大量的反馈意见。
展望未来，我们正计划为设计方案和讨论设立一个集中的场地，使过程更加明显和有序。到目前为止，Kotlin的标准化工作尚未开始，但是我们意识到，我们需要比以后更早地做到这一点。
该项目的语言设计和总体指导由JetBrains聘用的团队完成。我们目前在Kotlin上有超过20人全职工作，这也是JetBrains对Kotlin承诺的另一个证明。
### 号码

我们来看看一些数字：

* 上个月，11K +人们在上个月使用Kotlin，上周只有5K左右;
* 数百个StackOverflow答案;
* 两本书：Kotlin in Action和Kotlin for Android Developers;
* Slack约1400人（获得邀请）;
* IntelliJ IDEA和Rider等项目中的Kotlin码超过500K行。

谈到代码行，GitHub开放存储库中的这些数量随着时间的推移呈指数级增长</strong>（JetBrains的项目被排除在外）：<center> <br/>
<img alt =“Kotlin GitHub Adoption”data-recalc-dims =“1”onmouseout =“this.src ='https：//d3nmt5vlzunoa1.cloudfront.net/kotlin/files/2016/02/KotlinAdoption.png';” onmouseover =“this.src ='https：//d3nmt5vlzunoa1.cloudfront.net/kotlin/files/2016/02/KotlinAdoption.gif';” src =“https://i2.wp.com/blog.jetbrains.com/kotlin/files/2016/02/KotlinAdoption.png?w=640&amp;ssl=1”/> <br/>
</center>
当然，我们也有越来越多的使用Kotlin </strong>的公司，包括Prezi和Expedia。顺便说一下，如果您使用Kotlin，请确保您向我们发送 [拉请求](https://github.com/JetBrains/kotlin-web-site/blob/master/_data/companies-using-kotlin.yml) 。
## 即将到来的路线图

从1.0开始，我们致力于语言及其标准库（<code> kotlin-stdlib </code>）的长期<strong>向后兼容性</strong>：

* 较新的编译器将使用较旧的二进制文件（但较旧的编译器可能不了解较新的二进制文件，如javac 1.6无法读取由javac 1.8编译的类）;
* 较旧的二进制文件将在运行时继续使用较新的二进制文件（尽管更新的代码可能需要较新的依赖关系）。

这仅适用于JVM / Android支持。 JavaScript支持现在仍然是实验性的，稍后会有自己的发行版。
对于计划，我们最近的目标是（除了错误修复）：

* Kotlin工具链的性能不断提高（例如，Gradle中的增量编译，现在正在进行）;
* JavaScript支持（包括在可能的情况下交叉编译为JVM和JS）;
* 支持使用优化的lambdas等生成Java 8字节代码（只要Android用户需要，将积极支持Java 6）。

工具更新和错误修复将作为增量更新发布，即1.0.X.更大的变化将首先通过早期访问计划（EAP），然后将作为1.1发布。
## 如何开始

使用该语言的最简单的方法是通过其<strong>在线迷你IDE：<a href="https://try.kotlinlang.org"> try.kotl.in </a> </strong>，其中包括 [Koans](http://try.kotlinlang.org/koans) - 一组介绍性问题，它们引导您完成语言的基础知识</strong>。
在您的机器上使用Kotlin（和Koans可以完成 [离线](https://kotlinlang.org/docs/tutorials/koans.html) ）：

* IntelliJ IDEA（终极或社区）：只需在Java项目中创建Kotlin项目或Kotlin文件;
* Android Studio：通过插件管理器安装插件;
* Eclipse：通过Marketplace安装插件。

注意：如果您运行的是较旧版本，则可能需要将Kotlin插件更新为1.0。
要了解概念的速度，可以使用语言<strong>文档和教程</strong> [官方网站](https://kotlinlang.org) 。我们社区成员提供的伟大文章和介绍可以在这里找到 [2015年摘要](http://blog.jetbrains.com/kotlin/2016/01/kotlin-digest-2015/) 。
如果您将Kotlin引入到Java项目中，您可以使用IDE中内置的<strong> Java-to-Kotlin转换器</strong>，帮助逐步轻松迁移。
最后但并非最不重要的是，请确保您加入我们的讨论 [论坛](https://devnet.jetbrains.com/community/kotlin) 要么 [松弛](http://kotlinslackin.herokuapp.com/) 。
再次，<strong>我们要感谢大家</strong>。没有社区，我们不可能做到这一点。
有一个漂亮的Kotlin！ <strong>现在</strong> <img alt =“:)”class =“wp-smiley”data-recalc-dims =“1”src =“https://i2.wp.com/blog.jetbrains.com /kotlin/wp-includes/images/smilies/simple-smile.png?w=640&amp;ssl=1“style =”height：1em; max-height：1em“
美国<em>请参阅有关<a href="https://www.reddit.com/r/programming/comments/45wcnd/kotlin_10_released_pragmatic_language_for_jvm_and/"> Reddit </a>和<a href =“https：//新闻的讨论。 ycombinator.com/item?id=11103087">黑客新闻</a> </em>
