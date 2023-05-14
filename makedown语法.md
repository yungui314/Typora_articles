# 1、标题

## 类 Setext 形式:

```
This is an H1
=======

This is an H2
----------
```

效果

This is an H1
=======

This is an H2
----------



## 类Atx 形式

```
# this is H1
## this is H2
###### this is H6
```

效果：

# this is H1
## this is H2
###### this is H6



# 2、字体

```
**这是加粗**
__这也是加粗__
*这是倾斜*
_这也是倾斜_
***这是加粗倾斜***
~~这是加删除线~~
```

效果：

**这是加粗**

__这也是加粗__

*这是倾斜*

_这也是倾斜_

***这是加粗倾斜***

~~这是加删除线~~



# 3、分割线

```
***
**********
- - -
_________________
```

效果：

***

*********

------

-----------------



# 4、引用

```
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.
```

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

### 也可以只在整个段落的第一行最前面加>

```
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.
```

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

### 也可以嵌套引用

```
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> > > > Back to the first level.
```

> This is the first level of quoting.
>
> > This is nested blockquote.
>
> > > > Back to the first level.



# 5、列表

### 无序列表

```
- 列表内容
+ 列表内容
* 列表内容

注意：- + * 跟内容之间都要有一个空格
```

- 列表内容
+ 列表内容

* 列表内容

### 有序列表

*很重要的一点是，你在列表标记上使用的数字并不会影响输出的 HTML 结果*

```
你的标记写成：
1.  Bird
1.  McHale
1.  Parish

甚至：

8. Bird
1. McHale
4. Parish

效果都一样。
```

1.  Bird
2.  McHale
3.  Parish

8. Bird
9. McHale
10. Parish

### 列表可以嵌套

*上一级和下一级之间敲三个空格即可。*

```
* 一级无序列表内容

   * 二级无序列表内容
   * 二级无序列表内容
   * 二级无序列表内容
```

* 一级无序列表内容

   * 二级无序列表内容
   * 二级无序列表内容
   * 二级无序列表内容

*要让列表看起来更漂亮，你可以把内容用固定的缩进整理好：*

```
*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing
```

*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing

*列表项目可以包含多个段落，每个项目下的段落都必须缩进 4 个空格或是 1 个制表符：*

```
1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.
```

1. This is a list item with two paragraphs. Lorem ipsum dolor
   sit amet, consectetuer adipiscing elit. Aliquam hendrerit
   mi posuere lectus.

   Vestibulum enim wisi, viverra nec, fringilla in, laoreet
   vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
   sit amet velit.

2. Suspendisse id sem consectetuer libero luctus adipiscing. 



# 6、表格

```
表头|表头|表头
---|:--:|---:
内容|内容|内容
内容|内容|内容

第二行分割表头和内容。
- 有一个就行，为了对齐，多加了几个
文字默认居左
-两边加：表示文字居中
-右边加：表示文字居右
注：原生的语法两边都要用 | 包起来。此处省略
```

| 表头 | 表头 | 表头 |
| ---- | :--: | ---: |
| 内容 | 内容 | 内容 |
| 内容 | 内容 | 内容 |

# 7、代码

#### 单行代码

```
这里有一句代码`代码内容`。
```

这里有一句代码`代码内容`。

#### 代码块

```
\```
  代码...
  代码...
  代码...
\```
\ 是为了防止转译，实际是没有的。
```

```
  代码...
  代码...
  代码...
```



# 8、段落与换行

 **我们在两个不同的文字块之间，一定要空行以示区分，不然就会被归入同一文字块中。**

但有时也可以使用标记来强制空行和空格，比如需要首行缩进的时候： *一个空格大小的表示：\  或 \*  两个空格的大小表示：\ 或 \ *不换行空格：\ 或 \* 强制空行： \



# 9、纯文本进阶使用

#### 更改字体、大小、颜色

