---
title: 第一期:(1)hexo常用命令及markdown基础语法
date: 2019-06-24 11:23:43
<<<<<<< HEAD
cover: /img/1.jpg
=======
categories: 
    - Hexo
>>>>>>> 621d0618623c158a0985d8d2b17236b65fad70db
tags:
    - md语法
    - 6月
---
### hexo常用命令

#### 1、分段:两个回车:
```
        一个人会落泪，是因为痛；一个人之所以痛，是因为在乎；一个人之所以在乎，是因为有感觉；
     
        一个人之所以有感觉，仅因为你是一个人！所以，你有感觉，在乎，痛过，落泪了，说明你是完整的一个人。
    难过的时候，原谅自己，你只不过是一个人而已，没必要把自己看的这么坚不可摧。
```

#### 2、换行 两个空格 + 回车 :
```
            一个人之所以有感觉，仅因为你是一个人！所以，你有感觉，在乎，痛过，落泪了，说明你是完整的一个人。  
        难过的时候，原谅自己，你只不过是一个人而已，没必要把自己看的这么坚不可摧。
```
#### 3、标题 # ~ ###### 井号的个数表示几级标题，即Markdown可以表示一级标题到六级标题:

## H2: 一个人之所以有感觉，仅因为你是一个人！
### H3: 一个人之所以有感觉，仅因为你是一个人！
#### H4: 一个人之所以有感觉，仅因为你是一个人！
##### H5: 一个人之所以有感觉，仅因为你是一个人！
###### H6: 一个人之所以有感觉，仅因为你是一个人！

#### 4、引用 >:

> 一个人之所以有感觉，仅因为你是一个人！

#### 5、列表 * ， + ， - ， 1. ，选其中之一，注意后面有个空格:

* The reason why a person feels is because you are a person!
+ The reason why a person feels is because you are a person!
- The reason why a person feels is because you are a person!

1. The reason why a person feels is because you are a person!
2. The reason why a person feels is because you are a person!
3. The reason why a person feels is because you are a person!
    
#### 6、代码区块 四个空格 开头:
```
    The reason why a person feels is because you are a person!
```
#### 7、链接:
`
    [文字](链接地址)
`

#### 8、图片:
`
    ![](图片地址) //图片地址可以是本地路劲，也可以是网络地址
`
#### 9、强调:

**字体删除** 
__字体删除__ 
_字体删除_ 
*字体删除*
~~字体删除~~

#### 10、代码:

```
    The reason why a person feels is because you are a person! 
```
#### 11、字体及颜色用法:

> <font color=red face="黑体">我是黑体字</font>
> <font face="黑体">我是黑体字</font>
> <font face="微软雅黑">我是微软雅黑</font>
> <font face="STCAIYUN">我是华文彩云</font>
> <font color=black size=4 face="黑体">黑体</font>
> <font color=#00ffff size=3>null</font>
> <font color=gray size=5>gray</font>

#### 12、代码段:

`
The reason why a person feels is because you are a person! 
`

#### 13、JavaScript 示例:

```
/**
* nth element in the fibonacci series.
*/

function fib(n) {
    var a = 1, b = 1;
    return a;
}
document.write(fib(10));
```

#### 14、表格
 
| 项目        | 价格    |  数量   |
| --------    | -----: | :----:  |
| 计算机      | \$1600  |   5    |
| 手机        |   \$12  |   12   |
| 管线        |    \$1  |   234  |



