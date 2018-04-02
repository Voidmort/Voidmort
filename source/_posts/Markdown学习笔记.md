---
title: Markdown学习笔记
date: 2018-03-30 12:02:27
tags: markdown
categories: 学习笔记
---

初次写博客，从搭建github hexo走了不少坑，稍后记录搭建博客过程，首先学习使用markdown
教程来源：http://www.markdown.cn/
markdown是一个HTML的转换工具，是HTML的书写格式

# 标题语法

类Atx形式在首行插入1个到6个#，对应到标题1到6
一定要# + 空格 + 标题
加空格！！！！！！
```	
	# 一级标题
	## 二级标题
	###### 六级标题
```

# 区块引用
段首使用 > 作为引用，引用部分也支持markdown语法
```	
	>hello word!
	># 标题一
	>代码提示：
	>    return Null;
```
>hello word!
># 标题一
>代码提示：
>    return Null;

# 列表
markdown支持有序和无序列表
无序列表标记符号可以是“* + -”，有序符号是数字加英文点“1. ”

```	
	* red
	* green
	* blue
	+ red
	+ green
	- red
	1.good
	2.name
	3.learn 
```

* red
* green
* blue
+ red
+ green
- red
1. good
2. name
3. learn

# 代码区块

要在 Markdown 中建立代码区块很简单，只要简单地缩进 4 个空格或是 1 个制表符就可以，例如，下面的输入：
这是一个普通段落：

```
    //这是一个代码区块。
	#include <stdio.h>
	#include <stdlib.h>
	
	int main()
	{
		print("Hello word!\n");
		return 0;
	}
```

# 分割线
三个连续的* - _	
	*********************
************************

# 链接
链接文字用[方括号]标记
要建立一个内行式链接，只要在方括号后面紧接着元括号并插入网址链接
	
	This is [an example](http://example.com/ "Title") inline link.
	[This link](http://example.net/) has no title attribute.


[百度一下](http://www.baidu.com/ "百度")
This is [an example](http://example.com/ "Title") inline link.
[This link](http://example.net/) has no title attribute.

# 代码
标记段行内代码，用反引号包起来（'）

	use the 'printf()' function

Use the `printf()` function.

# 图片
和链接一样
```
	![Alt text](/path/to/img.jpg)
	![Alt text](/path/to/img.jpg "Optional title")
```
[Alt text](/path/to/img.jpg)

详细叙述如下：

一个惊叹号 !
接着一个方括号，里面放上图片的替代文字
接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上 选择性的 'title' 文字。

# 其他
## 反斜杠
在一下符号前面加入反斜杠来插入普通符号：

```	
	\   反斜线
	`   反引号
	*   星号
	_   底线
	{}  花括号
	[]  方括号
	()  括弧
	#   井字号
	+   加号
	-   减号
	.   英文句点
	!   惊叹号
```

## 自动链接
处理短链接用<>括住能够自动转换成链接
<http://www.baidu.com>
<wxj5658@hotmai.com>

# 编辑软件
windows平台
* [Markdownpad](http://markdownpad.com/ "markdownpad")

激活：

```
	注册信息

	邮箱地址：

	Soar360@live.com

	授权密钥：
	GBPduHjWfJU1mZqcPM3BikjYKF6xKhlKIys3i1MU2eJHqWGImDHzWdD6xhMNLGVpbP2M5SN6bnxn2kSE8qHqNY5QaaRxmO3YSMHxlv2EYpjdwLcPwfeTG7kUdnhKE0vVy4RidP6Y2wZ0q74f47fzsZo45JE2hfQBFi2O9Jldjp1mW8HUpTtLA2a5/sQytXJUQl/QKO0jUQY4pa5CCx20sV1ClOTZtAGngSOJtIOFXK599sBr5aIEFyH0K7H4BoNMiiDMnxt1rD8Vb/ikJdhGMMQr0R4B+L3nWU97eaVPTRKfWGDE8/eAgKzpGwrQQoDh+nzX1xoVQ8NAuH+s4UcSeQ==
```

在windows 10 系统下，windows10 MarkdownPad html会产生一个 渲染错误 awesomium（ This view has crashed ），此时就需要下载一个 HTML UI ENGINE（awesomium_v1.6.6_sdk_win）去解决该错误，该组件的下载地址：
 http://markdownpad.com/download/awesomium_v1.6.6_sdk_win.exe