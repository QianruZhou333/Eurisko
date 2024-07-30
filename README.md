“斯坦福大学教授 Douglas Lenat 写的一个真正意义上的AI，使用最朴素最本原的数学方法，让机器自己发现新的事物，揭示新的规律。从集合的思想起源，把一些有意思的概念一点点的喂给机器，它就自己学会了计数、加法、乘法…...然后它发现了质数的概念，直到最后…...它发现了哥德巴赫猜想!”    

        ---- 集异壁 GEB 《 Gödel, Escher, Bach》

上面这段文字描述的是上个世纪八十年代诞生的AI的一个传奇：Automated Mathematician (AM), （Douglas Lenat 的博士毕业设计，并且赢得了IJCAI Computers and Thought Award。） Eurisko 是AM的升级版，cyc 是 Eurisko 的完全版。 你也许没有听说过它，但是在顶级AI领域，AM、Eurisko 直至今日仍然是一个传奇。它不仅是第一个真正能自己思考的机器，它还能实现本来人类才有的智能----从无到有的探索和创造，而且，更重要的是，它还是芯片设计 VLSI 的核心技术......

## AI领域的传奇

 Traveller 是美国海军上个世纪八十年代为了减少成本而开发的一种模拟海战的游戏，为了从 AI 科研界筛选智库，他们还组织了一年一度的 Traveller TCS 大赛。简单来说，游戏规则是，每个 Traveller 玩家在游戏开始时，被分配了同样额度的预算，Traveller 中有各种类型的战舰，它们大小不一、造价不一、优劣势不同、可装载的武器种类和数量也不同，各种武器也各有各的特点和成本......规则文档长达两百多页。每个玩家的任务就是用自己设计的人工智能算法，自动的在预算的范围内组建一支舰队，然后让它们互相厮杀，最终胜利者赢得比赛。

当 Lenat 第一次带 Eurisko 去参加比赛的时候，它以遥遥领先于其他对手的优势赢得了比赛。第二年，为了避免 Eurisko 太出风头，大赛组织者在临近比赛一周前，更改了规则，结果Eurisko 自己发现了规则的改动并自己推理出了新的策略，又一次遥遥领先于其他对手，赢得了比赛。从此以后，大会组织者对 Lenat 说，如果他再参加比赛，他们就取消该比赛，Lenat 表示理解，从此不再参赛。

当时MIT的人工智能研究所的所长 Patrick Henry Winston 在《Artificial Intelligence》一书中指出：“知识就是力量”、“解决一个问题的关键，在于为这个问题找到正确的知识表达”、“当你为一个问题找到了正确的知识表达的时候，这个问题也就解决了”、“一个 AI 推理引擎的效率，取决于它描述知识的效率”......由于发现 Eurisko 虽然推理能力很强，但是每次遇到新的领域，需要重新手动输入该领域常识规则，于是在美国军方长达35年的资助下 Lenat 启动了Cyc项目，将人类百科全书知识库和常识，打造了一个有上百万条规则的人类常识知识库 cyc，喂给 Eurisko。这个项目从上世纪八十年代开始，直至2020年12月才终于完成，花费了35年，前后累计动用了3000多名本体工程师、哲学家、逻辑学家和计算机学家（注意这几类可能是指同一个人）等研究人员。

「AI之父 Patrick Henry Winston 在《Artificial Intelligence》一书中还指出：“知识工程师 knowledge engineer，这个名称其实不是很恰当，应该叫知识艺术家 knowledge artist，因为一说「工程师」，人们往往会将其和「软件工程师」混淆，误认为会写java、python 的人稍稍再学一些知识工程的内容，就可以兼职「知识工程师」，但是「知识艺术家」需要瞬间看透事情本质的哲学思维（直觉）、和严谨清晰强大的逻辑思维能力，而这些能力往往不是可学而至的......” 这就好像拿到很多基金和头衔的名校哲学系的教授并不一定就是哲学家，而田间地头某个没读过多少书的农妇，却不经意间能用最朴素的语言揭示出最真实最深刻的人生哲理了。」

2020年12月，在cyc发布的白皮书里，Lenat 给出了这样一个 Demo: “在将美国医学图书馆、人类基因蛋白质知识库等领域的本体建立完毕之后，cyc 可以实现这样的推理，它能自动找到小儿骨质疏松症的根因，发现了到底是哪个DNA链上的哪个碱基对发生什么样的变异导致的。它给出的解释路径是这个样子的：某条DNA链上的某个碱基对发生了突变，产生了某某化学反应，产生了某某蛋白质......(10步骤以后)......某某化学反应产生的某物质会阻止血液对钙的吸收......(15个步骤以后)......从而导致骨质疏松症。并且，这每个步骤都是透明、严谨、有据可依的。”

