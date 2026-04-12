# 2026/04/12 13:24~ 以下内容由Gemini AI优化

# Learning Html, JavaScript, CSS

学习HTML, JavaScript + CSS中，于2026年4月2日开始

目前仅仅使用该学习网站： [Developer.Mozilla.org](https://developer.mozilla.org/zh-CN/docs/Learn_web_development/Getting_started/Your_first_website/Creating_the_content) 与该视频： [YouTube.com](https://youtu.be/6HHN0G2cwBM)

目前仅使用该工具：[VsCode.Dev](https://vscode.dev)

目前计划为：
~~目标为制作一个画画网站，可以画画并保存~~ 将我学到的东西弄成一个网站

# Index (目录):

[2026/04/02 21:34](#20260402-2134)

[2026/04/04](#20260404)

# **2026/04/02 21:34**

> **进度记录：** 先做到这里：[https://youtu.be/6HHN0G2cwBM?t=1121](https://youtu.be/6HHN0G2cwBM?t=1121)

### TODO:

虽然说已经学了挺多了，但有些东西还需要稍加稳固一下，或者也许在再看Mozilla.org的教程时会再次学到？
明天要把视频看完，并且再弄个总结。

## **到现在学到的东西**：

### 📄 HTML 基础标签 (按功能分类)

**1. 网页骨架与头部设置**

  * `<!DOCTYPE html>` = 声明文档类型，告诉浏览器这是一个 HTML5 网页。
  * `<html lang= "zh"></html>` = 设置 HTML 语言为中文。
  * `<head></head>` = 头部文件（里面的内容不会在网站页面内直接显示，用于存放配置）。
  * `<meta name="viewport" content="width=device-width" />` = 视口设置，用于响应式网页设计，确保网页在手机等移动设备上也能按照正确的比例显示。
  * `<title></title>` = 网页的标题（显示在浏览器标签页上）。
  * `<link rel="stylesheet" href="/style/style.css">` = 从 `/style/style.css` 导入 CSS 文件（*注：修正了原笔记中 href 漏掉的等号 `=`*）。

**2. 网页结构与语义化区块**

  * `<body></body>` = 网页中所有的主要可见内容都放在这里。
  * `<header></header>` = 头部内容 / 页眉。
  * `<nav></nav>` = 网页中的导航栏。
  * `<main></main>` = 网页的主要核心内容。
  * `<section class=""></section>` = "HTML `<section>` 元素表示 HTML 文档中一个通用独立章节，它没有更具体的语义元素来表示。一般来说会包含一个标题。" -- [Mozilla.org](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Reference/Elements/section)
  * `<footer>Copytight © 2026 1224HuangJin 版权所有</footer>` = 最下面的文字 / 页脚，通常用于显示版权信息等。。。

**3. 文本与内容排版**

  * `<h1> -> <h6>` = 标题，子标题等（数字越小字越大）。
  * `<p></p>` = 普通文字段落。
  * `<br>` = 在文字/内容中强制换行。
  * `<strong></strong>` = 加粗文字，类似 Markdown 的 `**<文字>**`。
  * `<blockquote cite="link?">"君子藏器而身，<br>待时而动。"</blockquote>` = 引用内容区块。`cite="link"` 属性用于在代码层面标明引用的来源链接（通常不会直接显示给用户，给搜索引擎或阅读器看的）。

**4. 链接、图片与列表**

  * `<a href="link">文字</a>` = 在某文字中插入超链接。
  * `<img src="图片链接" width="宽度" height="高度" alt="Alt 文字">` = 插入图片（`alt` 是图片加载失败时显示的替代文字）。
  * `<ol>     <li>1</li>  <li>2</li>   </ol>` = 有数字顺序的列表（`ol` = ordered list + `li` = list item）。
  * `<ul>     <li>1</li>  <li>2</li>   </ul>` = 无数字的黑点列表（`ul` = unordered list + `li` = list item）。

### 🎨 CSS 样式与排版

（以下内容基本皆来自： [PAPAYA 电脑教室](https://www.youtube.com/watch?v=6HHN0G2cwBM) 的视频内）

#### 🔹 基础语法与选择器

选定某个元素，比如说：

```css
a {
    /* 样式属性写在这里 */
}
```

（其实也可以弄`<a></a>`，`<p></p>`，`<h1></h1>`，`<header>`等等。。）然后再内部添加内容。

**示例：**

```css
header {
    background-color: black;
    height: 100px;
    width: 100%;
    position: relative;
}
```

**注意：** 如果要更改某个 `class` 内容的 CSS 的话，你需要在名字面前写上一个点（`.`）、示例：

```css
.class {
    /* 样式 */
}
```

#### 🔹 样式属性字典 (截至 2026/04/02)

**1. 尺寸与盒模型 (Box Model)**

  * `height: 100px;` = 元素的高度。
  * `width: 100%;` = 元素的宽度（占满父元素的 100%）。
  * `padding: 0;` = **内边距**（元素内部的内容与边框之间的距离）。
  * `margin: 0;` = **外边距**（元素与其他元素之间的外部距离）。
  * `margin-right: 4vw;` = 添加右边距，`4vw` = 视窗(屏幕)宽度的 4%。

**2. 定位与排版 (Positioning & Layout)**

  * `position: relative/absolute/fixed;`
      * `relative`: 相对定位（可以通过 top/left 移动，且可以直接覆盖到另外一个东西的上面，保留原来空间）。
      * `absolute`: 绝对定位（直接脱离原本位置，根据最近的父元素定位）。
      * `fixed`: 固定定位（将 position 改为 fixed，那就不会跟随网页运动了，就是会固定在屏幕上）。
  * `left: 120px;` = 距离左侧 120 像素。
  * `right: 5vw;` = 距离右侧 5%（视窗宽度）。
  * `top: 0;` = 贴紧最上面。
  * `display: inline;` = 将元素变为行内元素（例如在"头部"的"li"区块列表中，使它变为横排的，而非上下的）。
  * `flex-direction: column;` = "CSS 中的 flex-direction 属性定义了弹性元素在弹性容器中的排列方向。当设置为 column 时，弹性元素将垂直排列，从上到下。"<br>-- [Bing Search](https://www.bing.com/search?q=flex-direction%3A+column%3B+%E6%98%AF%E4%BB%80%E4%B9%88%EF%BC%9FCSS&PC=U316&FORM=CHROMN)

**3. 背景设置 (Background)**

  * `background-color: black;` = 纯色背景颜色。
  * `background-image: url(...);` = 在...中添加背景图片。
  * `background-repeat: no-repeat;` = 不要重复平铺显示背景图片。
  * `background-position: center;` = 将背景图片对齐到正中间（*注：修正了原拼写*）。
  * `background-size: cover;` = 背景尺寸自适应，使其覆盖整个元素。

**4. 文本与颜色 (Text & Colors)**

  * `color: red;` = 更改文字颜色。
  * `line-height: 80px;` = 文字的行高/行距（*注：修正了原拼写*）。
  * `text-indent: -9999px;` = 首行缩进将文字推到 -9999px（使其虽然存在，但肉眼看不到，为了保留结构给搜索引擎优化 SEO）。
  * `text-decoration: none;` = 代表在文本中，不要显示任何"文字装饰"（比如去掉链接自带的下划线）。

**5. 伪类交互 (Pseudo-classes)**

```css
a:hover {
    text-decoration: underline;
} 
```

\= 意思是：在鼠标悬停在链接上方时，显示下划线（underline）。

-----

<details>
<summary>🖼️ 视频参考图片来自：[https://youtu.be/6HHN0G2cwBM?t=871](https://youtu.be/6HHN0G2cwBM?t=871)</summary>
<img width="1240" height="539" alt="image" src="https://github.com/user-attachments/assets/b3517266-a211-400c-8fe2-6f5adcba2e31">
</details>

<details>
<summary>📂 `/style/style.css` 的所有代码（截至2026/04/02）</summary>

```css
/* 开始/Start */
/* 以下内容皆学自：https://youtu.be/6HHN0G2cwBM */ 
*{
    padding: 0;
    margin:0;
}
/* "头部"，背景颜色=黑色 
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
/* h1 主标题文字颜色 = 白色
position 解释： https://youtu.be/6HHN0G2cwBM?t=851
right:5vw = 向右间距 5%
top: 0 = 弄到最上面
line-height: 80px; = 文字的行高 
background-image:url(...) = 在h1中添加背景图片
background-repeat: no-repeat; = 不要重复背景图片
background-position: center; = 将背景图片移到中间
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
/* text-decoration 在这边代表链接中的下划线
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
/* display: inline; = 在"头部"的"li"区块中（列表），使它变为横着的，而非上下的
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
line-height: 80px; = 文字的行距
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

/* */
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

-----

# **2026/04/04**

## 视频中学到的东西：

今天只学了视频内的东西（[https://www.youtube.com/watch?v=6HHN0G2cwBM\&t=1121s](https://www.youtube.com/watch?v=6HHN0G2cwBM&t=1121s) 后的）：

### HTML 补充:

  * `<div>` = 该标签定义 HTML 文档中的一个分隔区块或者一个区域部分。<br> 该标签常用于组合块级元素，以便通过 CSS 来对这些元素进行格式化。<br> \<div style="text-align: right;"\>[菜鸟教程](https://www.runoob.com/tags/tag-div.html)\</div\>
  * `<section class="HTML" id="HTML">` = Section 的补充（AI帮助）。如果要在网页内制作跳转锚点链接（如使用 `<a href="#HTML">`），那就需要在相应的 section 后面加上唯一的 `id="HTML"`。

### CSS 补充：

  * `border: 1px solid #FEF7E6;` = 添加一条细实线边框。
  * `border-radius: 5px;` = 给边框或背景添加圆角效果。
  * `justify-content: center;` = （Flex 弹性布局中）决定主轴的对齐方式。如果是横向排版，这是指**左右水平居中**。
  * `align-items: center;` = （Flex 弹性布局中）决定交叉轴的对齐方式。如果是横向排版，这是指**上下垂直对齐/居中**。
  * `line-height: 1.8em;` = 动态行高设置，`1.8em` 表示行高是当前文字大小的 1.8 倍。
  * `margin-bottom: 30px;` = 元素的底部外边距（与下方元素拉开 30 像素的距离）。

-----

### 📱 响应式设计语法 (Media Queries)：

这部分代码用于让网站在不同的设备（如手机）上改变排版：

```css
/* 当屏幕宽度小于或等于 768px 时执行以下样式（通常是手机或小型平板） */
@media screen and (max-width: 768px) {
    
    /* 隐藏页眉里的无序列表（通常是隐藏桌面端导航栏） */
    header ul {
        display: none;
    }

    /* 将页眉的标题定位到水平正中间 */
    header h1 {
        left: 50%; /* 移动到距离左侧 50% 的位置 */
        transform: translateX(-50%); /* 向左回弹自身宽度的 50%，实现完美居中 */
    }

    /* 调整关于部分的一级标题字号，防止在小屏上显得太大 */
    .First-about h2 {
        font-size: 40px;
    }

    /* 针对移动端菜单按钮（汉堡菜单）的样式设置 */
    .menu {
        display: block;             /* 显示该元素（之前可能是隐藏的） */
        background-color: transparent; /* 背景透明 */
        color: white;               /* 图标或文字颜色为白色 */
        font-size: 35px;            /* 设置图标大小 */
        position: absolute;         /* 绝对定位，方便调整位置 */
        top: 15px;                  /* 距离顶部 15 像素 */
        left: 20px;                 /* 距离左侧 20 像素 */
        border: none;               /* 去掉边框 */
        cursor: pointer;            /* 鼠标悬停时显示小手图标 */
    }
}
```

## 在随便什么网站学到的CSS：

  * `text-align: <left/right/center>;` = 文本对齐方式，将段落文字向左对齐、向右对齐、或居中对齐。

-----

# 有些东西我直接省略了、因为不需要

### 比如说：

  * [HTML表单设计](https://youtu.be/6HHN0G2cwBM?t=1358)

<br>

# 🎉 目前，网站已初步建造完成。
