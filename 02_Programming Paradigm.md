# 编程范式
## 什么是编程范式

<p align=right>
三观不正，一事无成！
        —— 某领导
</p>

我们常说，C++的一个特点是“支持多种编程范式”，那么到底什么是编程范式呢？不知道大家在开始写代码前，有没有问过自己这样三个问题：

1. 要解决的这个问题有什么特点和内在逻辑？
2. 编程所用的语言提供了哪些语法支持和功能模块？
3. 写代码时，如何使上面两者很好地匹配，从而得到一个优美而高效的解决方案？

这三个问题的答案，基本上就决定了整个代码的编程风格和基调，而这个“编程风格和基调”，就是*编程范式*。可以这么说：编程范式就是编程时的“三观”。

在维基百科上，对*编程范式*的解释是这样的（http://zh.wikipedia.org/wiki/编程范型 ）：
```
编程范型或编程范式（英语：Programming paradigm），（范即模范之意，范式即模式、方法），是一类典型的编程风格，是指从事软件工程的一类典型的风格。
……
编程范型提供了（同时决定了）程序员对程序执行的看法。
```
大家可以琢（gan）磨（shou）一下是不是这么一回事儿。


## 常见的编程范式

<p align=right>
（孔乙己）点头说，“对呀对呀！……回字有四样写法，你知道么？”
                                    ——《孔乙己》

</p>

编程范式有很多种分类方法，比如结构化编程和非结构化编程、命令式编程和声明式编程、面向过程编程和面向对象编程等。每种分类方法的依据和着眼点都不相同，在这里，我们只能对几种比较常见的编程范式做一个简单介绍：
- 面向过程编程
    将待解决的问题归结为“按某种顺序，对某些数据进行某种处理”。对数据进行处理就是一个“过程”。通过把不同的过程按某种方式组合起来，并在过程之间传递数据，最终得到想要的结果（还记得怎样把一头大象塞进冰箱吗？）。比如图像处理、数值计算等这类问题，比较适合面向过程编程。
    
- 面向对象编程
    将待解决的问题归结为“若干个实体之间的交互”。各个实体之间可以是平级关系（比如同学之间），也可以有一定的层级关系（比如老师和学生）或者包含关系（比如班级与学生）。通过在实体之间传递信息，得到最终结果。面向对象编程比较典型的应用场景是：图形界面（GUI）、多媒体系统。
    
- 函数式编程
    将待解决的问题归结为“对一系列函数进行组合并求值”。这里说的“函数”很像数学中的函数，可以将其视为一个“*把特定输入映射成特定输出*”的黑盒子。而且这个黑盒子很靠谱，不管什么时候，在什么情况下，都能确保同一个输入得到的输出结果一定是相同的。这一点使得函数式编程适合构建很复杂的分布式，多并发系统。
    
- 泛型编程
    泛型编程跟前面三种编程范式略有不同，它主要针对的不是如何对问题建模，而是*如何利用编程语言的类型系统来生成代码，或者动态添加某个功能*。它主要用于元编程（可以生成程序的程序）。

由于C++可以很好地支持面向过程、面向对象和泛型编程，并对函数式编程也有一定的支持，所以说C++是一种“多范式编程语言”。
