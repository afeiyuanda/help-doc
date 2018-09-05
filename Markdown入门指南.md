# Markdown入门指南

> Writing is about content, about what you want to say – not about fancy formatting.

## 什么是Markdown？

**Markdown**是一种 _轻量级的标记语言_，易读、易写、适用于网络书写。

### 无处不在的Markdown

* 个人笔记、博客网站，如[印象笔记][evernote]、[马克飞象][maxiang]、[简书][jianshu]、[WordPress][wordpress]、Tumblr等都支持Markdown语法
* Seqrise的数据集说明、SevenBridge的工具说明等都支持Markdown语法
* 很多的知识库、技术文档、开发文档使用Markdown书写
* *.etc*

## Markdown语法实例

### 段落标题

语法格式：

```
# 一级标题
## 二级标题
###### 六级标题
```

### 链接

这是[BMKCloud官网](http://www.biocloud.net/)链接的例子。

### 图片

下面是插入**本地图片**和**网络图片**的例子：

![Earth](basic_img/info-circle.png)

![Logo](http://www.biocloud.net/wp-content/uploads/2017/01/logo_big.png)


### 列表

下面是**无序列表**：

* 项目一  `* + 空格`
* 项目二
    * 子项目一
    * 子项目二
* 项目三

下面是**有序列表**：

1. 项目一 `数字 + . + 空格`
3. 项目二 
    1. 子项目一
    2. 子项目二
1. 项目三

### 引用

> 开卷有益。

### 表格

下面是表格的例子：

|第一列|第二列|第三列|
|:---|:--:|--:|
|a|b|c|
|1|2|3|

### 代码块

这是一个`print`。

下面是一段==perl代码==：

```perl
sub say_hello {
    print "hello, markdown.";
}
```

### 目录

[TOC]

### 行内格式

* ~~删除线~~
* _下划线_
* **重点**
* ==高亮==
* 上角标^(上角标)
* *斜体*

### 更多

见Gitbook上的 [Gitbook 学习使用笔记](https://zq99299.gitbooks.io/gitbook-guide/)、[Markdown 简单的世界](https://wizardforcel.gitbooks.io/markdown-simple-world/)等。

## Markdown书写工具

_任何文本编辑器_都可以用来书写Markdown文档。

### MWeb

[MWeb](http://zh.mweb.im/)适用于个人文档库、静态博客的书写。目前只有iOS版本。

MWeb特性：

* 自定义编辑器主题
* 自定义预览样式（CSS，定义字体、字号等）
* 自定义静态网站模板
* 文档历史版本

### Atom

开源社区GitHub出的**[Atom](https://atom.io/)**是一个功能极其强大的开源文本编辑器。

安装Markdown预览插件[markdown-preview](https://atom.io/packages/markdown-preview)，使用ctrl+shift+m预览。

### Gitbook

**[Gitbook](https://www.gitbook.com/)**适合于 _团队合作_书写大型文档。

及其强大的

使用Gitbook书写的《[Gitbook 学习使用笔记](https://zq99299.gitbooks.io/gitbook-guide/)》。

Info styling
> **[info] For info**
>
> Use this for infomation messages.

Warning styling
> **[warning] For warning**
>
> Use this for warning messages.

Danger styling
> **[danger] For danger**
>
> Use this for danger messages.

Success styling
> **[success] For info**
>
> Use this for success messages.


{% includeCsv src="./other/test.csv", encoding="utf-8", useHeader="true" %}{% endincludeCsv %}


[evernote]: https://www.yinxiang.com/
[maxiang]: https://maxiang.io/
[jianshu]: http://www.jianshu.com/
[wordpress]: https://cn.wordpress.org