```
<font face="黑体">我是黑体字</font>
<font face="微软雅黑">我是微软雅黑</font>
<font face="STCAIYUN">我是华文彩云</font>
<font color=red>我是红色</font>
<font color=#008000>我是绿色</font>
<font color=Blue>我是蓝色</font>
<font size=5>我是尺寸</font>
<font face="黑体" color=green size=5>我是黑体，绿色，尺寸为5</font>
```

<font face="黑体">我是黑体字</font>
<font face="微软雅黑">我是微软雅黑</font>
<font face="STCAIYUN">我是华文彩云</font>
<font color=red>我是红色</font>
<font color=#008000>我是绿色</font>
<font color=Blue>我是蓝色</font>
<font size=5>我是尺寸</font>
<font face="黑体" color=green size=5>我是黑体，绿色，尺寸为5</font>

####  为文字添加背景色

```
<table><tr><td bgcolor=yellow>背景色yellow</td></tr></table>
```

<table><tr><td bgcolor=yellow>背景色yellow</td></tr></table>

####  设置文字居中

```
<center>居中</center>
<p align="left">左对齐</p>
<p align="right">右对齐</p>
```

<center>居中</center>
<p align="left">左对齐</p>
<p align="right">右对齐</p>

#### 加入上下标

```
H<sub>2</sub>O  CO<sub>2</sub>
爆米<sup>TM</sup>
```

H<sub>2</sub>O  CO<sub>2</sub>
爆米<sup>TM</sup>



# 9、进阶使用

#### 超链接

```
This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.
```

This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.

*如果想要在新页面中打开的话可以用html语言的a标签代替。*

```
<a href="超链接地址" target="_blank">超链接名</a>
```

<a href="超链接地址" target="_blank">超链接名</a>

#### 参考式的链接

*在链接文字的括号后面再接上另一个方括号，而在第二个方括号里面要填入用以辨识链接的标记：*

```
This is [an example][id] reference-style link.
```

*接着，在文件的任意处，你可以把这个标记的链接内容定义出来:*

```
[id]: http://example.com/  "Optional Title Here"
```

链接内容的形式为：  *方括号（前面可以选择性地加上至多三个空格来缩进），里面输入链接文字*  接着一个冒号  *接着一个以上的空格或制表符*  接着链接的网址  *选择性地接着 title 内容，可以用单引号、双引号或是括弧包着*  链接网址也可以用尖括号包起来：`[id]: <http://example.com/>  "Optional Title Here"`

#### 自动链接

```
<http://example.com/>
```

<http://example.com/>

#### 插入图片

*行内式*

```
![Alt pic](/path/to/img.jpg)

![Alt pic](/path/to/img.jpg "Optional title")
```

![Alt pic](/path/to/img.jpg)

![Alt pic](/path/to/img.jpg "Optional title")

*参考式*

```
![Alt pic][id]
```

![Alt pic][id]

```
[id]: url/to/image  "Optional title attribute"
```

[id]: url/to/image  "Optional title attribute"

*两个问题：1.如果使用本地路径插入本地图片，不灵活不好分享，本地图片的路径更改或丢失都会造成markdown文件调不出图。 2. 插入网络图片，则非常依赖网络，如果是本地图片，还需要先上传到网络服务器上。*

***上传本地图片方法***

1.将本地图片上传到github

首先在github中新建一个repo，然后git clone下来，然后把你想要的图片放到这个文件夹中然后上传，然后到GitHub中找到这个图片查看地址，在markdown中引用就好了。

2. * 把图片存入markdown文件

   * 用base64转码工具把图片转成一段字符串

   * 把字符串填到基础格式中链接的那个位置。

由于图片转成base64编码，会非常的大，一般至少都要上千行，这个时候会发现插入的这一长串字符串会把整个文章分割开，非常影响编写文章时的体验。这时候就可以用**参考式**，把大段的base64字符串放在文章末尾，然后在文章中通过一个id来调用，文章就不会被分割的这么乱了。

#### latex公式

```
$ X\stackrel{F}{\longrightarrow}Y $
```

$ X\stackrel{F}{\longrightarrow}Y $

#### 目录

```
[TOC]
```

[TOC]



