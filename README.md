#Markdown
@(Markdown)[使用技巧|markdown]

**主要内容**
>#####Markdown *是什么* ？
>#####*谁* 创造了它？
>#####*为什么* 使用它？
>#####*如何* 使用它？
>#####*什么地方* 可以使用它？

---------------------

##正文

###Markdown是什么？

Markdown是一种轻量级`标记语言`，  它是以（简单、易懂的语言编译）文档形式，并以HTML的格式发布。

###谁创造了它？

Markdown是由

###为什么使用它？

因为它使用方便，没有过多的难点和权限，并且你还会很**容易**的上手。
在文本呈现上，整个文本看起来**非常干净**，**重点**和**逻辑**十分突出，有一种来自 [幕布](https::/www.mubu.com/) 的芳香。

###如何使用它？

这里就是markdown重要的语法。其中主要有 **标题、段落、格式化、水平线、区块引用、代码块、标记、列表、链接、图片、反斜杠`\`**

####标题

标题有两种格式：
1）使用 `=` 和 `-` 来修饰。
> 一级标题
> `=============================`
> 二级标题
> `-----------------------------`

效果如下：
> 一级标题
> ===============================
> 二级标题
> ---------------------------------------------

2)使用`#`修饰。
> 一级标题
> `#`
> 二级标题
> `##`
> 三级标题
> `###`
> 四级标题
> `####`
> 五级标题
> `#####`
> 六级标题
> `######`

效果如下：
> #一级标题
> ##二级标题
> ###三级标题
> ####四级标题
> #####五级标题
> ######六级标题

####段落

段落的前后都需要空行，所谓空行就是没有内容的行。
如果想要段内强制换行，使用的方法是**两个以上的空格**加上回车。

####格式化

格式化分为`加粗`和`斜体`，使用`*`或`_`修饰。
> \*斜体\* 或 \_斜体\_
> \**加粗\* *或 \__加粗\__

效果如下：
> *斜体* 或 _斜体_
> **加粗** 或 __加粗__

####水平线

使用**三个或以上的**`-`、`*`或`_`修饰。
> \------------------------------------------
> \****************************************
> \__________________________________

效果如下：
> ---------------------------------------------
> *******************************************
> ___

####区块引用

使用`>`修饰。
> \>区块引用
> \>>嵌套区块引用

效果如下:
> 区块引用
>> 嵌套区块引用

####代码块

代码块的建立，需要每行前加`Tab`、`4个空格`或`制表符`。

普通块：

>void main() 
{
		printf("Hello，world");
}

代码块：

    void main()    
    
    {
    
    printf("Hello，world")；    
    
    }    
**注意**:需要和普通块区分`空行`。

####标记

使用`` ` 进行修饰。

> \`标记\`

效果如下:
> `标记`

####列表

无序列表：使用`.`、`+\*`和`-`修饰。

> \ - ( + \ * ) 第一项
	\ - ( + \ * ) 第二项	  
	\ - ( + \ * ) 第三项

效果如下:
> - 第一项
> - 第二项
> - 第三项

**注意**:符号前的**空格**确定项的等级,空格越多，等级越低。

有序列表：将上面的符号修改为`数字`，并用`.`进行修饰。

> 1\. 第一项
> 2\. 第二项
> 3\. 第三项

效果如下：
> 1. 第一项 
> 2. 第二项
> 3. 第三项

**注意**：标记后面至少有一个**符号**或**制表符**，如果不在区块内，则要用**空行分开**。

####链接

链接有两种形式，**链接式**和**参考式**。

**链接式**，如：
> \[Markdown\]\(https:://github.com/younghz/Markdown "Markdown"\)

 效果如下
 > [Markdown](https:://github.com/younghz/Markdown "Markdown")

**参考式**
> [Markdown ] [1] 
> [Markdown ] [2]
> 
>\[1\]: https://github.com/younghz/Markdown
>\[2\]: https://github.com/younghz/Markdown

效果如下：

> [Markdown ] [1] 
> [Markdown ] [2]

[1]: https://github.com/younghz/Markdown
[2]: https://github.com/younghz/Markdown


**注意**：`[0]: https://github.com/younghz/Markdown`不出现在代码块中。
`[]`后面不能有**空格**。

####图片

图片和链接使用方法类似，只是在之前加上一个`!`。

####反斜杠`\`

它(`\`)可以使Markdown语言中的符号，修改为普通符号，从而被显示出来。如：

符号显示：
> - 

写法如下：  
> `\- `

效果：
> \- 

###什么地方使用它？

Markdown使用者：
+ github
+ 简书
+ Reddit
+ Apollo
+ Stack Overflow
+ 等等

###其它

其中包括：**表格、公式、流程图、时序图**

表格的使用(非traditonal markdown)：

用`|`表示表格纵向边界，表头和表内容用`-`隔开，并可用`:`进行对齐设置，两边都有`:`则表示居中，若不加`:`则默认左对齐。

|代码库                              |链接                                |
|:------------------------------------:|------------------------------------|
|MarkDown                              |[https://github.com/younghz/Markdown](https://github.com/younghz/Markdown "Markdown")|
|MarkDownCopy                              |[https://github.com/younghz/Markdown](https://github.com/younghz/Markdown "Markdown")|

### 代码块
``` python
@requires_authorization
def somefunc(param1='', param2=0):
    '''A docstring'''
    if param1 > param2: # interesting
        print 'Greater'
    return (param2 - param1 + 1) or None
class SomeClass:
    pass
>>> message = '''interpreter
... prompt'''
```

### LaTeX 公式

可以创建行内公式，例如 $\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$。或者块级公式：

$$	x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a} $$

### 表格
| Item      |    Value | Qty  |
| :-------- | --------:| :--: |
| Computer  | 1600 USD |  5   |
| Phone     |   12 USD |  12  | 
| Pipe      |    1 USD | 234  |

### 流程图
```flow
st=>start: Start
e=>end
op=>operation: My Operation
cond=>condition: Yes or No?

st->op->cond
cond(yes)->e
cond(no)->op
```

以及时序图:

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```

> **提示：**想了解更多，请查看**流程图**[语法][3]以及**时序图**[语法][4]。

### 复选框

使用 `- [ ]` 和 `- [x]` 语法可以创建复选框，实现 todo-list 等功能。例如：

- [x] 已完成事项
- [ ] 待办事项1
- [ ] 待办事项2

> **注意：**目前支持尚不完全，在印象笔记中勾选复选框是无效、不能同步的，所以必须在**马克飞象**中修改 Markdown 原文才可生效。下个版本将会全面支持。
*********
##资料参考

+ [Markdown基本语法](https://github.com/younghz/Markdown)_作者：younghz
+ [马克飞象](https://maxiang.io/#)
***
  [3]: http://adrai.github.io/flowchart.js/
  [4]: http://bramp.github.io/js-sequence-diagrams/
  [5]: https://dev.yinxiang.com/doc/articles/enml.php

