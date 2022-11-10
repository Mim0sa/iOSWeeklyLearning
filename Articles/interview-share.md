# iOS 求职寒冬？听听他们怎么说

这是一次线上分享的文字整理版，视频内容可以点这里查看：[线上视频](https://www.bilibili.com/video/BV1gG411P7iu/?vd_source=f78da65b081aa6d30ae7bf2aded1d695 "本期分享视频内容")。

## 为啥会有这场分享

![](https://cdn.zhangferry.com/Images/20221030232624.png)

最近在帮团队招人，像朋友圈、脉脉、公众号添了不少推广信息，但能捞到的简历却很少，仅有的简历，能通过筛选的不足 1/3，可见招人之难。另一方面，现在找工作也挺难，因为今年被裁员的人有很多，很多公司还锁了 HC，市场整体竞争压力大。但这两个问题不应该一起出现才对，找工作人多，应该更容易捞到简历，更容易招到合适的人，然而事实却相反，这就很奇怪了，那这里面的 gap 到底在哪里呢？

最近正好有两个朋友都如愿找到了满意的工作，所以就拉他们来一起分享下面试经历。另外还邀请到字节客户端 APM 团队负责人东野浪子，让他通过面试官角度来帮我们理解招人的标准。互联网寒冬，iOS 更甚，处在找工作的节点又该如何应对，且听他们怎么说。

## 分享者介绍

![](https://cdn.zhangferry.com/Images/20221030232513.png)

### @阿卡拉

我是阿卡拉，毕业于郑州大学本科软件工程专业，2019 年 6 月进入腾讯。在腾讯主要负责的工作一直都是客户端基础平台建设，在工程效能方面不停的探索。我是国庆节前后刚入职的抖音。

### @JY

我是 JY，17 年毕业，是 iOS 摸鱼周报的联合编辑。我之前是在微盟的 App 基础技术部门工作、主要负责 APM 以及线上 Bug 排查等。因为公司裁员不得不重新找工作，目前是拿到了小红书的 Offer。

## 如何准备面试

![](https://cdn.zhangferry.com/Images/20221030232455.png)

### @阿卡拉

腾讯在 2022 年上半年就已经开始在慢慢的砍各种业务线，当时，对于我来说，感知比较弱，主要的原因是我一直在工程效能这一块，对于业务线的情况了解不是太多，仅仅是了解到外部的一些声音。

在 5 月 30 号，我们工程效能部门很多小组也开始在裁员，但是我们组的工具平台在最近的两年发展是挺不错的，这一次裁员没有涉及到组内任何同学。

或许是因为部门裁员的力度还是不够，接下来在 6 月 30 号开始裁员，我们组涉及到的有 16 个人左右，最后仅剩下 4 个人做日常维护。

在腾讯的这三年，我发现自己的能力提升是比较快的，从进入公司的小职员，慢慢到一个大的项目的负责人，这也得益于我的 leader 和身边同事的配合。所以，总的来说，并不是我要考虑换工作，而是公司的环境让自己被迫开始换一个工作环境。

公司有 2 个月的缓冲期，缓冲期阶段除了处理手里的交接工作，同时也让自己休息一段时间，对这些接踵而来的消息做一个消化。然后就开始了我的复习计划：

- 整理 iOS 基础知识（八股文）【计划是 2 个周，实际花费 3 周】
  - 计算机基础知识：主要是网络，操作系统等基础知识
  - iOS 的 dispatch：一直想把该模块的源码看完，但都是比较零散的，所以去看源码做了总结
  - iOS 的 dyld/objc：这个是 iOS 动态库加载的原理，所以需要去深入了解，objc 中包括很多的技术支持，如 autoreleasepool， 消息转发，AssociatedObject 机制。
  - Runloop 机制，KVO 与 KVC 机制，Block 管理机制，iOS 事件处理机制等等
- 整理曾经看过的开源库：自己之所以喜欢去研究这些源码，是因为他们给我代码能力提升了很多，无论是从设计上和实现方案上都能有比较好的选择。【计划 1 周，实际花费 2 周】
  - AFNetworking：iOS 网络访问最出名的网络库，没有之一
  - YYCache，YYModule等由 ibireme 大神的开源组件合集
  - CocoaLumberjack：也是 iOS 出名的日志库，整个仓库的设计将设计模式很好的应用
  - OCMock：这个是一个单元测试组件，但是如果想验证自己的基础如何，这个仓库我觉得是最佳开源库，可以将 objc 的很多知识点应用进去。
- 项目相关【计划 1 周，实际花费 2 周】
  - 单元测试自动化：整理整个单元测试的执行流程和之前的实现方案。
  - 质量组件化：熟悉自己开发的所有的 SDK ，包括语音 SDK，大文件上传 SDK，屏幕录制SDK 等等。
  - 变异测试：我主要负责的一个平台。变异测试的整理设计方案与之后的优化方向；梳理 Objective C 热重载执行方案与设计；LLVM 对 Objective C 语言的语法树分析并做各种能力；LLVM 的 pass 化服务梳理。
- 算法【每天早上刷算法】
  - leetcode 上刷「剑指 offer」第一版和第二版，然后刷 leetcode 热题 100（热题100要看着题目就马上写出来的那种）
  - 回忆算法：主要是算法小抄和这个作者的网站：https://labuladong.github.io/algo/

总结下来，整体上花了大概 1 个半月的时间，基本都是在腾讯的缓冲期每天静下心来一步一步的梳理。其中准备算法耗时最多吧，前后刷了差不多 300 题。

### @JY

我换工作的契机是因为公司裁员。在国庆节前两天，被通知 Last day，不需要交接。所以我是从国庆节前那几天才开始准备的。我主要准备的是简历，这里我的想法是需要明确自己想要去什么样的公司，然后根据公司要求和自己擅长的点，可以准备多份简历。简历里最主要的内容就是自己的项目经历，项目最好能体现出具体的优化指标。我面了很多家公司，都针对指标被问了一些具体的优化问题。

其次就是八股文，因为我之前有记一些笔记，再结合网上别人总结的一些内容，每天早晚都会大概看一遍。

算法这块，我在 Leetcode 上开了一个会员，这样能看到热门公司题库，我把想要面的公司的算法都刷了一遍，有些题目可能不止一遍。

这里最耗时的就是算法这块了，有些 Hard 级别的算法题很难写出来，也会花费不少时间。所以如果算法比较弱的话，需要多刷一刷找找题感，才能更好的应对各种复杂的问题。

## 如何写简历

简历是面试过程中的敲门砖，只有简历通过，才会有后面的面试过程，所以它的优先级是很高的。很多人都有分析过简历应该怎么写，不应该怎么写，但讲再多都不如亲自去看一下优秀的简历是什么样的。下面是阿卡拉和 JY 两个人的简历，部分内容做了脱敏处理。

### @阿卡拉

![](https://cdn.zhangferry.com/Images/20221031231150.png)

### @JY

![](https://cdn.zhangferry.com/Images/20221031231537.png)

## 如何获取更多应聘机会

![](https://cdn.zhangferry.com/Images/20221031231641.png)

### @阿卡拉

招聘渠道的话，小公司直接去 BOSS 上面找，大公司找内推。我对下个阶段其实考虑挺多的，结合自己的诉求，我主要有三个方面考虑：

1、大公司：字节，阿里，腾讯这一类的大公司，只要招聘的业务不是太偏就可以。业务上我希望继续在工程效能方向继续深挖。

2、有前景的公司，看中公司的进步和发展，看中公司的业务。

3、加班压力小的公司。

### @JY

我基本也都是通过 BOSS 或者内推方式，我会让朋友来面试我，培养自己的面感，这个过程也会一点点增加自信。因为现在大环境不好，很多大公司的 HC 都是很宝贵的，最好是准备很充分了再去面。

对于意向工作，我更关注的是该组是负责哪一块，是否是核心部门，公司发展前景如何。最重要的还有自身的发展方向和工作内容是否匹配。

### @zhangferry

找工作前需要考虑的这几个问题，第三个是非常重要的。不管因为什么原因需要换工作，都可以把换工作这个节点当做整个职业规划的下一个拐点。之前的工作有哪些不好，踩了哪些坑，要去避免；了解到哪些行业热点，对哪个领域感兴趣，都可以通过换一份让自己满意的工作获得。这一点容易被遗漏，但非常值得花时间去规划。

### @东野浪子

挑选工作时要提前想好自己的诉求是什么，更高的薪资？更看好的行业？想从业务开发切换为技术开发？或者就是想工作的轻松点，这都是没问题的。把这些诉求按照优先级进行排序，赋予不同的权重值，然后再分门别类的把你所能投的一些公司或者职位按照权重进行打分，分数最高的那个就是最适合你的岗位。

很多时候都不可能一个 Offer 覆盖你所有诉求，这时就可以利用这个方法论进行选择了。

## 如何进行面试

![](https://cdn.zhangferry.com/Images/20221101081818.png)

### @阿卡拉

我投的简历还是蛮多的，大概有十几家，最终进入面试环节的有七到八家，但是真正满足我那几个诉求的只有两到三家。我觉得寒冬的感受还是挺明显的，阿里、腾讯、大江、虾皮这些都已经不怎么招人了，因此可选的公司范围没有那么广。

技术面中基础知识，也就是我们常说的八股文还是比较重要的，也经常被问到。像是 Runloop、KVC/KVO、Objc、Block、GCD、Autorelease 这些技术点要非常清楚，每个点都需要深入。我自己在整理文档的时候基本也是从这几个方向展开的。

总共走完流程的有 4 家，有两家因为薪资不满意，还有一家其实挺想去的，但感觉他的发展前景不太好，最终就选择了字节。不说别的，就薪资这一块，字节还是棒棒的。

最终通过面试感觉还是因为自己准备比较充足，比较全面，哪些相关的知识点，我会把里面的方法论也都提炼出来。比如说 Autorelease 或者 Cache 相关内容，我会考虑如何把他们应用到自己的项目中去。只有真真实实地去考虑了这个东西，而且了解它的各方面内容，面试官问你的时候你就会感觉很轻松。

关于这些知识点的学习，我还会分有很大比重去看开源库。说实话我觉得腾讯这边，很多业务代码拿出来，大家都不想去看的，这些东西不会给人带来提升。而开源库是经过社区检验的，都是质量非常高的内容，仔细研究，更能学到东西。

字节给我面试体验就是他们的面试深度，整个面试过程就是带着你一步步往深了聊，但这随之而来的就是难度提升，这也是我为啥会把面字节的面试安排放到最后。

### @JY

我投的简历不多，都是自己比较想去的才会投，除了两三家没有面试，其他都有。寒冬的感觉还是很明显的，因为我很多朋友去年找工作的时候，HC 很多，难度也不算高。今年因为有很多公司在裁员，有一些公司也锁了 HC，市面上人确实比较多，所以每次面试都应该把握好机会。

我在技术面上感觉稍微有些不同，一面遇到问八股的比较多，后面几面基本都是围绕项目在问。最经常被问到的就是你们团队为什么要做这个？为什么要采用这种方案？过程中遇到了哪些问题？你是如何去解决的？其次就是结果，带来了哪些收益，我感觉大厂的面试很像项目讨论会，双方就一个功能点不断地探讨，技术深度慢慢深化，这样整体面下来也会感觉比较舒服。

有一些没有走完的面试流程，可能是复习的时候没有准备到位，也有一些是平常工作中很少使用到的，因为答的不太好就被 pass 了。

面试通过的原因，我觉得主要还是平常的积累，平常做了什么项目，需要经常复盘总结。把遇到的问题以及收益都记录下来，组织自己的语言表达出来。

小红书整体的面试还是比价舒适的。整个面试都是从浅到深的，基本没有问什么八股，都是围绕项目开展的。

## 面试回顾及总结

![](https://cdn.zhangferry.com/Images/20221102221550.png)

### @阿卡拉

面试中踩过的坑，第一不要盲目面试，盲目面试会发现其实很多岗位都是不符合自己预期的，这些过程会有很多无效沟通，浪费了挺多时间。第二面试一定要做好总结，像是每次面试被问到的问题，如果我不知道或者感觉答的不好，下面我会再去总结和调整，短板补充是一个比较重要的提升过程。

面试对我还有一点改变是，因为在腾讯这三年都没有考虑过面试这件事，一直是比较佛系的状态，这次面试经历基本是反向的去提升自己的能力。因为面试的缘故我有充足的时间去系统的学习之前遗漏的知识点，并为下个阶段做一个规划。

如果面试不顺的话，就当做跟这家公司没有缘分吧。选择是双向的，我经常跟一些同事开玩笑说，在腾讯小马哥拥有我是他的幸福，而不是我的幸福。现在在字节也一样，他拥有我是他的幸福，但反过来对我来说，也促成了我的幸福。

关于选择这块，因为在腾讯时组内相处比较和谐，我也更倾向于氛围和谐的团队，工作和生活都要做最真实的自己。另外我觉得大家还是要选一个自己感兴趣的东西，一直坚持做下去，丰富自己的生活。

### @JY

踩过的坑是，简历一定要写自己熟悉的（至少能够展开来讲的），不要写一些不是很熟悉，或者临时抱佛脚的东西，一旦被面试官问到，会很影响在面试官心中的印象。面试的时候，如果可以的话，就把面试官引到自己的舒适区，因为每个人技术侧重不同，这样的话更能体现你的优势，这样面试成功的几率也会更大。

面试过程做的特别对的事情是，我每次面试都会录音，面试完会听着录音进行复盘。有些人可能觉得自己面完感觉很不错，但有时候自己再听一遍时会发现自己有很多可以改进的地方。

做的不错的地方是调整自己心态吧，刚开始投简历的时候一个面试都没有，自己心态受到了一些影响，因为是被裁的，心情有些失落。然后我趁国庆节，前三天，出去旅游了一下，回来就放松下来了，再去调整心情，安心准备复习，这样效果会好很多。

换工作的话，主要是看公司能否满足自身发展，因为我们换一份工作一般都是期望工作一年以上的（大家肯定不希望自己简历花掉），如果这段经历跟自己不匹配，那整体工作状态可能会不开心。另外像阿卡拉说的，团队氛围，可能进入团队之前会比较难判断出团队氛围好不好，一般二面或者三面就是你的领导，这时你可以看你自己的感觉和面试官契不契合，也可以先以是否符合自身发展为主。我接触的程序员都是蛮好相处的。

## 如何筛选候选人-面试官角度 @东野浪子

![](https://cdn.zhangferry.com/Images/20221106214853.png)


我简单自我介绍下吧，我是 15 年毕业，16 年开始做面试官，我刚看了一下面试记录，这些年来总共面试了大概有 570 多位候选人。我现在是在字节的客户端架构部门下的 APM 部门，带客户端团队。

### 好简历体现在哪里

先说第一点，作为面试官视角，第一眼关注的是你的硬性指标：学校、工作经历、技能匹配程度。重点大学和大厂经验会是加分项，另外还会去看你的技能匹配程度，如果你之前是做基础技术的，你应聘的也是基础技术，这就属于比较匹配。

但是如果你的这些条件都不算出彩的话，就需要用项目经历去弥补了。对于项目经历的整理和描述要条理清晰，可以使用 STAR 法则，我做这个东西的背景是什么，基于这个背景，你的目标是什么，你通过什么行动达成了什么样的目标，最终一定要有结果，而且最好是可以用数据量化的结果。项目中要突出重点，一些重要的结果和数据，可以使用加粗的形式去强化。

简历也可以体现个人风格，我看过一些简历，一看就知道这个人非常的极客。因为它里面有非常多的专业术语，能明显感觉出他对技术的理解非常深刻。如果你面试的是基础技术部门，那就应该在简历里多写一些你在底层技术的探索，或者你在技术优化上做过的一些事情。这些都是简历相关的内容。

### 好的应聘者需要具备哪些特征

对面试阶段候选人的表现，最重要的就是基础一定要扎实，基础决定了你以后的发展潜力，甚至决定你在职场中的天花板。这里基础又包括很多方面，比如计算机基础、操作系统原理、网络等等，这些东西一定要多查漏补缺，不要有明显硬伤。这一点如果表现不好，那肯定是过不了面试的。

再就是数据结构和算法，有一点需要澄清下就是不要畏惧算法，至少在我们团队算法考察最多就是 medium 级别，不会在算法层面太为难大家。很多同学面试挂掉，如果把结果归结于算法没写好，是需要纠正的。因为算法是作为一个侧面角度考察的，一般不会直接决定面试结果，如果你自认为是因为算法没写好而没有通过面试，那可能你在算法之外的表现也没能征服面试官。

第二点是领域知识，做 iOS 开发对苹果开发相关的比如 UI 动画、多线程、内存管理、性能稳定性等都要有一定的了解。如果是做底层技术，你还需要掌握 dyld、runtime 相关的底层原理和常见的优化手段。很多人会把这说成八股文，我感觉更合适的是把它作为对你技能点的考察。这类问题通常的考察方式往往是从一个非常简单的问题切入，然后抽丝剥茧，逐渐加大难度，看你能够顺利的通过多少关。

第三点属于项目亮点，比如一个很常见的面试问题：你做过最满意的一个项目是什么，项目里有哪些亮点内容？亮点内容应该体现出一定的复杂度，你跟其他人的方案有什么差别，使用了哪些设计能力，涉及哪些技术选型，如何协作和执行的。同时也不能只谈难度不谈收益，它达到了哪些业务价值，你在这里承担了什么角色，是否是跨部门项目，这些方面都可以作为亮点去讲。业务价值描述时可以通过方案前后的对比来体现，之前指标是多少，使用该方案之后达到了多少，这种展现是非常直观的，更能引起面试官的共鸣，这个技巧同样也可以用到汇报工作和晋升答辩中。

软素质也会作为面试考察中比较重要的一点，因为应聘者最终会成为我的同事或者下属。我会比较关注自驱力，你对技术是否有好奇心，会主动地探索。然后是规划能力、沟通协作能力、迁移复用能力等。这些点比较多，如果无法通过一次沟通完全展示出来，那可以根据自己的需要选择一两个方面有体现也行。比如你想转技术栈或跨专业，那你就要说服面试官为什么之前积累的经验可以继续复用。

### 一些面试小技巧

![](https://cdn.zhangferry.com/Images/20221106214920.png)

对于没有把握的问题，不要不懂装懂，面试官会很讨厌不懂装懂的情况，这会严重扣分。还有就是对于你没有把握的问题，最好不要一言不发或者直接说我不了解。如果遇到了这类问题可以尝试从自己熟悉的角度切入，或者给出一个简单版本的答案。

第二个技巧是不要在面试过程中与面试官发生冲突，有可能他老问八股文，你感觉面试官在刁难你，或者你觉得面试官很菜，无论如何都不要起冲突。因为一般面试都会有面评记录，如果有冲突，这个事情被记录，后面会影响你再面其他部门，得不偿失。

还有一个技巧就是多复盘总结，很多人会有一个面试误区，感觉面试没发挥好，就不去想它了，而产生一些抵触情绪，这其实对自己提升是无益的。一定要有复盘，也可以跟小伙伴一起讨论自己的面试情况，避免自己有认知偏差。因为有时候我们感觉自己回答的很好，但最终却没面上，有一种可能就是你回答没有达到点子上，或者回答的比较浅显，跟面试官期待有偏差。

### @zhangferry

对于软素质，我感觉它体现了一个隐藏因素 — 兴趣，有了兴趣做驱动，才会有自驱力，才会去主动探索。很多人对编程，对开发是不感兴趣的，只是把它当做挣钱的一种手段，这没什么不好，反过来完全出于兴趣，敲代码时快乐的不得了的人也很少。不管怎样的状态，工作中还是应该尝试去找些让自己兴奋起来的点，比如解决了某个技术问题，老板给我金钱奖励；写了一篇文章，提高自己在技术圈的知名度；在团队做了技术分享，获得同事的赞扬等等。这些跟技术联通的点和个人成就感结合起来，就能激发兴趣，从而更好的提升个人的创造性。上班很辛苦，但不应该只有辛苦，毕竟这份工作我们还要再做几年甚至几十年都有可能，一直都处于不开心的状态其实是对自己的惩罚。怎么去找激发自己兴趣的那个点，需要每个人结合自身情况多想一想。

## 面试结果由什么决定

![](https://cdn.zhangferry.com/Images/20221105234741.png)

@zhangferry：本次分享的目的是给大家提供一些值得借鉴的面试方法，其实刚才也聊了很多面试之外的事，包括如何挑选岗位，如果在工作中补足自己学历或者经历的短板。回到一个比较重要的问题上，一次面试，我有多大概率能够成功。我认为，日常工作经验和总结占 60%，面试准备占 30%，面试相关的技巧和运气占剩余的 10%。平常工作所积累的经验是最重要的，除此之外通过充足的准备并结合一些技巧，面试就轻轻松松了。还有一点就是运气，考察的都是我准备的题，那运气很好；通过了所有面试但 HC 锁了，那运气很差，这真没地方说理去，运气无法改变，但可以通过前面的准备增加通过的概率。

还有一点想要强调的是，有不少人会在准备不充分的情况下去面试，这个其实是挺不好的。因为现在外面面试机会真的不多，每次面试机会都是非常宝贵的，一定要珍惜。以字节为例，不超过半年的面试，面评记录会一直留着。如果你之前面试效果不好，那后面你准备充分了，换个部门去面，就很大概率会因为面评不好直接被刷下来。我遇到过好几次这种情况，有些人会说不知怎么简历被 HR 捞到了，然后电话联系要约面试，自己稀里糊涂就参加了，结果没面好。如果遇到这种情况，一定要以自己实际准备的情况来决定是否要参加面试。

## QA

### 遇到面试就紧张，脑袋空白，面试过程不会吹怎么办？

@东野浪子：紧张背后的原因大多数情况就是准备不充分，导致不自信，我们应该从这个方面去解决紧张的问题。充分的准备就是上面说的一些基础知识，领域知识，要非常熟悉；涉及项目经历这块则可能需要更长期的准备。比如日常工作中主动承担一些有挑战性的业务，对一些技术问题进行深入探索。这些点都是面试过程中可以让自己出彩的地方，所以工作的一部分也是在为自己的简历打工。

不会吹可能侧面想说的是不会表达的意思，面试很强，实战一般。比如有些人实力是 60 分，他能说成 80 分，而有些人实力是 80 分，因为不会表达，让人听起来只有60 分。这样的话，就需要培养一下自己的演讲或者表达能力了。这种能力在日常工作工作、汇报或者晋升答辩时都非常重要，这也属于面试考察的一部分，平时可以刻意得去培养锻炼一下。

### 写了两年 UI 怎么办，就做了基本的页面开发，感觉项目经历很空洞

@东野浪子：如果一直重复一种开发模式，那确实不太好。你可能很难改变开发的需求，但是使用什么样的技术却是没人会限制你的。即使是开发 UI，从 Frame、Autolayout、Masonry 再到 SwiftUI，包括 RN 和 Flutter，这里都会涉及很多  UI 内容。不同框架的出现是解决什么问题的，怎么才能更适合当前工作且提高效率，这些都是自己可以延伸思考的事情。另一方面，你做 UI 会不会涉及到流畅性问题、会不会涉及一些 Crash，那这些问题都是也可以再延伸很多内容。所以即使复杂度不高的项目，也存在深入的问题，就看你有没有主动给自己增加难度，去做有挑战性的那部分。没有大厂经历也类似，没人会限制你学习大厂的技术，现在有很多途径去获取他们的技术方案，自己可以多学习，多思考，然后实践到自己的项目中。我们是非常欢迎这种有自驱力和主动性的同学的。

### 如何寻找自己的第二增长曲线

@东野浪子：第二增长曲线，往大了说比如你现在是一个程序员，这是你的主业，第二曲线就可能是一个副业。比如炒股、做新媒体、公众号、拍抖音等等。往小了说，比如你现在是 iOS 开发，你只会 OC，那 Swift 以后可能会是一个趋势，你能精通 Swift，那这就会成为你的第二曲线。比如你现在是做 UI 页面，做纯业务，那是不是可以去了解一些底层技术，像是 APM、DevOps、编译链接、端智能等，或者往跨端、全栈方面考虑，这些都是可以成为第二曲线的。第二曲线的东西一定要跟你的兴趣匹配，你要对它有热情，即使没有收益也能够坚持下去那种。

### 请问“横向协作能力，迁移复用能力”，这两个软素质一般会如何考察和作答？ 是否是先回答自己的方法论，然后举例来说明？

@东野浪子：横向协作能力，一般会在大型一些的跨团队合作项目中会有。比如我们是做客户端监控的，有些东西就会是一个双端方案。比如客户端上报流量，太高的时候后端会触发一些容灾或者限流，这个跟每个端的特性都没有关系。那如果作为这个项目的 Owner，你怎么把事情推进下去，怎么保证项目周期可控。他会涉及一些跨团队的沟通协作、目标对齐还有项目管理，这里体现的就是横向协作能力。

迁移复用能力属于比如你在一个领域 APM 做了很久，那现在需要专做音视频，相对于 APP 来说，怎么对音视频进行性能优化呢？这里有很多方法论其实是可以迁移出来再次适用的，像是线上容灾、问题响应、防裂化等处理方式都有一定的相似性。

## 内推信息

本次分享还有一个目的是信息互通，各位分享者所在团队都有招聘需求，以下是他们的内推信息：

| 内推人（微信）           | 岗位描述                           | 招聘需求                                                     |
| ------------------------ | ---------------------------------- | ------------------------------------------------------------ |
| zhangferry（zhangferry） | [北/上/杭]抖音iOS基础技术-研发效能 | 有静态分析、LLVM、单元测试、自动测试框架、架构、工程效率、全栈开发等经验者优先，有业务背景但对技术有深度追求者优先。 |
| 东野浪子（569087164）    | [北京]字节跳动 APM客户端-iOS       | 负责字节跳动所有移动端产品的性能优化和问题排查。北京还有 3 个 HC |
| 阿卡拉（myself439664）   | [深]抖音iOS基础技术-自动化测试     | 提升抖音等产品的研发代码质量，降低测试成本，参与自动化测试服务建设。 |
| JY（q491964334）         | [北/上]小红书-客户端基础架构       | 有过千万 DAU APP 的基础架构方面的开发经验，具有钻研 iOS 系统底层实现与优化的能力 |

对于内推岗位，我也维护了一个公共链接，[内推信息汇总](https://k27yiuwa7e.feishu.cn/base/bascnqNyF9TdWql6bxLD1LyfcUe?table=tbllqXuKIdww2xOj&view=vewzESLDQx "内推信息汇总")，大家如果有招人需求可以到这里来填写，编辑权限以开放。老司机技术周报很早就开始维护一份内推信息，会更全一些，可以点击这个查看：[iOS靠谱内推专题](https://www.yuque.com/iosalliance/article/bhutav "iOS 靠谱内推专题")。
