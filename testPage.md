---
title: testPage 这是一个页面的标题
toc: yes
categories: test, new page,语法 markdown
format: markdown
---

> This is a test page.

# First Menu

### Using


* input `http://www.ccyuki.com:7500/testPage`
* click `click create a new page`
* finish

# Second Menu

#### Wiki links
```
链接页面方式：[something](Page Name)

注意页面名称可以包含空格和特殊字符。不需要CamelCase(骆驼命名)。CamelCase单词不会自动转化为wiki链接。 
Wiki页面可以组织成目录。例如: 
Wine/Pinot Noir 
Wine/Burgundy 
Wine/Cabernet Sauvignon
```
#### 上传文件
```
可以上传一个文件——图片、PDF、或其他一些resource。

点击“upload”按钮在导航栏中。系统将提示你选择要上传的文件。 
需要对上传的文件或资源有一个简单的description。 
通常你可以离开“Name on wiki”空白,因为现有的文件将使用默认的名称。如果不想要这个,可以自己提供一个名字。注意,上传的文件必须包括一个文件扩展名(例如pdf格式)。 
如果你提供一个新版本的文件已经存在于wiki,选择复选框“覆盖现有的文件”。 
链接到一个上传文件,就是用它的名字在一个常规wiki链接。例如,如果你上传一张fido.jpg,可以插入图片(markdown-formatted)页面如下: ![fido](fido.jpg)。如果你上传一个PDFprojection.pdf,你可以插入的链接使用:[projection](projection.pdf)。
```

# Markdown语法
```
一级标题
=========
二级标题
---------
```
一级标题
=========
二级标题
---------
```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题


- [ ] Eat
- [x] Code
  - [x] HTML
  - [x] CSS
  - [x] JavaScript
- [ ] Sleep

4.2 段落

段落的前后要有空行，所谓的空行是指没有文字内容。若想在段内强制换行的方式是使用两个以上空格加上回车（引用中换行省略回车）。

4.3 区块引用

在段落的每行或者只在第一行使用符号>,还可使用多个嵌套引用，如：

    > 区块引用
    >> 嵌套引用

效果：

 > 区块引用
 >> 嵌套引用

4.4 代码区块

代码区块的建立是在每行加上4个空格或者一个制表符（如同写代码一样）。如
普通段落：

void main()
{
printf("Hello, Markdown.");
}

代码区块：

    void main()
    {
        printf("Hello, Markdown.");
    }
    
注意:需要和普通段落之间存在空行。

4.5 强调

在强调内容两侧分别加上*或者_，如：

    *斜体*，_斜体_
    **粗体**，__粗体__

效果：

*斜体*，_斜体_
**粗体**，__粗体__

4.6 列表

使用·、+、或-标记无序列表，如：

    -（+*） 第一项 -（+*） 第二项 - （+*）第三项

注意：标记后面最少有一个_空格_或_制表符_。若不在引用区块中，必须和前方段落之间存在空行。

效果：

第一项
第二项
第三项

有序列表的标记方式是将上述的符号换成数字,并辅以.，如：

1. 第一项
2. 第二项
3. 第三项

效果：

1. 第一项
2. 第二项
3. 第三项

4.7 分割线

分割线最常使用就是三个或以上*，还可以使用-和_。

*******
-------
_______

4.8 链接

链接可以由两种形式生成：行内式和参考式。
行内式：

    [Markdown库](https:://github.com/younghz/Markdown "Markdown")。

效果：
[Markdown库](https:://github.com/younghz/Markdown "Markdown")。

参考式：

    [younghz的Markdown库1][1]
    [younghz的Markdown库2][2]
    [1]:https:://github.com/younghz/Markdown "Markdown"
    [2]:https:://github.com/younghz/Markdown "Markdown"

效果：

[younghz的Markdown库1][1]

[younghz的Markdown库2][2]

[1]:https:://github.com/younghz/Markdown "Markdown"
[2]:https:://github.com/younghz/Markdown "Markdown"

    注意：上述的[1]:https:://github.com/younghz/Markdown "Markdown"不出现在区块中。

4.9 图片

添加图片的形式和链接相似，只需在链接的基础上前方加一个！。
   
    [icon.png](./images/icon.png)

![GitHub](https://avatars2.githubusercontent.com/u/3265208?v=3&s=100 "GitHub,Social Coding")

4.10 反斜杠\

相当于反转义作用。使符号成为普通符号。

4.11 符号'`'

起到标记作用。如：

    `ctrl+a`

效果：
`ctrl+a`

4.11 删除'~'

起到删除作用。如：

    ~~ctrl+a~~

效果：

~~ctrl+a~~

其它：

列表的使用(非traditonal markdown)：

用|表示表格纵向边界，表头和表内容用-隔开，并可用:进行对齐设置，两边都有:则表示居中，若不加:则默认左对齐。

| left | center | right |
| :--- | :----: | ----: |
| aaaa | bbbbbb | ccccc |
| a    | b      | c     |

|     name     | age |             blog                |
| ------------ | --- | ------------------------------- |
| _LearnShare_ |  12 | [LearnShare](http://xianbai.me) |
| __Mike__     |  32 | [Mike](http://mike.me)          |