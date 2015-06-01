# GitHubHelp <a name="TEST"/>
GitHub help,About README.md help:How to write the README. Md.

<a name="index"/>
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

###关于换行

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
需要高亮显示的文字用\`\`包裹起来：\`文本\`

Hello,`World`.

###删除线
需要删除线显示的文字用\~~\~~包裹起来:\~~文本\~~

这是一个 ~~删除线~~

###斜体
需要斜体显示的文字用\*\*或\_\_包裹起来:\*文本\*或\_文本\_

*斜体1*  _斜体2_

###粗体
需要粗体显示的文字用\*\*\*\*或\_\_\_\_包裹起来:\*\*文本\*\*或\_\_文本\_\_

**粗体1**  __粗体2__

<a name="link"/>
#④链接

###链接外部URL
▪要显示一个超链接的话，就直接输入这个链接的URL

▪给一段文字加入超链接的格式：\[要显示的文字\](链接的地址 "悬停显示的字")。"悬停显示的字"是可选项。

▪给一段文字加入超链接的格式：

\[要显示的文字\]\[id\]

\[id\]:链接的地址 "悬停显示的字"

"悬停显示的字"是可选项。中括号\[\]里的id，可以是数字，字母。这两行可以不连着写，一般把第二行的链接统一放在文章末尾，id上下对应就行了。这样正文看起来会比较干净。

https://github.com/

[GitHub](https://github.com/)

[GitHub](https://github.com/ "点击链接跳转到GitHub")

[GitHub][1]
[1]:https://github.com/ "点击链接跳转到GitHub"

###链接本仓库里的URL

[images](./images)

###锚点
我们可以使用HTML的锚点标签来设置锚点：[回到目录](#index)  
但其实呢，每一个标题都是一个锚点，不需要用标签来指定，比如我们 [回到顶部](#TEST)

<a name="image">
#⑤插入图片

▪第一种方法：!\[\](图片链接的地址 "悬停显示的字")。"悬停显示的字"是可选项。

▪第二种方法：GitHub仓库里的图片（建议使用这种方法，其他来源URL很可能会失效）。

前提是你的远程仓库有图片，图片链接的地址格式如下：

https://github.com/你的用户名/你的项目名/raw/分支名/存放图片的文件夹/该文件夹下的图片

其中，raw表示原数据的意思；主分支master。一般默认。

![](http://dl.bizhi.sogou.com/images/2015/05/13/1171967.jpg)

###GitHub仓库中的图片

![](images/girl.jpg)

![](images/girl.jpg "阳光下的女孩")

###<a name="piclink">给图片加上超链接
[![image]](http://dl.bizhi.sogou.com/images/2015/05/13/1171967.jpg)
[image]:http://dl.bizhi.sogou.com/images/2015/05/13/1171967.jpg "阳光下的女孩"

<a name="list"/>
#⑥列表
▪插入圆点符，在文字前加\*，要注意的是星号* 后面要有一个空格。否则显示为普通星号。此外还有二级圆点和三级圆点。就是多加一个Tab。第二行一个Tab，第三行两个Tab。

* 前端开发
  * javascript*jquery
  *	html
  * css
    * html5


###数字列表

####一般效果
就是在数字后面加一个点，再加一个空格。不过看起来起来可能不够明显。    
面向对象的三个基本特征：

1. 封装
2. 继承
3. 多态

####数字列表自动排序
也可以在第一行指定`1. `，而接下来的几行用星号`*`（或者继续用数字1. ）就可以了，它会自动显示成2、3、4……。    
面向对象的七大原则：

1. 开闭原则
* 里氏转换原则
* 依赖倒转原则
* 接口隔离原则
* 组合/聚合复用原则
* “迪米特”法则
* 单一直则原则

####多级数字列表
和圆点的列表一样，数字列表也有多级结构：  

1. 这是一级的数字列表，数字1还是1
   1. 这是二级的数字列表，阿拉伯数字在显示的时候变成了罗马数字
      1. 这是三级的数字列表，数字在显示的时候变成了英文字母
	    1. 四级的数字列表显示效果，就不再变化了，依旧是英文字母

### 复选框列表
- [x] C
- [x] C++
- [x] Java
- [ ] C#

<a name="reference"/>
#⑦块引用

###常用于引用文本
####文本摘自《深入理解计算机系统》P27
　令人吃惊的是，在哪种字节顺序是合适的这个问题上，人们表现得非常情绪化。实际上术语“little endian”（小端）和“big endian”（大端）出自Jonathan Swift的《格利佛游记》一书，其中交战的两个派别无法就应该从哪一端打开一个半熟的鸡蛋达成一致。因此，争论沦为关于社会政治的争论。只要选择了一种规则并且始终如一的坚持，其实对于哪种字节排序的选择都是任意的。
><b>“端”（endian）的起源</b><br>
以下是Jonathan Swift在1726年关于大小端之争历史的描述：<br>
“……下面我要告诉你的是，Lilliput和Blefuscu这两大强国在过去36个月里一直在苦战。战争开始是由于以下的原因：我们大家都认为，吃鸡蛋前，原始的方法是打破鸡蛋较大的一端，可是当今的皇帝的祖父小时候吃鸡蛋，一次按古法打鸡蛋时碰巧将一个手指弄破了，因此他的父亲，当时的皇帝，就下了一道敕令，命令全体臣民吃鸡蛋时打破较小的一端，违令者重罚。”

###块引用有多级结构
>数据结构
>>树
>>>二叉树
>>>>平衡二叉树
>>>>>满二叉树


<a name="code">
#⑧插入代码
我们需要在代码的上一行和下一行用\`\`\` 标记。第一行后可加语言，可加亮代码。\`\`\` 不是三个单引号，而是数字1左边，Tab键上面的键。 示例如下：
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
```Java
public static void main(String[]args){} //Java
```
```c
int main(int argc, char *argv[]) //C
```
```Bash
echo "hello GitHub"#Bash
```
```javascript
document.getElementById("myH1").innerHTML="Welcome to my Homepage"; //javascipt
```
```cpp
string &operator+(const string& A,const string& B) //cpp
```

如果你想使一段话中部分文字高亮显示，来起到突出强调的作用，可以把它用 \` \` 包围起来。

<a name="table">
#⑨插入表格

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| 表头1  | 表头2|
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| 名字 | 描述          |
| ------------- | ----------- |
| Help      | Display the help window.|
| Close     | Closes a window     |

表格中也可以使用普通文本的删除线，斜体等效果

| 名字 | 描述          |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |

表格可以指定对齐方式

| 左对齐 | 居中  | 右对齐 |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |

<a name="expression"/>
#⑩表情
Github的Markdown语法支持添加emoji表情，输入不同的符号码（两个冒号包围的字符）可以显示出不同的表情。

比如`:blush:`，可以显示:blush:。

具体每一个表情的符号码，可以查询GitHub的官方网页[http://www.emoji-cheat-sheet.com](http://www.emoji-cheat-sheet.com)。


####说明

markdown支持大部分的html文本编辑标签。例如换行，用\<br\>等。但markdown有些标签写起来要简洁得多。附：[markdown支持的html标签](https://github.com/github/markup/tree/master#html-sanitization)。

####以上资料来源于[jingwhale博客](http://www.cnblogs.com/jingwhale/p/4223657.html)和 [Jelly-GitHub](https://github.com/guodongxiaren/README/blob/master/README.md)
