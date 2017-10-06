--- 
layout: post
title:  Elon Musk的A字思考法：如何深入思考一个问题？
tags: 
- learner
status: publish
type: post
published: true
---


# 1. 引子：千面之神

深入思考，显有成效的一个典型例子，就是Elon Mask。所以[我们看看他是如何思考的呢？][1] 一张图说明他与常人思考的差异，假设你要解构字母「A」，搞清楚构成「A」的深层原理，具体来讲，你有两种方法：

![][image-1]

以上两种方法，你认为哪种方法能更好地识别构成「A」的模式？

方法 1 中的每个「A」虽然各不相同，但给出了更多表现形式，能让我们识别出其中的模式。方法2中的「A」却不能给我们任何的提示。

当我们学习任何东西时，尝试观察许多不同的案例，形成自己的直觉判断，甚至建立自己独特的解读组合。

如何将以上方法应用到我们的日常生活呢？当进入一个新的领域时，我们不应该一上来就采用一种方法或采用最佳实践，而是应该探索多种不同的方法，解构每个方法，然后通过对比，发现其中潜在的底层原理。

这也是脑科学中的一条常识：人脑不善于在一个问题上深入思考，更善于在不同事物中找不同。相比于计算机，人可以快速地将两个不同之处找出来，人脑拥有强大模式识别能力。

**所谓知识，无非是信息。利用找不同，你可以在一瞬间，得出众多信息。**

他们称这个学习方法为迁移学习(learning transfer)。这也是为什么许多人，提倡主题学习，提倡批量处理问题。

借鉴Elon Mask的学习方法，我将以Hash Table这个知识点为例，融合自己的学习习惯，梳理一下学习一个知识，从入门，进阶到深入的学习策略。


# 2. 建构：第一印象

对于某个知识的入门，我的策略是：**始于wikipedia, 途径google,止于著作。**

## 2.1 始于wikipedia

在Wikipedia中，寻找知识的 **本质，基石和地图** ，理解不深入没关系，首先保证方向正确。

以Hash Table为例：（学会了哈希表，你就已经掌握了5%的计算机）

1)  **本质**  ：是根据键（Key）而直接访问在内存存储位置的数据结构。也就是说，它通过计算一个关于键值的函数，将所需查询的数据映射到表中一个位置来访问记录，这加快了查找速度。这个映射函数称做散列函数，存放记录的数组称做散列表。

2)  **基石(最少必要知识)** ：1)构造散列函数Hashing 2)处理冲突Collision resolution 3)效率分析: load factor  (对比一下[中文维基][2]和[英文Wiki][3]标题就可以了，取交集即可😄)

3) **地图(定位知识在领域中的位置)** ：Hash Table是一种「数据结构」中array的一种。而数据结构是计算机中存储、组织数据的方式。而正确的数据结构选择可以提高算法的效率。而[算法][4]是计算机处理信息的本质。

![][image-2]

## 2.2 途径google
在Google中，寻找知识的**类比和可视化**，建立**直觉**，我通常google的关键词如下：

1. Google: **hash name origin**

	[Why it is called “hash table”, or “hash function”? Hash doesn’t make any sense to me here][5]
	> The term “hash” comes by way of analogy with its non-technical meaning, to “chop and mix”. Indeed, typical hash functions, like the mod operation, “chop” the input domain into many sub-domains that get “mixed” into the output range to improve the uniformity of the key distribution.

2. Google:  ** hash intuition **
	- 无术语定义：A hash table is a collection of items which are stored in such a way as to make it easy to find them later. 
	- [Another explanation of hash functions][6]

3. Google: hashing simple explanation 
	- [Is there a gentle hash function tutorial? ][7]
	- [What is hashing in simple terms?  ][8]
	- [Hashing - The Greatest Idea In Programming][9] 

4. Google: hash simple example 
	- [Understanding Hash Functions and Keeping Passwords Safe][10]

5. Google: **Hash table visualization**
	- [Open hashing][11]

6. Google images: **[Hash Table gif][12]**

7. Youtube: **Hash Table**
	- [Data Structures: Hash Tables][13]

8. Youtube: **Hash table visualization**
	- [Hash table visualization][14]

## 2.3 止于著作

在找书过程，目前遇到的最好的程序员书单是：http://lucida.me/blog/developer-reading-list/

对于Hash Table而言，我会在Mac中书所在文件夹，进行全文搜索，或者对进行主题锁定，「程序设计\>5.算法与数据结构」和 「程序设计 \> 2. 编程语言」， 在知识的进阶阶段会使用到。


![][image-3]



小结：这个时代，信息在爆炸，但是优质信息并没有，反而可能遭遇沙漠埋没黄金的下场。如何找到优质信息？答案是：**用信任过滤信息，用好书找到好书。前者是找到靠谱推荐源，如某大牛；后者是使用靠谱推荐系统，如Amazon.**



# 3. 解构：模式识别