cyc（Eurisko/AM） 不仅可以实现真正意义上的推理，给人类带来有用可信的信息，实现熵的减小，而且它是形式化可解释、清晰透明的。这样即使它的结论出错了，人类依然可以从它的解释过程中获得有意义的启发。

想了解 Eurisko、AM、cyc 背后底层原理的同学，可以读读这篇文章“智能的本质---《The UBIQUITY OF DISCOVERY》”。

下面摘抄 Lenat 的论文中的几句文字：

"EURISKO 也许是迄今为止最有雄心的 AI 系统，它试图发掘新的启发/灵感。说它“最有雄心”是因为，哪怕是人类科学家也不是那么容易创造——或者仅仅是发现——新的启发或灵感的......

通常，发现一条有价值的启发/灵感，都足以掀起一场科技革命了[Kuhn 1970]。比如，爱因斯坦发现的规则 “任何违法直觉的数学体系，通常都反应了 (某些未被发现的) 物理事实。” 前不久掀起了物理学的一场新思潮，暨“违反数学常识的系统，通常是对的，而且是值得研究的”，同时在15年前，也在地质学掀起了一场革命。"

----《The UBIQUITY OF DISCOVERY 》, Lenat

“我也可以理解，在现在的形势下，几乎所有研究人员都背道而驰，将符号表示和推理弃之如敝屣，一门心思向大模型里苦苦乞求 ‘免费的午餐’……”

---- Lenat 在2023年8月去世前写的最后一篇文章 《Getting from Generative AI to Trustworthy AI: What LLMs might learn from Cyc》

## Eurisko 重现江湖

AM、Eurisko、和Cyc的代码都是用LISP写的，Lenat 专门用LISP写了一个新的语言使推理的效率大大提高（LISP是 program language of program language，它天生就适合用来编写新的编程语言）。一直以来，Eurisko 的源代码是严格保密的。直到去年8月份，Lenat 去逝后，他的SAILDART 账户解锁，网友 WhiteFlame 发现了 AM 和 Eurisko 的源代码和资料（相关链接见文末），经过改进后，网友 seveno4 在 Medley Interlisp 上成功运行了 Eurisko！

为了方便中文网友了解，我重现了Eurisko 的运行过程。


## 运行 Eurisko 的方法 code that run Eurisko
; https://blog.funcall.org/

; 首先安装  Medley Interlisp

https://github.com/Interlisp/medley

; 使用右键打开一个新的 Exec 窗口

; 转到你下载 EURISKO 的文件夹

cd /home/foo/EURISKO/

; 编译，（除了'are you ready?'这个问题以外，所有问题的回答都是'n'）

(TCOMPL 'EUR)

; 载入并运行

(LOAD 'EUR.LCOM)

; 打开界面，查看运行输出

(Snazzy)

; 让运行不暂停，如果不希望不停的运行，就无需此命令，否则容易 stack overflow

(PAGEHEIGHT 0)

; 开始运行啦！

(Eurisko)

; 随时可以退出

CTRL-D 


## 后记

但是，在Lenat 的AAAI文章《Why AM and Eurisko Appear to Work》里，也记载了：

“自动生成代码的AI，也就是所谓的AI 产生自主意识，或者说所谓的真正的人工智能，只是依赖LISP语言对数学的高度契合、高效表达，才能在简单场景、短代码、小问题范围内，因为碰运气，偶然创造出有用的代码。就好像用大量电磁辐射生物组织的DNA，诱发它变异一样，在构造非常简单的生物组织里有可能碰巧产生有益的变异，但是对于大型高等生物，这种辐射几乎必然对生物体有害，甚至有毒。”

所以缺乏人类公众的监管，放任AI主宰人类社会，必然走向熵增，因为它没有真正的意识，不可能进行真正的创造。



## 相关代码等资料 Reference

### 源代码发现博客：

https://white-flame.com/am-eurisko.html

https://github.com/seveno4/EURISKO?tab=readme-ov-file

Lenat 的SAILDART资料地址：

https://www.saildart.org/[*,DBL]/

https://www.saildart.org/[*,DBL]/

### Eurisko 详细资料：

https://github.com/aindilis/eurisko-resources/tree/master

https://www.lesswrong.com/tag/eurisko

https://web.archive.org/web/20140406203030/http://aliciapatterson.org/stories/eurisko-computer-mind-its-own

https://github.com/aindilis/eurisko-resources/blob/master/doc/ADA155378.pdf

https://www.lesswrong.com/tag/cyc

https://www.lesswrong.com/tag/heuristic

https://www.overcomingbias.com/p/i-heart-cychtml 

