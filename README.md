# Learning Html, JavaScript, CSS 
学习HTML,JavaScript + CSS中，于2026年4月2日开始

目前仅仅使用该学习网站： [Developer.Mozilla.org](https://developer.mozilla.org/zh-CN/docs/Learn_web_development/Getting_started/Your_first_website/Creating_the_content) 与该视频： [YouTube.com](https://youtu.be/6HHN0G2cwBM)

目前仅使用该工具：[VsCode.Dev](https://vscode.dev)

目前计划为：
~~目标为制作一个画画网站，可以画画并保存~~ 将我学到的东西弄成一个网站

# Index:
[2026/04/02 21:34](#20260402-2134) 
<br>
[2026/04/04](#20260404)


# **2026/04/02 21:34**
## 先做到这里：https://youtu.be/6HHN0G2cwBM?t=1121

# TODO:
虽然说已经学了挺多了，但有些东西还需要稍加稳固一下，或者也许在再看Mozilla.org的教程时会再次学到？

明天要把视频看完，并且再弄个总结。

## **到现在学到的东西**：
# HTML:
`<!DOCTYPE html>` = 类型？

`<html lang= "zh"></html>` = html语言等于中文

`<head></head>` = 头部文件（不会在网站内显示）

`<meta name="viewport" content="width=device-width" />` = ?

`<title></title>` = 标题

`<link rel="stylesheet" href"/style/style.css">` = 从 `/style/style.css`导入CSS文件

`<body></body>` = 网页中所有的主要内容

`<nav></nav>` = 网页中的导航栏

`<main></main>` = 主要内容

`<header></header>` = 头部内容 / 页眉

`<h1> -> <h6>` = 标题，子标题等...

`<p></p>` = 普通文字

`<a href="link">文字</a>` = 在某文字中插入链接

`<img src="图片链接" width="宽度" height="高度" alt="Alt 文字">` = 插入图片

`<br>` = 在文字/内容中换行

`<blockquote cite="link?">"君子藏器而身，<br>待时而动。"</blockquote>` = 引用代码（blockquote）然后也可以加上 cite="link"来添加引用的链接？）：

`<strong></strong>` = 类似MD的 `**<文字>**`

`<ol>     <li>1</li>  <li>2</li>   </ol>` = 有数字的列表（`ol` + `li`）

`<ul>     <li>1</li>  <li>2</li>   </ul>` = 无数字的列表（`ul` + `li`）

`<section class=""></section>` = "HTML `<section>` 元素表示 HTML 文档中一个通用独立章节，它没有更具体的语义元素来表示。一般来说会包含一个标题。" -- [Mozilla.org](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Reference/Elements/section)

`<footer>Copytight © 2026 1224HuangJin 版权所有</footer>` = 最下面的文字 / 页脚，通常用于显示版权信息等。。。

# CSS:
（以下内容基本皆来自： [PAPAYA 电脑教室](https://www.youtube.com/watch?v=6HHN0G2cwBM) 的视频内）

选定某个元素，比如说：

```
a{
    }
```

（其实也可以弄`<a></a>`，`<p></p>`，`<h1></h1>`，`<header>`等等。。）
然后，你可以在内部添加内容

示例：

```
header {
    background-color: black;
    height: 100px;
    width: 100%;
    position: relative;
}
```

注意，如何要更改某个class内容的CSS的话，你需要在名字面前写上一个点、示例：
```
.class{
    }
```

以下为我到现在 2026/04/02 21:34~ 学到的所有可在CSS内使用的东西:

`color: red;` = 更改颜色

`left:120px;` = 像左移动120像素？

`right:5vw` = 向右间距 5%

`top:0;` = 弄到最上面

`line-heght:80px` = 文字的行距 

`background-image:url(...)` = 在...中添加背景图片

`background-color: black;` = 背景颜色

`background-repeat: no-repeat;` = 不要重复显示背景图片

`background-posotion: center;` = 将背景图片移到中间

`background-size: cover` = 背景尺寸

`text-indent: -9999px;` = 将文字推到 -9999px （使其虽然存在，但肉眼看不到，为了搜索引擎优化）

`text-decoration: none;` = 代表在...文本中，不要显示任何"文字装饰"（链接下划线）

```
a:hover{
    text-decoration:underline
} 
```
= 在鼠标在链接上时，显示下划线（underline）

`display: inline;` = 在"头部"的"li"区块中（列表），使它变为横着的，而非上下的

`margin-right: 4vw;` = 添加右边距，4vw = 视窗(屏幕？)宽度的 4%

`padding: 0;` = 边框填充？（不确定）

`margin: 0;` = 页边框填充？（不确定）

`height: 100px` = 高度

`width: 100%` = 宽度

`position: relative/absolute/fixed` = relative 是 可以直接覆盖到另外一个东西的上面，absolute是直接将元素更改？将position改为fixed，那就不会跟随网页运动了（就是会固定在上面）


`flex-direction: column;` = "CSS 中的flex -direction属性定义了弹性元素在弹性容器中的排列方向。当设置为column时，弹性元素将垂直排列，从上到下。"<br>-- [Bing Search](https://www.bing.com/search?q=flex-direction%3A+column%3B+%E6%98%AF%E4%BB%80%E4%B9%88%EF%BC%9FCSS&PC=U316&FORM=CHROMN)

<details>
<summary>图片来自：https://youtu.be/6HHN0G2cwBM?t=871</summary>
    <img width="1240" height="539" alt="image" src="https://github.com/user-attachments/assets/b3517266-a211-400c-8fe2-6f5adcba2e31" />
</details>

<details>
<summary>`/style/style.css` 的所有代码（截至2026/04/02）</summary>
    
```
/* 开始/Start */
/* 以下内容皆学自：https://youtu.be/6HHN0G2cwBM */ 
*{
    padding: 0;
    margin:0;
}
/* 
"头部"，背景颜色=黑色 
高度（height）占80px（80像素）
宽度（width）占满屏幕
position 解释： https://youtu.be/6HHN0G2cwBM?t=851
*/
header {
    background-color: black;
    height: 100px;
    width: 100%;
    position: relative;
}
/* 
h1 主标题文字颜色 = 白色
position 解释： https://youtu.be/6HHN0G2cwBM?t=851
right:5vw = 向右间距 5%
top: 0 = 弄到最上面
line-heght:80px = 文字的行距 
background-image:url(...) = 在h1中添加背景图片
background-repeat: no-repeat; = 不要重复背景图片
background-posotion: center; = 将背景图片移到中间
width: 210px; = 宽度弄到210px（210像素）
text-indent: -9999px; = 将文字推到 -9999px （使其虽然存在，但看不到，为了搜索引擎优化）
*/
h1 {
    color: white;
    position: absolute;
    left:120px;
    top:0;
    line-height: 80px;
    background-image:url(/images/web-logo.png);
    background-repeat: no-repeat;
    background-position: center;
    /* 核心修复代码（AI的帮助）：https://gemini.google.com/share/8f7d3ac049eb  */
    background-size: 80px 80px;  /* 自动缩放图片，使其完整显示在 80px 的格子内 */
    /* 或者你也可以手动指定大小，比如： */
    /* background-size: 40px 40px; */
    width: 100px;
    height: 100px;
    text-indent: -9999px;
}
/* 
text-decoration 在这边代表链接中的下划线
在第一个:
header a{
        ...
        text-decoration: none;
}
代表在a文本中，不要显示任何"文字装饰"（链接下划线）
*/
header a{
    color: white;
    text-decoration: none;
}
/* 
display: inline; = 在"头部"的"li"区块中（列表），使它变为横着的，而非上下的
margin-right: 4vw; = 添加右边距，4vw = 视窗(屏幕？)宽度的 4%
 */
header li{
    display: inline;
    margin-right: 4vw;
}
/*
position 解释： https://youtu.be/6HHN0G2cwBM?t=851
right:5vw = 向右间距 5%
top: 0 = 弄到最上面
line-heght:80px = 文字的行距
*/
header ul{
    position: absolute;
    right:5vw;
    top:0;
    line-height: 80px;
}
/*
而在下面那段代码中，在
header a:hover{
    text-decoration:underline
} 
个人解读为：
在鼠标在链接上时，显示下划线（underline）
*/
header a:hover{
    text-decoration: underline;
}
/* 在Section中的class需要以"."开始*/

/*  */
.First-about{
background-color: wheat ;
/* 在AI的帮助下，添加了背景虚化效果："linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5))," */
background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url(/images/about-background.jpg);
background-repeat: no-repeat;
background-size: cover;
background-position: center;
height: 95vh;
display: flex;
flex-direction: column;
align-items: center;
justify-content: center;
color:white;
}
/* 2026/04/02 先做到这里：https://youtu.be/6HHN0G2cwBM?t=1121 */
.First-about h2{
font-size:60px;
color: blanchedalmond;
}

.First-about p{
    color: #FEF7E6;
}

.HTML{

}

.CSS{

}

.contact{

}
/* 结束/Finish */
```

</details>

### 一个CSS示例
```
h1 {
    color: white;
    position: absolute;
    left:120px;
    top:0;
    line-height: 80px;
    background-image:url(/images/web-logo.png);
    background-repeat: no-repeat;
    background-position: center;
    /* 核心修复代码（AI的帮助）：https://gemini.google.com/share/8f7d3ac049eb  */
    background-size: 80px 80px;  /* 自动缩放图片，使其完整显示在 80px 的格子内 */
    /* 或者你也可以手动指定大小，比如： */
    /* background-size: 40px 40px; */
    width: 100px;
    height: 100px;
    text-indent: -9999px;
}
```
虽然靠了AI的帮助，但是因为视频中未讲解，下面是解释：
```
/* 
h1 主标题文字颜色 = 白色
position 解释： https://youtu.be/6HHN0G2cwBM?t=851
right:5vw = 向右间距 5%
top: 0 = 弄到最上面
line-heght:80px = 文字的行距 
background-image:url(...) = 在h1中添加背景图片
background-repeat: no-repeat; = 不要重复背景图片
background-posotion: center; = 将背景图片移到中间
width: 210px; = 宽度弄到210px（210像素）
text-indent: -9999px; = 将文字推到 -9999px （使其虽然存在，但看不到，为了搜索引擎优化）
*/
```

# 2026/04/04
## 视频中学到的东西：
今天只学了视频内的东西（https://www.youtube.com/watch?v=6HHN0G2cwBM&t=1121s 后的）：
# HTML:
`<div>` = 该标签定义 HTML 文档中的一个分隔区块或者一个区域部分。 <br> 该标签常用于组合块级元素，以便通过 CSS 来对这些元素进行格式化。 <br> <div style="text-align: right;">[菜鸟教程](https://www.runoob.com/tags/tag-div.html)</div>

`<section class="HTML" id="HTML">` = Section的补充（AI帮助），如果要在使用 `<a href="#HTML">` 那就需要在section后面加上`id="HTML"`。
# CSS：
`border: 1px solid #FEF7E6;` = 细边框

`border-radius: 5px;` = 细边框圆角效果

`justify-content: center;` = 水平对齐（上下对齐）

`align-items: center;` = 垂直对齐（左右对齐）

`line-height: 1.8em;` = 行高1.8倍

`margin-bottom: 30px;` = 标题/字的底部外边距

### 响应式设计语法：

## 在随便什么网站学到的CSS：

`text-align: <left/right/center>` = 将文字向左或向右对齐，或居中，与上下对齐

# 有些东西我直接省略了、因为不需要
### 比如说：
[HTML表单设计](https://youtu.be/6HHN0G2cwBM?t=1358)


# 目前，网站已初步建造完成。
