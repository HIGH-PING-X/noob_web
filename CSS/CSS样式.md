# CSS

Cascading Style Sheet（层叠样式表）

- CSS导入方式：


```html
<!-- 行内样式仅对当前标签生效 -->
<div style="border: 1px solid black;width: 100px; height: 100px;">&nbsp;</div>


<!-- 内部样式：内部样式仅对当前页面生效 -->
<head>
   <style type="text/css">
   .one {
         border: 1px solid black;
         width: 100px;
         height: 100px;
         background-color: lightgreen;
         margin-top: 5px;
   }
   </style>
</head>


<!-- 外部样式：需要引入外部的CSS样式文件 -->
<head>
   <link rel="stylesheet" type="text/css" href="/static/css/example.css" />
</head>
```

- CSS选择器：

1.三种基本选择器：

```html
    <style>
            /* 标签选择器 */
            p {
                color: blue;
                font-weight: bold;
            }
            
           /* id选择器 */
            #noob00 {
                font-size: 20px;
                background-color: aqua;
            }
            
            /* 类选择器 */
            .noob01 {
                border: 1px solid black;
                width: 100px;
                height: 100px;
                background-color: lightgreen;
                margin-top: 5px;
        }
    </style>
    <body>
        <p>标签选择器的样式</p>
        <div id="noob00">Hello,div01......</div>
        <div class="noob01">类选择器的样式</div>
    </body>
```

2.层次选择器：

```html
<style>
    /* 后代选择器:在某个元素后面 */
    	body p{
    		background:red;
    }
    
   	/* 子选择器：后面一个 */
    	body>p{
        	background:red;
    }
    
    /* 相邻兄弟选择器：同辈 */
    	.noob + p{
        	background:red;
    }
    
    /* 通用选择器 */
    	.noob +p{
        	background:red;
    }
</style>
<body>   
    <p>p0</p>
    <p class="noob">p1</p>
    <p>p2</p>
    <p>p3</p>
    <ul>
        <li>
        	<p>p4</p>
        </li>
        <li>
        	<p>p5</p>
        </li>
         <li>
        	<p>p6</p>
        </li>
    </ul>
</body>
```

3.结构伪类选择器：

```html
<style>
/* ul的第一个子元素 */
ul li:first-child{
	background:red;
}

/* ul的最后一个子元素 */
ul li:last-child{
	background:red;
}

/* 选中p1，定位到夫元素，选择当前的第一个元素/选择当前p元素的父级元素，选中父级元素的第一个，并且是当前元素才生效。顺序 */
p:nth-child(2){
	background:red;
}

/* 选中夫元素下的p元素的第二个，类型 */
p:nth-of-type(1){
	background:red;
}
    
/* 变色 */
/* 鼠标悬浮变色 */
noob:hover{
	coloer:red;
}
/* 鼠标按住变色 */
noob:active{
    coloer:red;    
}
</style>
```

4.属性选择器：

``` vim
属性名 属性名 = 属性值（正则）
= 绝对等于
*= 包含这个元素
^= 以这个元素开头
$= 以这个元素结尾
```

- 字体样式：


```html
<style>
    noob{
		font-family:字体;
        font-size:字体大小;
        font-weight:字体粗细;
        coloer:颜色;
        text-shadow:颜色 x轴 y轴 大小;(阴影)
    }
</style>
```

- 文本样式：


```html
<style>
    noob{
        /*
        RGB:0~F
		RGBA A(透明度):0~1
        */
        coloer:rgb(0,0,0);
        coloer:rgba(0,0,0,0);
        text-align:剧中,靠左,靠右;
        text-indent:首行缩进em;
        background:背景颜色;
        height:行高;
        line-height:块高;
        text-decoration:underline(下划线) line-through(中划线) overline(上划线) none(去下划线);
        vertical-align:middle(图片文本水平对齐);
    }
</style>
```

- 列表样式：

```html
<style>
    noob{
        list-style:none(去圆点) circle(空心圆) decimal(数字) square(正方形);
        text-indent:首行缩进em;
        width:; 
    }
</style>
```

- 背景样式：

```html
<style>
    noob{
        height:;
        weight:;
        border:边框粗细 边框线条 颜色;
        background-image:url("图片地址");
        background-repeat:repeat-x(水平平铺) repeat-y(垂直平铺) no-repeat(不平铺);
        bckeground-position:位置坐标;(定位背景图片颜色)
        background-attachment:scroll(固定图片会随页面滚动) fixed(固定图片不会随页面滚动);
        background-image: linear-gradient(颜色渐变方向,颜色,颜色,……);
    }
</style>
```

- 盒子模型：

```html
<style>
    /* 内外边距设为0 */
    body{
        margin:0;
        padding:0;
    }
    
    noob{
        border:边框粗细 边框线条 颜色;
        margin:上 左 下 右;
        padding:上 左 下 右;
        margin:0 auto;(居中对齐)(前提是一个快元素)
        border-radius:;(圆角边框)(圆角=边框时为圆)
        box-shadow:颜色 x轴 y轴 大小;(阴影)
    }
</style>
```

- 浮动：

```html
<style>
    noob{
        disply:block inline inline-block(是块元素但可以在一行);
        float:left right;
        clear:left right both none;(去除浮动)
        overfloat:hidden(自动隐藏) auto;
    }
</style>
```

- 定位：

```html
<style>
    noob{
        position:relative(相对定位) absolute(绝对定位) fixed(固定定位);
        top:;
        bottom:;
        left:;
        right:;
        z-index:数字越大层级越高;(图层)
        opacity:0~1;(透明度)
    }
</style>
```

