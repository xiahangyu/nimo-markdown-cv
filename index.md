---
layout: cv
title: hangyux
pdf: true
---
# 夏航宇

<div id="webaddress">
<i class="fi-mail" style="margin-left:1em"></i>
<a href="348106768@qq.com" style="margin-left:0.5em">348106768@qq.com</a>
<i class="fi-telephone" style="margin-left:1em"></i>
  <a href="348106768@qq.com" style="margin-left:0.5em">+86-13797506543</a>
</div>

## **教育背景**
### **墨尔本大学** `2017.2 - 2019.1 @墨尔本，澳大利亚`
- 计算机科学 理学硕士学位
  
### **华中农业大学(211)** `2012.9 - 2016.6 @武汉，中国`
- 计算机科学与技术 工学学士学位

## **专业技能**

### **编程语言**
- C++, Python, PDDL, Strips, Java, Haskell
  
### **技术**
- UE4: 
    - 基本渲染管线，PBR
    - UMG, Slate
    - 材质系统基础
	- 些许Game play相关知识
    
- AI Planning:
    - Search: blind/heuristic, MDP, MCTS/UCT, Iterated Width, AlphaGo Zero
    - Reinforcement Learning: Q-learning, Sarsa, Deep-Q-Learning  
  
- Machine Learning: 
    - Basic: Regression, Bayesian Regression, SVM, Kernel, GMM/EM, PCA, MDS
    - NLP: VSM, Tagging(HMM, VITERBI), CFG(CYK/PCYK), IE(NER, RE), Machine Translation(IBM model1 & EM)
    - Web Search: IR(Querying, Querying Completion/Expansion)
 
- 手机设备自动化相关:
    - UiAutomator (Android)
    - Minicap, Minitouch/Multitouch (Android)
    - Adb (Android)
    - Wda (IOS) 

- 后台相关: 了解有限
    - RESTful, RPC, GPRC
    - Django
    - Redis

## **工作经历**
### **深圳前海创梦天地** `2020.4 - 至今`
- UE4客户端开发

### **腾讯计算机系统有限公司** `2019.4 - 2020.4`
- 测试开发

## **项目经历**
### **一款TPS游戏** [C++] `2019.4 - 至今`
  - 主要负责部分UI界面的开发：好友，房间，聊天，局内枪械数据面板等
  - 游戏启动器：游戏pak打包。启动器为program类型的独立程序，负责更新pak和代码，并启动游戏。
  
### **Smart tool** [Python] `2019.11 - 2020.4`
  - 一个PC端手机自动化脚本录制工具。客户端使用WxPython开发，通过在工具中操作手机自动生成对应流程的脚本流程文件(一些json文件定义的状态转换图)。
  - 因为有AIClient手机驱动的经历，这个项目中主要工作集中在客户端开发。多个Panel之间的消息通信（使用了一个类似publisher-subscriber的多线程机制），以及复杂的状态转换生成。

### **维护山竹客户端** [Python] `2019.9 - 2020.4`
  - 一个分布式自动化测试平台的执行工具。由Agent和runner构成。
  - Agent管理当前电脑上连接的测试手机，实时从服务器拉取测试任务，启动任务，等待结束后上传任务结果。
  - Runner执行测试脚本，操控手机，收集执行信息，上传本次测试结果。

### **AIClient** [Python] `2019.7 - 2020.4`
  - 一个与远程手游AI服务器通信的手机客户端。负责从手机截取图片发送至AI服务器，获取对应动作消息后在手机执行对应动作。客户端与服务端共同合作实现包括启动游戏，登陆账号，进入对局，自动游戏的效果。
  - 手机驱动：Adb安装启动游戏，UiAutomator手机截图/执行动作，MultiTouch多点触控。
  - 网络通信：RESTful API与AI模型管理服务器申请AI服务 (HTTP)，ZeroMQ(TCP)与AI服务进行同步/异步通信。

### **Watcher** [Python] `2019.4 - 2019.7`
  - 一个RESTful web服务监控系统。定时监控一些服务器接口返回数据的有效性，结果通过邮件通知和网页显示。监控云服务器共享磁盘各路径大小（可配置路径，可highlight和ignore指定路径），空间过低时邮件警报。
  - Docker服务器，Redis数据存储，Nginx+wsgi负载均衡

### **基于游戏图像数据的 Atari 游戏通用性 AI (研究生毕业论文)** [[C++, Python源码](https://github.com/xiahangyu/ALE-Atari-Width)] `2017.8 - 2018.11`
  - 基于 M.G Bellemre et. al. 开发的 **Atari Learning Environment (ALE)** 设计可以被用于不同类型 Atari 游戏的 AI
  - 核心方法 **Iterated Width Search** + **B-PROS Method**。
  - 此外还尝试使用了 **CNN** 和 **LSTM** 的 **AutoEncoder** 来对游戏图像进行特征提取。
  - 该 AI 可以在没有硬编码任何游戏策略的情况下取得比一般人类玩家更高的游戏分数[[游戏视频](https://www.youtube.com/channel/UC9QnDPExehDjGwc428EXnyg/playlists)]

### **阅读理解式 Question & Answering 模型** [[Python源码](https://github.com/xiahangyu/Question-Answering)] `2018.4 - 2018.5`
  - 对单词作**Embedding**
  - **BM25/TF-IDF** 定位问题相关段落和句子
  - **seq2seq** 的 **GRU/LSTM** 模型来做(答案段落/答案句子, 问题)->(答案)的预测

### **基于Spark的笛卡尔遗传程序算法分布式化研究 (本科毕业设计)** [[Scala源码](https://github.com/xiahangyu/Spark-CGP)] `2015.11 - 2016.6`
  - 设计11位多路选择器的逻辑电路. 
  - 基于**Spark/GraphX**图计算框架，并行化解决串行笛卡尔遗传程序无法处理规模极大、迭代层次极深的问题
  - 5台worker，1台master。通过大量的分布式计算最终在30分内成功找到一组解(串行C程序花费3.5个小时无法求解)

### **Ext2 文件仿真系统** [[C++源码]](https://github.com/xiahangyu/Ext2-simulation) `2015.6 - 2015.7`
  - 在 windows 系统下面模拟 Ext2 文件系统的磁盘初始化，文件/文件目录操作
  - 相关数据结构: 组块描述表，位图，内外存 i 节点，进程文件打开表，系统文件打开表
  - 相关算法: 路径解析，逻辑物理地址映射，空闲块分配，块回收

## **校园经历**
在校期间多次参与千人规模的校园乐队演出，担任鼓手一职。

<!-- ### Footer

Last updated: Nov 2018 -->
