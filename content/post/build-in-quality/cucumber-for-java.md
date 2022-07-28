---
title: "Cucumber for Java"
date: 2022-07-21T23:48:49+08:00
url: /build-in-quality/cucumber-for-java/
categories:

- Build-in Quality

summary: The Helper of Cucumber for Java
---

# 为什么写这篇 Helper
The Cucumber For Java Book - Behavior-Driven Development for Testers and Developers  
*Written by Sea Rose, Matt Wynne, and Aslak Hellesoy*  
*Source Code：https://pragprog.com/titles/srjcuc/the-cucumber-for-java-book/*  
    
    
    
《The Cucumber For Java Book》这本书对于刚入门的新手来说过于不友好，
一个是 Java 世界的人不习惯用命令行来操作，大多数人是用 IDE 来写 Java，
另一个是多数时候 Cucumber 多数时候是结合 Sprint boot 等框架一起编写，很少这样Core Java直接编写，书上的编写习惯给人感觉好像来自Ruby 世界，但是 Ruby 世界的命令千锤百炼，哪里像Java命令行那么丑，
对于有些想学习 BDD 的管理型教练来说还是有点晦涩，故此有了这篇 Helper 文章。
    
    

# The Helper of Cucumber for Java Book

## Environment and Command Line


这本书是需要安装 JDK 并设置对应的环境变量的，否则没法在 terminal 里面直接运行 Java 命令，可自行 Google JDK installation。

书中的例子只需要在 terminal下 cd 到对应的例子目录就可以直接运行，命令如下：

```bash
#first_taste/02/cucumber
$ java -cp "jars/*" cucumber.api.cli.Main -p pretty features
$ ./cucumber
```

java -cp 即 -classpath , 指定 classpath 目录后，jvm 就会去对应目录寻找 Java 类。

cucumber.api.cli.Main 就是我们要执行的程序的入口

-p pretty 就是告诉cucumber 使用 pretty format 来显示输出结果

```bash
#作为对比可以去掉参数运行试试
❯ java -cp "jars/*" cucumber.api.cli.Main features
```

features 是指到当前目录下的 features 目录去寻找 .feature 文件

```bash
#作为对比可以去掉features试试
❯ java -cp "jars/*" cucumber.api.cli.Main
```

​     

​      



## Regular Expression

正则表达式，做完就忘，触之google。

```java
@Given("^the price of a \"(.*?)\" is (\\d+)c$")
public void thePriceOfAIsC(String name, int price) throws Throwable {
  int bananaPrice = price;
}
```

`$` 匹配输入字符串的结尾位置

`^`  匹配输入字符串的开始位置

`\`  将下一个字符标记为原义字符, `\"` 匹配 `"`, `\\` 匹配 `\`

`+` 加号代表前面的字符必须至少出现一次（1次或多次）

`\d` 是匹配一个数字(0到9)

 `\d+` 表示一个或者多个数字

`"\\d+"` 是在程序字符串 `""` 中，先转意`\\`为`\`, 然后组合出`\d+`

`.`  匹配除换行符 \n 之外的任何单字符

`"(.*?)"` 则是得到包含几个元素的列表，每个元素直接对应原来文本中不同的位置匹配的项

​    

_To be Continued ..._这个人很懒，有缘再续写

