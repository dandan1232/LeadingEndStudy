# Emmet

## 1.Emmet是什么

###### Emmet是⼀个前端开发插件，可以快速⽣成html代码，提升开发效率. VScode默认⽀持Emmet

## 2.快速⽣成html结构⽂档

###### 在新建的html中输⼊! 或者html，⽣成html 5结构⽂档：

####  ！或者html:5

```html
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <title>Document</title>
</head>
<body>
</body>
</html>
```

###### html4结构⽂档

#### html:tx

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0
Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-
transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en">
<head>
 <meta http-equiv="Content-Type"
content="text/html;charset=UTF-8">
 <title>Document</title>
</head>
<body>
</body>
</html>
```

## 3.生成带id的标签

#### 元素名 #id名

###### 如

```html
div#box
```

###### 按tab或回车

```html
<div id="box"></div>
```

## 4.⽣成带class的标签

#### div.container

```html
<div class="container"></div>
```

###### 混合

#### div#header+div.main+div#footer.classnam1.classname2

```html
<div id="header"></div>
<div class="main"></div>
<div id="footer" class="classnam1 classname2"></div>
```

## 5.⽣成⼦代结点：>

#### div.header>ul.nav>li.nav-item

```html
<div class="header">
 <ul class="nav">
 <li class="nav-item"></li>
 </ul>
</div>
```

## 6. ⽣成兄弟结点: +

#### div+p+bq

```html
<div></div>
<p></p>
<blockquote></blockquote>
```

## 7.⽣成⽗代结点：^

#### div>p>h1^h2

```html
<div>
 <p>
 <h1></h1>
 </p>
 <h2></h2>
</div>
```

## 8.重复元素：

###### 任何元素后⾯加上*n就会被重复n次，⽐如⽣成⼀个包含4个li的ul：

#### ul>li.item*4

```html
<ul>
 <li class="item"></li>
 <li class="item"></li>
 <li class="item"></li>
 <li class="item"></li>
</ul>
```

## 9.⽣成分组：()

###### ⽤括号进⾏分组，这样可以更加明确要⽣成的结构，特别是层次关系，示 例：

#### div>(header>ul>(li>a)*2)+footer>p

```html
<div>
 <header>
 <ul>
 <li><a href=""></a></li>
 <li><a href=""></a></li>
 </ul>
 </header>
 <footer>
 <p></p>
 </footer>
</div>
```

## 10. 设置属性:[]

###### 属性写在[]内，属性当中采⽤等号赋值，多个属性⽤空格隔开. 示例

#### a[href=”https://www.baidu.com” title=”百度⼀下，你就知道”]

```html
<a href="”https://www.baidu.com”" title="”百度⼀下，你就知
道”"></a>
```

## 11.对⽣成内容编号:$

###### 可以使⽤美元符 $对项⽬编号，示例

#### ul>li#item$*5

```html
<ul>
 <li id="item1"></li>
 <li id="item2"></li>
 <li id="item3"></li>
 <li id="item4"></li>
 <li id="item5"></li>
</ul>
```

###### 上⾯的例⼦是从⼩到⼤，从⼤到⼩可以在$后加@－：

#### ul>li#item$@-*5

```html
<ul>
 <li id="item5"></li>
 <li id="item4"></li>
 <li id="item3"></li>
 <li id="item2"></li>
 <li id="item1"></li>
</ul>
```

###### 从指定序号3开始 ，⽣成5个

```html
<ul>
 <li class="item3"></li>
 <li class="item4"></li>
 <li class="item5"></li>
 <li class="item6"></li>
 <li class="item7"></li>
</ul>
```

## 12.⽣成⽂本内容:{}

###### 想要在⽣成的元素内插⼊内容，可以使⽤{},把⽂本内容放进去即可。示 例：

```html
<ul id="id">
 <li class="classname">⽣成⽂本内容</li>
 <li class="classname">⽣成⽂本内容</li>
 <li class="classname">⽣成⽂本内容</li>
 <li class="classname">⽣成⽂本内容</li>
 <li class="classname">⽣成⽂本内容</li>
</ul>
```

## 13.⽣成随机⽂本

###### emmet的lorem将⽣成⼀段随机⽂本。示例：

#### p.content>lorem

```html
<p class="content">
 Lorem ipsum, dolor sit amet consectetur adipisicing
elit. Commodi dicta, consequatur quod est magni sequi ex
voluptatum ea. Illo, esse
 eaque libero magni minus optio nihil eius unde velit
vitae.
</p>
```

#### ⼩结：上述内容总结了emmet⽣成html⽂档结构、类、id、属性、 ⽂本内容、⽗级节点、兄弟阶段、⼦节点、序号的⽅法。正确安装 emmet插件，注意中英⽂切换和空格，熟练掌握以上命令可以快速 提⾼开发效率

