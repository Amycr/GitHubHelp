# GitHubHelp
GitHub help,About README.md help:How to write the README. Md.

#目录
* [关于标题](#title)
 * 大标题
 * 中标题
 * 标题等级
* [横线](#line) 
* [显示文本](#text)
 * 普通文本
 * 单行文本
 * 多行文本
 * 文字高亮
* [链接](#link)
 * 文字超链接
     * 链接外部URL
     * 链接本仓库里的URL
 * 锚点
* [插入图片](#image)
 * 显示图片
    * 来源于网络的图片
    * GitHub仓库中的图片
 * 图片超链接
* [列表](#list)
 * 圆点列表
 * 数字列表
 * 复选框列表
* [块引用](#reference)
* [插入代码](#code)
* [插入表格](#table)
* [表情](#expression)

<a name="title"/>
①关于标题
=

▪大标题
====

在文本下面加上 等于号 = ，那么上方的文本就变成了大标题。等于号的个数无限制，但一定要大于0个。

▪中标题
-------

在文本下面加上下划线 - ，那么上方的文本就变成了中标题，同样的下划线个数无限制。

▪标题等级:除此以外，关于标题还有等级表示法，分为六个等级，显示的文本大小依次减小。不同等级之间是以井号 # 的个数来标识的。一级标题有一个 #，二级标题有两个# ，以此类推。

#一级标题

##二级标题

###三级标题

####四级标题

#####五级标题

######六级标题

实际上，前文所述的大标题和中标题是分别和一级标题和二级标题对应的。三到六级没有下面的横线。

<a name="line"/>
#②横线
\*\*\*、\-\-\-、\_\_\_显示虚横线

***

---

___

<a name="text"/>
#③显示文本

###普通文本

这是一段普通的文本

####关于换行

回车不能换行，可以使用\<br>。但是使用html标签就丧失了markdown的意义。  可以在上一行文本后面补两个空格，  
这样下一行的文本就换行了。

或者就是在两行文本直接加一个空行。

也能实现换行效果，不过这个行间距有点大。

###单行文本
文本前面加Tab

    Hello,World.
    
###文本块

    欢迎使用GitHhub,
    祝您玩的愉快！
    
###部分文字高亮
需要高亮显示的文字用\`\`包裹起来：\`文本\`,该效果对‘文本前面加Tab’的内容无效

Hello,`World`.

    Hello,`World`.

####删除线
需要删除线显示的文字用\~~\~~包裹起来:\~~文本\~~

这是一个 ~~删除线~~

####斜体
需要斜体显示的文字用\*\*或\_\_包裹起来:\*文本\*或\_文本\_

*斜体1*  _斜体2_

####粗体
需要粗体显示的文字用\*\*\*\*或\_\_\_\_包裹起来:\*\*文本\*\*或\_\_文本\_\_

**粗体1**  __粗体2__



<a name="link"/>
#④链接
▪要显示一个超链接的话，就直接输入这个链接的URL

▪给一段文字加入超链接的格式：\[要显示的文字\]( 链接的地址 "悬停显示的字")。"悬停显示的字"是可选项。

▪插入圆点符，在文字前加\*，要注意的是星号* 后面要有一个空格。否则显示为普通星号。此外还有二级圆点和三级圆点。就是多加一个Tab。第二行一个Tab，第三行两个Tab。


https://www.google.com/?gws_rd=ssl

[谷歌](https://www.google.com/?gws_rd=ssl)

[谷歌](https://www.google.com/?gws_rd=ssl "点击链接跳转到谷歌")

* 前端开发
  * javascript*jquery
  *	html
  * css
    * html5

<a name="image">
③插入图片
=

▪第一种方法：!\[\](图片链接的地址 "悬停显示的字")。"悬停显示的字"是可选项。

▪第二种方法：GitHub仓库里的图片（建议使用这种方法，其他来源URL很可能会失效）。

前提是你的远程仓库有图片，图片链接的地址格式如下：

https://github.com/你的用户名/你的项目名/raw/分支名/存放图片的文件夹/该文件夹下的图片

其中，raw表示原数据的意思；主分支master。一般默认。

![](http://dl.bizhi.sogou.com/images/2015/05/13/1171967.jpg)

![](images/girl.jpg)

![](images/girl.jpg "阳光下的女孩")

<a name="code">
④插入代码
=

我们需要在代码的上一行和下一行用\`\`\` 标记。第一行后可加语言，可加亮代码。\`\`\` 不是三个单引号，而是数字1左边，Tab键上面的键。 示例如下：
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
如果你想使一段话中部分文字高亮显示，来起到突出强调的作用，可以把它用 \` \` 包围起来。

<a name="table">
#⑤插入表格

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

####说明

markdown支持大部分的html文本编辑标签。例如换行，用\<br\>等。但markdown有些标签写起来要简洁得多。附：[markdown支持的html标签](https://github.com/github/markup/tree/master#html-sanitization)。

####以上资料来源于[jingwhale博客](http://www.cnblogs.com/jingwhale/p/4223657.html)和 [Jelly-GitHub](https://github.com/guodongxiaren/README/blob/master/README.md)
