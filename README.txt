HTML 作用：展示网页结构
HTML 的 tag 包括哪些？？？？
HTML 的属性都包括哪些？？？？
<!DOCTYPE html> 作用是什么？？？
========================================================================================================
HTML head 元素：
HTML head 元素 规定文档相关的配置信息（元数据），包括文档的标题（title），引用的文档样式(css)和脚本(script)等。
1.title
title 出现在标签栏中。同样，当你把页面存为书签时，存的也是 title。title的内容同样会出现在搜索的结果中。

2.meta
meta 是用来描述数据的数据。其作用是描述这个文档。
可以指定文档中的字符编码。<meta charset="utf-8">
可以添加作者和描述。name 指定了meta 元素的类型； 说明该元素包含了什么类型的信息。content 指定了实际的元数据内容。
指定包含关于页面内容的关键字的页面内容的描述是很有用的，因为它可能或让你的页面在搜索引擎的相关的搜索出现得更多 

2.添加图标
页面添加图标的方式有：

将其保存在与网站的索引页面相同的目录中，以.ico格式保存（大多数浏览器将支持更通用的格式，如.gif或.png，但使用ICO格式将确保它能在如Internet Explorer 6一样久远的浏览器显示）
将以下行添加到HTML <head>中以引用它：
<link rel="shortcut icon" href="favicon.ico" type="image/x-icon">

3.在head中添加css和javascript
添加css的方法：
放在head
<link rel="stylesheet" href="my-css-file.css">
如何引入多个css，为什么要引入多个css

添加javascript的方法
没必要放在head
<script src="my-js-file.js"></script>
如何引入多个 script，为什么要引入多个 script


========================================================================================================
文字处理
span 和 p 的区别？？？？？？？
1.文字结构化处理的方法：
使用 p 和 h
2.列表Lists
列表分为无序列表(ul)和有序列表(ol)。列表中的某一项用 li 来表示。
嵌套列表。将一个列表嵌套到另一个列表中。（所有元素理论上都可以嵌套）
3.重点强调
斜体强调： <em></em>
黑体强调：<strong></strong>

========================================================================================================
超链接 a
超链接的意义在于将文档链接到其它文档。
创建超链接：
1.使用<a></a>   (archor)
<a href="http://www.google.com">GOOGLE</a>
2.使用title属性添加支持信息
<a href="https://www.mozilla.org/en-US/"
   title="The best place to find more information about Mozilla's
          mission and how to contribute">the Mozilla homepage</a>
当鼠标悬停的时候，会出现title所提供的信息。
3.可以把内容或者块级元素转成链接。只需把内容防盗啊<a></a>中
<a href="https://www.mozilla.org/en-US/">
  <img src="mozilla-image.png" alt="mozilla logo that links to the mozilla homepage">
</a>
4.URL与path
URL： uniform resource locator
这里涉及到网页的结构：
当在网站上工作时， 你会有一个包含整个网站的目录。一般在根目录中会有一个 index.html 。
而这个 index.html 就是第一个呈现给你的网页。
path这里指的是相对路径。以当前网页为基准，进行导向。
5.文档片段
超链接除了链接到文档外，也可以链接到HTML文档的特定部分（被称为文档片段）。要做到这一点，你必须首先给要链接到的元素分配一个id属性。
<h2 id="Mailing_address">Mailing address</h2>
然后链接到那个特定的id，您可以在URL的结尾使用一个井号指向它，例如：

<p>Want to write us a letter? Use our <a href="contacts.html#Mailing_address">mailing address</a>.</p>
你甚至可以在同一份文档下，通过链接文档片段，来链接到同一份文档的另一部分：

<p>The <a href="#Mailing_address">company mailing address</a> can be found at the bottom of this page

6.电子邮件链接
当点击一个链接或按钮时，打开一个新的电子邮件发送信息而不是连接到一个资源或页面，这种情况是可能做到的。这样做是使用<a>元素和mailto：URL的方案。
其最基本和最常用的使用形式为一个mailto:link （链接），链接简单说明收件人的电子邮件地址。例如:

<a href="mailto:nowhere@mozilla.org">Send email to nowhere</a>

除了电子邮件地址，您还可以提供其他信息。事实上，任何标准的邮件头字段可以被添加到你提供的邮件URL。 其中最常用的是主题(subject)、抄送(cc)和主体(body) (这不是一个真正的头字段，但允许您为新邮件指定一个短内容消息)。 每个字段及其值被指定为查询项。

下面是一个包含cc、bcc、主题和主体的示例：

<a href="mailto:nowhere@mozilla.org?cc=name2@rapidtables.com&bcc=name3@rapidtables.com&subject=The%20subject%20of%20the%20email&body=The%20body%20of%20the%20email">
  Send mail with cc, bcc, subject and body
</a>


========================================================================================================
高阶文字排版
https://developer.mozilla.org/zh-CN/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting

========================================================================================================
文档组成部分
布局细节
https://developer.mozilla.org/zh-CN/docs/Learn/HTML/Introduction_to_HTML/%E6%96%87%E4%BB%B6%E5%92%8C%E7%BD%91%E7%AB%99%E7%BB%93%E6%9E%84

========================================================================================================
HTML 调试
https://developer.mozilla.org/zh-CN/docs/Learn/HTML/Introduction_to_HTML/Debugging_HTML
========================================================================================================
HTML 调试


HTML 元素类型分为内联元素（inLine level）和块级元素(block level)。
内联元素的意思是，元素会在同一行中紧密排列。
块级元素是指每个元素都单独占一行。


HTML 中的特殊字符
在HTML中，字符 <, >,",' 和 & 是特殊字符. 它们是HTML语法自身的一部分, 那么你如何将这些字符包含进你的文本中呢, 比如说如果你真的想要在文本中使用符号&或者小于号, 而不想让它们被浏览器视为代码并被解释?

我们必须使用字符引用 —— 表示字符的特殊编码, 它们可以在那些情况下使用. 每个字符引用以符号&开始, 以分号(;)结束.

原义字符	等价字符引用
<	&lt;
>	&gt;
"	&quot;
'	&apos;
&	&amp;
在下面的例子中你可以看到两个段落，它们在谈论web技术:

<p>HTML 中用 <p> 来定义段落元素。</p>

<p>HTML 中用 &lt;p&gt; 来定义段落元素</p>






CSS 作用：展示网页样式

JS 作用：展示网页逻辑 DOM 

DOM --- Document Object Model
DOM 是一个树状结构。

HTML 文件中的所有 Object 组成一个 Object —— document
可以通过 document 来访问 HTML 中的 Object。返回 结果是一个 Array
document.getElementsByTagName("body") 或者用别的方法 .getElementsById

. 表示类。可以用于 HTML 生成含有某个类的.

HTML tag 后面跟的是 attribute
<h1 id="sp-list"></h1>   这里的 id 就是 attribute

