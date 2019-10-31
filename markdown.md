# **Markdown**
# Headers（标题）
几级标题就用几个"#"，最多支持六级标题
# this is a <h1> tag（一级标题）
## This is an <h2> tag（二级标题）
###### This is an <h6> tag（六级标题）
    
# Emphasis（强调）
强调是通过在文字两侧加入星号（*）、下划线（_）和波浪线（~）等符号实现的，注意符号和需要强调的文字之间没有空格！

*This text will be italic*（包括在两个*之间的文字为斜体，其他类似）

_This will also be italic_（斜体）

**This text will be bold**（黑体）

__This will also be bold__（黑体）

~~This text will be deleted~~（删除线）

_You **can** combine them_（可以多种格式复合使用）

# List（列表）
## Unordered（无序列表）
无序列表用 - + * 任何一种都可以，注意符号和文字之间有空格！

* Item 1
* Item 2
    + Item 2a
        - Item 2aa
            * Item 2aaa

## Ordered（顺序列表）
使用数字加点的方式，数字和点之间没有空格，而点和后面的文字之间有空格！无序列表和有序列表都可以进行嵌套。

1. Item 1
1. Item 2
    * Item 2a（无序）
    * Item 2b（无序）
1. Item 3
    1. Item 3a
    2. Item 3b
    3. Item 3C

# Blockquotes（引用）
引用的内容可以用 >来表示，比如本文中所有对命令的说明都采用了引用的方式。
> We're living the future so
> the present is our past.

# Code（代码）
## Inline code（行内代码）
代码之间分别用一个反引号包起来。

` print 'Hello world!' `

## Code blocks（代码块）

连用三个反引号将代码包起来。

```
def f(x):
    return x**2 + 2*x + 1
```
# Horizontal rules（分割线）

三个或者三个以上的 - 或者 * 都可以。

---
或者
***

# Useful syntax（插入对象）
这一部分主要介绍如何插入一些有用的对象，比如表格、图像和公式等，以及其他一些有用的语法。

## Tables（表格）

表格的插入非常简单，只需要按照如下语法画出表格形状即可，在编辑代码时不需要考虑对齐（但是为了美观和逻辑的直观，建议代码整齐）。竖线（|）用于分栏，短横线（-）用于分割表头和其余部分，冒号（:）用于标记表格内容的对齐方式（默认为左对齐）。如果嫌麻烦，这里有个神奇的表格生成网站[神奇的表格生成网站](https://www.tablesgenerator.com/markdown_tables "表格生成网站")，可以直接生成你所需要的代码，而且不止有Markdown代码，还有Latex和HTML代码！

|表头|表头|表头|
|:-------|:------:|------:|
|内容|内容|内容|
|内容|内容|内容|
|内容|内容|内容|

## Images（图像）
用 `![名称]( 图片地址 "标题") `可以添加在线图片或本地图片，其中标题为可选项。添加本地图片需要注意，使用jupyter notebook或lab的时候，图片必须放在程序所在文件夹或所在文件夹的子文件夹下！

![Github](https://github.githubassets.com/images/icons/emoji/octocat.png "title 添加在线图片")（添加在线图片）



![Github](/images/logo.png "title 添加本地图片")（添加本地图片）

## Links（链接）
用 `[名称](地址 "标题")` 可以添加超链接，语法和添加图片类似，只是少了叹号。

[GitHub](http://github.com "title GitHub")

## Equations（公式）
公式的编辑采用Latex语法，如果读者对Latex语法不熟悉，同样为大家提供一个神奇的网站[神奇的网站](https://www.codecogs.com/latex/eqneditor.php "公式生成网站")。

这是行内公式：
$E=mc^2$

这是公式块：
$$
e^{i\theta} = \cos \theta +i\sin \theta \
e^z = 1 + \frac{z}{1!} + \frac{z^2}{2!} + \frac{z^3}{3!} + \cdots = \sum_{n=0}^{\infty}\frac{z^n}{n!}
$$

![公式图片](https://latex.codecogs.com/gif.latex?E=Mc^{2} "E=mc^2")

## Backslash（反斜线）
如果想要插入以上内容中用到的一些符号（字面上，而非功能性应用），比如希望插入星号（*），但不是用这个星号来表示斜体或加粗等，那么可以在符号前面加反斜线（\）以插入这些普通符号。

```
\ 反斜线
` 反引号
* 星号
_ 底线
{} 花括号
[] 方括号
() 括弧
# 井字号
+ 加号
- 减号
. 英文句点
! 惊叹号
```

## Footnotes（脚注）
脚注可以用于编辑参考文献[^1]。

`在文中使用[^1]的方式标记脚注，
在文末使用[^1]:加入参考文献，注意要使用英文冒号，后面有无空格均可。`


[^1]:https://github.com/doublewaters/Learning-Markdown 
