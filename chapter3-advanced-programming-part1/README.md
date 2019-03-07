# Chapter 3 - Programming Advanced - Data Structures and Algorithms

Let us first look at the definition of data structures and algorithms on Wikipedia.

> Data Structure is the way in which data is stored and organized in a computer. Often, carefully chosen data structures can lead to algorithms that are optimally efficient.

> Algorithm refers to the specific steps and methods required to complete a task. That is to say, given the initial state or input data, it is possible to derive the required or desired termination state or output data.

The algorithm and data structure are the rhetoric and layout of the program. Although human programming has only been for decades, the problems solved by the application have covered every aspect of the world. Various problems were summarized by seniors and masters. Some people directly found solutions. Some people found ways to find solutions. Some people simply proved that it is impossible to solve them at this stage. The solution is collectively referred to as an algorithm. Learning algorithms is to learn the wisdom of predecessors and to take less detours. Zen has a cloud: not taking a detour is a shortcut! ! ! Even Newton Jazz is standing on the shoulders of giants, unless you feel better than the old cows, you can solve the problems that others have been thinking for more than a decade. To illustrate this relationship more vividly, let's play a classic math game:

> There are three bottles with capacities of two liters, three liters, and seven liters. Now it is necessary to quickly and accurately measure six liters of water. How can I get it?

Obviously we have to combine these three bottles to get an accurate six liters of water. How do we get it? I think smart, you must have an answer soon. The next question is how to use the algorithm to express it? - This is testing our mathematical thinking ability. The abstraction of the problem of bottled water is actually a problem of finding the integer solution of the polynomial equation of the integral coefficient. OK, click here.

According to the definition of data structure on Wikipedia, we can compare the bottle with water on top to the data structure - the bottle is filled with water and pour water under human intervention, through three steps - your algorithm, and finally It achieved six liters of water in a seven-liter bottle. It takes six bottles of water to get six liters of water. This kind of thing is definitely not something that smart people think of, so what would a smart person think? - Finding a six-liter bottle is not a step! So sometimes it is important to find the right data structure...

The predecessors have summed up a lot of algorithms and methods to generate algorithms, we can learn directly. If you are aggressive, one day, you will find that you need to create innovative algorithms yourself. At this time, mathematics will help you a lot. Maybe just a math tool is working, but it's more likely that your brain is trained in mathematics to help you. In short, for the sake of the future, it is right to improve mathematics literacy. This is not to say that there are more mathematical formulas and more math problems, but rather a kind of mathematical thinking.。**

