--- 
layout: post
title:  思路的诞生之正反思维：始末
tags:
- 思路的诞生
status: publish
type: post
published: true
---
	
	
<br>

> 凡事反过来想一想。 —— 不知名的观众	


### 1. 问题是这样的：

A move consists of taking a point (x, y) and transforming it to either (x, x+y) or (x+y, y).
Given a starting point (sx, sy) and a target point (tx, ty), return True if and 
only if a sequence of moves exists to transform the point (sx, sy) to (tx, ty). 
Otherwise, return False.

### 2. 一个理想的思路过程是：
	
1. 看到题目确定是一个**搜索**问题。
2. 然后搜索问题的解法，想到有三种： **DFS，BFS，双端BFS**。
3. 尝试完好写的BFS：超时！尝试完更好写的DFS: 超时！无计可施？🙄
4. 双端BFS？... 念口诀：**正的不行，反的行。**
	

<br>

<center> <b> Aha! 什么是树呢？ </b> </center>

<center> <b>众人疑惑脸。🤔 </b>	</center>

<center> 树的性质：<b> 每一个非根节点有且只有一个父节点啊</b>  </center>


	


	
来，看图:
	
![Reaching Points](https://i.imgur.com/FsKaX4b.png)
	
	
		

所以我们可以通过**“用大数减小数”**来达到父亲节点！ 
	
快要到达了终点了... 但还是超时了！ 
体会一下这个 ***Edge case: (1, 1) ->（1，10^9)***

那如何优化呢？ 

**Aha！[GCD:Euclidean algorithm!](https://upload.wikimedia.org/wikipedia/commons/e/e2/Euclidean_algorithm_252_105_animation_flipped.gif)** ✌️	 

### 3. Show me the code
	
<script src="https://gist.github.com/WillWang-X/807067fb94a4f0ee03a5dd391b305d4b.js"></script>


### 4. 想多玩一些？

- [782. Transform to Chessboard
](https://leetcode.com/problems/transform-to-chessboard/description/) : 如何从结局推开始，让复杂问题变成一个简单问题？



<br>
<br>

简之           
2018.02.11