对知识的进阶阶段，我的策略是：**让好奇心牵引，去主题阅读，批量处理，让模式自然涌现。**

因为在批量著作(books&papers&videos)中，**好书竞争好书，提供好视角。好奇心激起好奇心，提供好动力。**

这里便是Elon Musk学习方法的主要运用，对于Hash Table这个知识点，可以进行三个层面的解构，不同算法与数据结构书的解读，不同编程语言的实现，不同场景的运用(leetcode题目)，从而获得对共同模式的洞见。

## 3.1 第一层：不同作者的解读

### 1) **《Charles: Introduction to Algorithms, 3rd》**

《算法导论》这本书是从「集合」切入Hash Table, 切入的逻辑是，就像现在数学的基础是集合论，集合也是计算机科学的基础。数学的集合是不变的，而算法所操作的集合却是随时间的改变而增大，缩小或者产生其他变化，称为dynamic set。所以问题来了：如何表示和操纵有穷动态集合？

对动态集合的1)元素表示和2)操作的不同需求，我们构造了不同基础数据结构：栈，队列，链表，有树根，散列表，二叉查找树，红黑树。

当我们的算法是对元素表示的要求是「映射关系」，而元素操作的要求只是Insert, Search和Delete，我们构造了Hash Table这样的数据结构。

接着，就介绍在实际运用中的优缺点，以及面对不足——Collision, 两种解决方法：1）Chaining  2)Open Addressing.

最后，当操作需求的没有Delete操作，散列技术还可以获得出色的最坏情况性能。



### 2) **《Robert Sedgewick：Algorithms, 4th》**

《算法》这本书从「查找」切入Hash Table，切入的逻辑，在查找海量数据时，我们往往是像字典一样，先找到单词，然后再读出解释。而如字典般存储信息方式，我们称为符号表，每一条存储key(如单词)和value(如解释)。要在这样的海量信息寻找他们，一个问题自然就出来了：如何高效检索他们呢？

在说明两种实现算法之后，这本书用讲了三种经典数据类型来实现高效的符号表：**Binary Search Trees, Red–black trees, hash tables.**

在hashing tables中，

- 对hash function，对不同数据类型：positive integers, floating-point numbers, strings, compound keys 做了演示；
- 对两种解决Collision的两种Hashing做了图解分析：1) Hashing with separating chaining 2) Hashing with linear probing；
- 数组大小调整(Array resizing)的说明和分析，还有内存使用分析。

	  

### 3) **《Anany: Introduction to the design and analysis of algorithms, 3rd》**

《算法设计与分析基础》这本书是从「时空权衡」角度切入Hashing的，在这个章节介绍了两种技术：

- 一种是对问题的输入进行预处理，存储得到的信息，从而可以加速之后解决问题的速度，称为input enhancement。如字符串匹配的[Boyer-Moore Algorithm][15]。
- 另一种是仅仅是用额外的空间来加速对数据(更灵活)的获取，如Hashing。

对于Hashing则着眼于如何设计这个空间结构。

首先是**What**, 关键词：Hashing, hash table, hash function, hash address。

然后遇到collisons, 如何解决，是为**How**: 
- 1) open hashing, 对应separate chaining 
- 2) close hashing, 对应open addressing。

之后是**Why**, 为什么要学习Hashing, 介绍一些Hashing的一些应用。

一些关键词：linear probing，cluster，double hashing，rehashing，rehashing，bucket。

小结：**兼听则明，偏信则暗。** 通过不同书对Hash Tables不同侧面的解读，可以了解更完整Hash Tables：Hash Tables由集合引出，在查找中得到重要运用，以空间换得快速访问时间。共同重要的东西，正如wikipedia中总结的基石，1）构造Hashing 2）处理Collision 3)效率分析及扩展。

## 3.2 第二层：不同语言的实现

> 除非你掌握了两门以上的语言，否则你永远无法真正理解一门语言。—— 微软全球副总裁Peter Lee

如 Java vs Python 

- hashmap vs dict() 
- hashset vs set()

## 3.3 第三层：不同场景的运用

> 获取反馈是学习和改进的前提。 —— 《精益创业》