学算法很简单，也是找教材，做习题。教材容易找，但新手往往找不到合适的习题。可以尝试在完成教材上的所有习题之后去找编程竞赛的练习题来做,也就是所谓的 [Online Judge](http://en.wikipedia.org/wiki/Online_judge)，后续将深入讨论这个东西。

## 算法+数据结构=程序

> *Algorithms + Data Structures = Programs* is a 1976 book written by Niklaus Wirth covering some of the fundamental topics of computer programming, particularly that algorithms and data structures are inherently related.

算法与数据结构的基本概念已经在上文介绍过了，这里再稍微深入一步探讨，对于新手来说不必在本小节纠结过多，本节的存在一方面是为了本章的完整性而充实的，另一方面可供有一定基础的人参考。

实际上，数据结构与算法解决的问题是整个编程中最有限，最底层的那些问题，(它没有涉及到设计，用户等编程三层架构中的最重要的后二层)。它只解决对于计算机在组织内存,支持对这些内存中数据进行操作(排序，查找)等有限问题的问题，它仅仅能很好地解决这些问题，所以说它是面向计算机的功能性方案，是计算机的科学，解决对于计算机来说最为迫切要解决的那些问题，比如效益敏感类问题。如果放在整个大编程中来讨论，那么它是颇为有限的那类东西。

承载计算机科学最最根本的东西，是数据结构跟算法，而不是语言(语言只是表达工具)。难怪宏大的 [TAOCP](http://zh.wikipedia.org/wiki/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1%E8%89%BA%E6%9C%AF) 写的几乎全是数学和算法分析等内容，跟语言相比，语言本身并不能解决一个问题，它只是反映事物的工具，跟解决问题没有绝对的联系，数据结构与算法才是“真正能解决”计算机问题的手段与技术。你看路由器算法，这些底层的东西，都是数据结构与算法发挥作用的地方。

于是，当用数学和机器的眼光直面解决问题的时候，很自然地就产生了一门学科，即数据结构和算法。

**算法与数据结构实际上就是计算机编程界将应用问题离散化建模的方案，这样，就可以将应用问题转化为软件上可用的抽象，而所有一切软件上的问题，不过都是抽象。** [[1]](#ref1)


## 不会Coding如何破？

「能看懂别人的程序，但自己就是写不出来，Why？」——这个问题其实每个刚开始学习编程的人都会遇到，你所见到的各位达人大牛都曾经有过这么一段经历，所以完全不必为这种情况而怀疑自己的能力。为什么会有这样的情况出现？——因为思维模式。

在小学的数学教材里，有一种题型，叫应用题。它会给出很多生活中的场景，然后让你用数学知识来解决。在解这种题时，其实分为三个步骤，首先是要提取出数理模型，比如常见的追逐相遇这类问题，就要使用速度时间模型，然后把这个模型数学化，找出各个变量之间的关系，确定已知量和未知量，形成可求解的方程，最后求解。

编程的情况与此类似。首先要建立一个抽象描述模型，然后建立数学表达，接下来略有不同，不是亲自求解，而是给出求解的方法——也就是算法，最后是把算法转化为程序。而新手通常之所以会卡壳，是由于这个流程中有两个难关。建立模型不是问题，数学表达也不难，但找出算法却是非常艰难的事情，即使找到正确的算法，要把它写成正确的代码也不容易。新手常说我在学习XX语言,XX语言真复杂啊。其实学习语言本身只能保证你在最后一步，也就是翻译代码（又名coding）那里少出错误，即使你顺利的学习了一万种语言，你也会觉得编程很难，假如你没有学习算法的话。让我们找个具体的例子来说明，假设现在有个题目要找N个正整数中的最大值。显然这个题目模型很清楚，本身就是数学问题，也不需要数学表达了。接下来就是解法，新手这时就卡在这个地方了。

刚接手这个题目，很多人就会想用一种类似人类的快捷操作，比如三个数，瞥一眼就可以找出最大值，四个数也毫无问题，甚至十个数也是一下子。这时我问你，你怎么把这个瞥一眼的动作表示成程序，另外如果N大于10000怎么办？——哑口无言。原因是，人类的头脑过于聪明，可以同时处理很多事务，也就是可以并行处理一定量的数据（当然大规模数据就要另外对待）。而计算机——很遗憾，这方面的能力有所欠缺。这个时候你肯定会说：「现在不是有多处理器多核多线程等各种各样的并行处理的计算机了么？」我要告诉你，那些都是不同层次的概念。

目前这个时代的计算机，在出现革命性的变化之前，从CPU指令的层次来说，都是单线程单参数工作的。再说明白一点，这些机器任何时候只能一次处理两个数，而且其中一个还必须已经在CPU内部了，任何N>=3个数相加都必须转化成持续的两个数相加，就是先把第一个第二个加起来得到结果之后，才能和第三个相加，照此重复求得所有的和——这是目前的科技无法改变的铁律。这个时候我要请你记住一个重要的思想：编程中任何问题都要分解到足够小，小到机器可以一次解决的程度！当然，这不是意味着我们每次编程都得从CPU执行一次指令的角度去解决问题。

回到刚才的那个题目：寻找N个正整数中的最大值。我们知道直接解决是不可能的。而按照刚才讲过的铁律，我们知道直接找到两个数中的最大值是一次可以做到的。那怎样从2个扩展到N个呢？这里就是算法的天下了。一种很常见的想法是，完全可以从两个中找出最大值，再让它和接下来的一个比较，这就是N=3的情况，再把三个中的最大值和第四个比较，这就解决了 N=4，依此类推，我们似乎找到了通用的算法。是的，找到前N-1个中的最大值，然后与第N个比较——不要怀疑，这个算法方向是正确的。接下来就是把它细化使他能变成代码。

你注意到，首先要设法从1增加到N，而且每次前进一步都要做类似的操作，显然可以用一个循环来实现。每一次循环中，都需要将保留的最大值和当前的这第n个数比较，如果最大值比它大，那就保留，否则就要把最大值替换成新的——这就是条件语句的作用了。写完这个循环之后，还有些小细节，比如这个最大值在与第一个数比较之前应该是多少呢？太大的话，可能会比整个数列的数都大，这就会出问题。因此常用的做法是，就让他等于第一个数。然后包括读入那N个数，而输出最大值这些琐碎的细节就属于收尾工作了，没什么可多谈的。当然，即使是这样的小题，也不仅这一种算法。

你记不记得有一种叫做单淘汰赛的机制——最后顶点的就是最大值。用在这个地方正合适。不过，如果要把这个淘汰赛算法实现成程序的话，如何实现分组，如何表达这个淘汰过程和取出顶点的值，正是算法描述里要解决的。这个就是排序里很有名的最大堆排序。<a name="sec-coding"></a> 一旦算法（伪代码）描述齐备，程序编写不过是打字校对的工作。

为什么你可以看懂别人的程序呢？——因为他的算法隐含在程序中已经被实现了。就像你读王维的诗，总能在眼前浮现出一幅幅绝美的风景画，但轮到自己写，却描绘不出那样的画面。一方面是因为你束手无策，不知道怎样找到可实现的算法；另一方面是即使你找到了算法，也只是爱在心中口难开，不知道怎样去表达。

算法总是从问题出发，通过一定的模式，逐渐细化再细化，直到可以直接转成程序。新手很难一下子领会什么样的算法是可以实现的，但好在新手接触的问题一般不是很难，算法通常非常清楚明白，所以重点是要解决后面那个怎样把算法表达出来的问题。因此在这里建议各位新手默写教材上经典的例题程序。很显然对于那些例题，只要你用心看过就会领会它的算法。那么，你再默写一遍，即使和它的原程序样子不一样，也总算是把这个算法表达出来了。反复这样练习，这个表达问题不就解决了么？而且在这个过程中，至少你学到了一个算法。基于此原则，任何你遇到的可以看懂的例程（当然要是好的例程才行），都建议你默写它——尤其是开源的精品代码。


### Notes

1. <a name="ref1">[1]</a> 本小节内容引自 [算法+数据结构的本质 | 兮软](http://dev.gameres.com/Program/Other/bcxszyforgameres/bcxszy/xisofts.sinaapp.com/@p=104.htm)，该书完整版见[编程新手真言Ver3.0](http://dev.gameres.com/Program/Other/bcxszyforgameres/bcxszy/xisofts.sinaapp.com/@p=5.htm)
