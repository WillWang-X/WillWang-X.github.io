--- 
layout: post
title:  操作与被操作
tags:
- 思路的诞生
status: publish
type: post
published: true
---

<br>

> 如何能够将200ml的水装进100ml的杯子里？
	
### 1. 问题是这样子的：
	
Given a rows x cols screen and a sentence represented by a list of non-empty words, find how many times the given sentence can be fitted on the screen.
	
**Note:**	
- A word cannot be split into two lines.
- The order of words in the sentence must remain unchanged.
- Two consecutive words in a line must be separated by a single space.
- Total words in the sentence won't exceed 100.
- Length of each word is greater than 0 and won't exceed 10.
- 1 ≤ rows, cols ≤ 20,000.
	
**Example 1:**	
```
Input:
rows = 5, cols = 4, sentence = ["ab", "cde", "f"]
Output:
2
Explanation:
ab--
cde-
f-ab
cde-
f-ab
The character '-' signifies an empty space on the screen.
```
	
—— [418. Sentence Screen Fitting](https://leetcode.com/problems/sentence-screen-fitting/description/)
	
### 2. 一个理想的思路：
	
1) 问题简而言之，就是把「单词」往「表格」里塞，看最终能组成多少句子。
	
2) 分析一下，这里有两个操作对象：「单词」和「表格」。 如果在现实世界，我们的想法就是把「句子」拆成「单词」往「表格」里塞。那看看这个例子呢：
	
```
rows = 20000, cols = 20000, sentence = ["a", "b", "c"]
```
  
  在现实世界里，假设你站在在某一行的开头，你会看到一个满头大汗在不停塞"a_b_c_"，面对着望不到的尽头。(这意味这时间复杂度很高 = O(rows*cols) )
	
3) **那为什么不能反过来呢？**把「表格」拆成一个个「木条」往无尽长的「句子」中塞呢。现实世界的经验束缚了我们的想象。就像开始的问题，现实世界让我们默认是水是液态的一样。在电脑世界，犹如「盗梦空间」中一样，我们可以许多打破许多默认的假设。如下面所示：
	
![无穷的数列](https://i.imgur.com/vCcBId2.png)
	
### 3. Show me the code 
	
<script src="https://gist.github.com/WillWang-X/0b9979b846dac6f6bbae4ddce1881c16.js"></script>
	
### 4.想多玩一会
	
1. 这道题做法有没有可以改进的地方？提示：KMP(预处理), [时空权衡之预处理](https://willwang-x.github.io/2018/03/preprocessing), [Discussion的优雅解法](https://leetcode.com/problems/sentence-screen-fitting/discuss/90845/21ms-18-lines-Java-solution/95290)
2. 想一想[55. Jump Game](https://leetcode.com/problems/jump-game/description/) 有没有其他思路？可参考[DP solution](https://leetcode.com/problems/sentence-screen-fitting/discuss/90874/12ms-Java-solution-using-DP)
2. [322. Coin Change](https://leetcode.com/problems/coin-change/description/) : 改变循环中不同的操作先后顺序看看有什么不一样的惊喜？
	
### 5. 感谢
	
Credit to Huahua
	
	

<br>
<br>

简之           
2018.03.31          

