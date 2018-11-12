---
layout: cv
title: hangyux
pdf: true
---
# 夏航宇

<div id="webaddress">
<i class="fi-mail" style="margin-left:1em"></i>
<a href="xiahangyu@gmail.com" style="margin-left:0.5em">xiahangyu@gmail.com</a>
<i class="fi-telephone" style="margin-left:1em"></i>
  <a href="xiahangyu@gmail.com" style="margin-left:0.5em">+86-13540677782</a>
</div>

## 教育背景
### 墨尔本大学 `2017.2 - 2019.1 @墨尔本，澳大利亚`
- 计算机科学 理学硕士学位
  
### 华中农业大学(211) `2012.9 - 2016.6 @武汉，中国`
- 计算机科学与技术 工学学士学位

## 专业技能

### 编程语言
- C++, Python, PDDL, Strips, Java, Haskell
  
### 技术
- 智能规划:
    - 搜索: blind/heuristic, MDP, MCTS/UCT, Iterated Width, AlphaGo Zero
    - 强化学习: Q-learning, Sarsa, Deep-Q-Learning  
  
- 机器学习: 
    - 基础: 回归, 贝叶斯回归, SVM, Kernel, GMM/EM, PCA, MDS
    - NLP: VSM, Tagging(HMM, VITERBI), 语法分析(CYK/PCYK), 信息提取(NER, RE), 机器翻译(IBM model1 & EM)
    - 网页搜索: 信息检索(Querying, Querying Completion/Expansion)

## 项目经历
### **基于游戏图像数据的 Atari 游戏通用性 AI (研究生毕业论文)** [[C++, Python源码](https://github.com/xiahangyu/ALE-Atari-Width)] `2017.8 - 2018.11`
  - 基于 M.G Bellemre et. al. 开发的 **Atari Learning Environment (ALE)** 设计可以被用于不同类型 Atari 游戏的 AI (domain-independent)
  - **Iterated Width** 搜索+**B-PROS** 特征。此外还尝试使用了 **CNN** 和 **LSTM** 的 **AutoEncoder** 来对游戏图像进行特征提取。但效果不佳。主要原因是 GPU 性能不够，无法提供更复杂的计算
  - 该 AI 可以在没有硬编码任何游戏策略的情况下取得比一般人类玩家更高的游戏分数[[游戏视频](https://www.youtube.com/channel/UC9QnDPExehDjGwc428EXnyg/playlists)]

### **阅读理解式 Question & Answering 模型** [[Python源码](https://github.com/xiahangyu/Question-Answering)] `2018.4 - 2018.5`
  - 对单词作**embedding**。使用 **BM25/TF-IDF** 定位问题相关段落和句子，然后用 **seq2seq** 的 **GRU/LSTM** 模型来做(答案段落/答案句子, 问题)->(答案)的预测

### **基于Spark的笛卡尔遗传程序算法分布式化研究 (本科毕业设计)** [[Scala源码](https://github.com/xiahangyu/Spark-CGP)] `2015.11 - 2016.6`
  - 设计11位多路选择器的逻辑电路. 
  - 基于Spark/GraphX图计算框架提出了一种笛卡尔遗传规划程序的并行化方法来解决串行笛卡尔遗传程序无法处理问题规模极大、迭代层次极深的缺点
  - 5台worker，1台master。通过大量的分布式计算最终在30分内成功找到一组解 (串行C程序花费了3.5个小时都无法求解)。

### **Ext2 文件仿真系统** [[C++源码]](https://github.com/xiahangyu/Ext2-simulation) `2015.6 - 2015.7`
  - 在 windows 系统下面模拟 Ext2 文件系统的磁盘初始化，文件目录操作
  - 在逻辑上实现系统组块描述表，位图，内外存 i 节点，进程文件打开表，系统文件打开表，路径解析，逻辑物理地址映射，空闲块分配，块回收

<!-- ### Footer

Last updated: Nov 2018 -->