通大量的同类题练习，模式自然涌现，虽然有时只可意会，不能言传。
见 Hash Table 练习笔记:  [https://github.com/WillWang-X/AlgorithmsDelight/blob/master/Topic/Hash\_table.ipynb][16]

小结：通过主题阅读，不同作者，不同语言，不同题目，让作者互相讨论，自己作旁观者清。当然，阅读过程并非一定是线形路径，更多是一种有限深度搜索之后，再调整深度继续的搜索。最好的方式是**产生问题，让好奇心牵引前行。**


# 4. 重构：融会贯通

在知识的深入阶段，我的策略是：**发展于思考和讨论，下切到行动指南，回归到总结输出。**

## 4.1 第一层：发展于思考和讨论
> “每个从事复杂工作的人都需要同事，和别人共事的要求是你必须把自己的想法清楚地说出来，光是这个规矩就能让你受益匪浅。” —— 查理·芒格

在解构知识点后，往往是离散孤立的信息，时间长，就像没有根的浮萍，渐渐消失在脑海。而讨论，便是大家一起拼图的过程，找到信息到信息之间的知识道路。因为讨论，带来实时的交互和反馈，以及解惑。如果说模式识别是解构，那么讨论是融会贯通的重构开始。

![][image-4]

## 4.2 第二层：下切到行动指南
> “一个没有自我划界的观点，不是好观点；一个勇敢的作者，是应该多写让步的。” —— 陈虎平

行动指南是交流的成果，是用来总结Hash Table的优缺点，是了解Hash Table适用范围，最终最终形成批量处理此类问题的模式，对知识进行精细编码。
![][image-5]

当然，按照德雷福斯模型，新手，高级新手，胜任者，精通者，专家的路径。最后专家靠的是直觉，是内隐知识。

参考：[大师比新手强在哪里？][17]


Hash Table 用一句话说就是：**回眸一笑百媚生！**

## 4.3 第三层：回归到反思总结

> 不反思总结，为什么奢望成长呢？ —— No one 

![][image-6]

最后，最后可以整理成一篇文章或者笔记，因为[书写是为了更好的思考][18]。

小结：**讨论，连接知识与知识；行动，连接理论和经验；输出，连接自己和世界。**


# 5. 小结：三重境界

宋代禅宗大师青原行思提出参禅的三重境界：参禅之初，看山是山，看水是水；禅有悟时，看山不是山，看水不是水；禅中彻悟，看山仍然山，看水仍然是水。

同理，知识深入过程，也是三个阶段：**理解入门，看山是山，第一印象，是为建构；理解进阶，看山不是山，模式识别，是为解构；理解深入，看山还是山，融会贯通，是为重构。**

[1]:	https://medium.com/@michaeldsimmons/how-elon-musk-learns-faster-and-better-than-everyone-else-a010a4f586ef
[2]:	https://www.wikiwand.com/en/Hash_table#/Dynamic_resizing
[3]:	https://www.wikiwand.com/zh-hans/%E5%93%88%E5%B8%8C%E8%A1%A8#/.E4.BE.8B.E7.A8.8B
[4]:	https://www.wikiwand.com/en/ACM_Computing_Classification_System
[5]:	https://softwareengineering.stackexchange.com/questions/108124/why-it-is-called-hash-table-or-hash-function-hash-doesnt-make-any-sense-t
[6]:	http://blog.tyrannyofthemouse.com/2011/11/another-explanation-of-hash-functions.html
[7]:	https://stackoverflow.com/questions/3804403/is-there-a-gentle-hash-function-tutorial
[8]:	https://www.quora.com/What-is-hashing-in-simple-terms%0A
[9]:	http://www.i-programmer.info/babbages-bag/479-hashing.html
[10]:	https://code.tutsplus.com/tutorials/understanding-hash-functions-and-keeping-passwords-safe--net-17577
[11]:	https://www.cs.usfca.edu/~galles/visualization/OpenHash.html%0A
[12]:	https://2.bp.blogspot.com/-wvatIrYTbNg/UR0H5EltPEI/AAAAAAAARg8/2a9AE9leiKU/s1600/cuckoo_animated.gif
[13]:	https://www.youtube.com/watch?v=shs0KM3wKv8
[14]:	https://www.youtube.com/watch?v=FBP3JVnPBuM
[15]:	http://whocouldthat.be/visualizing-string-matching/
[16]:	https://github.com/WillWang-X/AlgorithmsDelight/blob/master/Topic/Hash_table.ipynb
[17]:	https://mp.weixin.qq.com/s?__biz=MzA4ODM4ODQ3MQ==&mid=2651930954&idx=1&sn=e6adbf0de88acb6830ae48e123ce87e8&chksm=8bcf0752bcb88e44607c53541b3e95e1b9862b51c2955e1b332faef63f994d1be69b17b249af&mpshare=1&scene=1&srcid=0209jeNt5sJ3cMRFJYKENHBR#rd
[18]:	http://mindhacks.cn/2009/02/09/writing-is-better-thinking/

[image-1]:	https://cdn-images-1.medium.com/max/1600/0*tG-pbbXuaTea4iwO. "two A"
[image-2]:	https://github.com/WillWang-X/WillWang-X.github.io/blob/master/_picture/datastructure.png?raw=true
[image-3]:	https://github.com/WillWang-X/WillWang-X.github.io/blob/master/_picture/book.png?raw=true "books"
[image-4]:	https://i.imgur.com/HQJURQD.png "information - knowledge "
[image-5]:	https://github.com/WillWang-X/WillWang-X.github.io/blob/master/_picture/prosandcons.png?raw=true
[image-6]:	https://i.imgur.com/1TfuRYe.png "方法论"