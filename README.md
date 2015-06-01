# GitHubHelp
GitHub help,About README.md help


①关于标题
=

▪大标题
====

在文本下面加上 等于号 = ，那么上方的文本就变成了大标题。等于号的个数无限制，但一定要大于0个。

▪中标题
-------

在文本下面加上下划线 - ，那么上方的文本就变成了中标题，同样的下划线个数无限制。

▪除此以外，关于标题还有等级表示法，分为六个等级，显示的文本大小依次减小。不同等级之间是以井号 # 的个数来标识的。一级标题有一个 #，二级标题有两个# ，以此类推。

#一级标题

##二级标题

###三级标题

####四级标题

#####五级标题

######六级标题

实际上，前文所述的大标题和中标题是分别和一级标题和二级标题对应的。三到六级没有下面的横线。


②显示文本
=

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

④插入代码
=

我们需要在代码的上一行和下一行用\`\`\` 标记。第一行后可加语言，可加亮代码。\`\`\` 不是三个单引号，而是数字1左边，Tab键上面的键。 示例如下：
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
如果你想使一段话中部分文字高亮显示，来起到突出强调的作用，可以把它用 \` \` 包围起来。

#⑤插入表格

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

#⑥以上基本够用了，不会的就用html标签。

markdown支持大部分的html文本编辑标签。例如换行，用<br>等。但markdown有些标签写起来要简洁得多。附：[markdown支持的html标签](https://github.com/github/markup/tree/master#html-sanitization)。

####以上资料来源于[jingwhale博客]("http://www.cnblogs.com/jingwhale/p/4223657.html")
