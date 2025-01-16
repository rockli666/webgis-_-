# webgis

* html 网页的内容
* css 网页的样式
* javascrit 网页的互动，点击按钮的反应

## 学习网站

> www.w3school.com.cn
> www.runoob.com 

## 标签

```html
<html>
     <body>里面是内容</body> 
</html>
```

* 标签
  
```html
<body></body>
```

* 元素=标签+内容
  
 ```html
  <body><h1>西南石油大学</h1></body>
  <!-- 标题和级别 -->
  <p>段落文字<\p>
  <!-- 段落文字 一个p就是一个段落-->
 ```

* 属性定义
  
```html
<h1 align='center'>西南石油大学</h1>
<!-- 定义了中间对齐的属性 -->
```

* 全局属性是所有标签都有的属性（“title”为例子）

```html
<h1 align='center' title ='请点击查看'>西南石油大学</h1>
<!-- 定义了中间对齐的属性和鼠标移动上去的显示 -->
```

* 在 HTML 中，`<p>`段落文本写在`<body>`外面是不符合标准规范的做法

* 链接

```html
<body>
    <p>
        <a href='https://swpu.edu.cn/' target='_blank'>西南石油大学<a>
    </p>
</body>
<!-- 把内容用a标签包围并用 新的页面打开 target -->
```

* 加入图片（同一个目录）

```html
<body>
     <img src='11.jpg' wight='800'/>
     <img src='图片网站链接' wight='800'/>
</body>
<!-- 自结束标签没有末尾 -->
```

* 加个输入框

```html
<body>
    <lable>姓名:</lable> <input type ='text'/>
</body>
<!-- 自结束标签没有末尾 -->
```

`<br/>`标签换行

* 按钮

```html
<body>
    <input type ='button' value='确定'/>
</body>
<!-- 自结束标签没有末尾 -->
```

* 单选框

```html
<body>
    <lable>是否本省生源</lable> <input type ='checkbox'/>
    <lable>性别：</lable>
    <lable>男</lable> <input type ='radio'name='w'/>
    <lable>女</lable> <input type ='radio'name='w'/>
    <input type ='file'/>

    
</body>
<!-- 自结束标签没有末尾 名字一样才唯一-->
```

`<hr/>`分割线

`<textarea rows="5" cols="10"></textarea>`输入框

* 作业：学生信息录入系统，用所有学过的，两段p文字

***

* 列表

`ul`无序列表

`li`成对出现，ul里面的项

```html
<ul>
<li>西南石油大学</li>
<li>四川大学</li>
</ul>
```

* 下拉列表

```html
<select>
<option>成都</option>
<option selected=selected>重庆</option>
</select>
<!-- seleced为首选项 -->
```

<select>
<option>成都</option>
<option selected=selected>重庆</option>
</select>

* 突出单独

> 用span框起来

```html
<span style='background-color:yellow;'>
    进阶
</span>
<!-- seleced为首选项 -->
```

* 网页额外信息

```html
<head>
    <title>第一个网页<title>
<head>
<!-- 网页名字 -->
```

* div
* span只能包裹文字，div任意

```html
<div>
    进阶
</div>
<!-- div可以包裹任何东西，是容器也是块元素，一般div+css -->
<!-- 好处是可以整体调成 -->
```

* 行内元素不换行（lable、input）
* 块元素自动换行（h，ul，div）
  
  `&nbsp`空格

  ***

# css定义样式

* 选择器和大括弧

```html
<head>
    <style>
        /* 样式 统一设置样式*/

        /* h2标签选择器 */
        h2{background-color:green;text-align;} 
        h2{color:red;}              
        /* 文本对齐在这里面设置 不要在body中 */

        /* id选择器 选择id等于www的元素*/
        #www{background-color:blue;}

        /* 类选择器 */
        .qq{text-align:center;}

    </style>
</head>
    <body>
        <!-- 内容 -->
        <h2 id='www' class='qq'>西南石油大学</h2>
        <!-- id是唯一的，类名是可以相同，合并一类 -->
        <h2>四川大学</h2>
    </body>
<!-- css的应用 -->
```

* 颜色背景位置

```html
<head>
    <style>
        /* rgb颜色 */
        /* red 0-255 blue 0-255 green 0-255 */
        #www{background-color:rgb(120,230,120)}
        /* 包括透明度 0-1*/
            #www{background-color:rgba(120,230,120,0.5)}

        /* 设置背景图像 铺满*/
        body{background-image:url('1.jpg')}
        
        /* 设置背景图像 一张*/
        body{background-image:url('1.jpg');background-repeat:no-repeat}

          /* 设置背景图像 位置*/
        body{background-image:url('1.jpg');
        background-repeat:no-repeat;
        background-position:right}

          /* 设置背景图像 位置*/
        body{background-image:url('1.jpg');
        background-repeat:no-repeat;
        background-position:10 20}
        
          /* 设置背景图像 位置*/
        body{background-image:url('1.jpg');
        background-repeat:repeat-x;
        background-position:right}
    </style>
</head>
    <body>
        <h2 id='www' class='qq'>西南石油大学</h2>
        <h2>四川大学</h2>
    </body>
<!-- css的应用 -->
```

* 边框

```html
<head>
    <style>
       h2{border-style:dashed;border-color:blue;border-width:8px;width:145}
       /* 可以合起来写 */
       h2{border: 6px red dotted;width:145px;height:145px}
    </style>
</head>
    <body>
        <!-- 内容 -->
        <h2 id='www' class='qq'>西南石油大学</h2>
        <!-- id是唯一的，类名是可以相同，合并一类 -->
        <h2>四川大学</h2>
    </body>
<!-- css的应用 -->
```

* 外边距：这个元素距离旁边元素或者父元素的距离

```html
<head>
    <style>
    #d1{border:6px blue dotted;width:400px;height:300px;}
    #d2{border:2px red solid;width:200px;height:100px;
    margin-left:30px;
    margin-top:30px;}
    #b1{
        margin-left:80px;
    }
    </style>
</head>
    <body>
        <div id="d1">
            <div id="d2">
                <input type='button' value="确定"/>
                <input type='button' value="取消" id="b1"/>
            </div>
        </div>
    </body>
<!-- css的应用 -->
```

***

* 回顾
  
```html
<head>
    <style>
        h2{color:red;text-align:cente;border:2px blue solid;}

        #d1{border:6px blue dotted;width:400px;height:300px;}
    
        #d2{border:2px red solid;width:200px;height:100px;
        margin-left:30px;
        margin-top:30px;}
   
    </style>
</head>
    <body>
     <h2>西南石油大学</h2>
        <div id="d1"><input type='button' value="确定"/></div>
        <div id="d2"><input type='button' value="取消"/></div>
        <div>
    </body>
    <!-- body就是整个窗口，也具有边框 -->
<!-- css的应用 -->
```

* 内边距（一个并不可用的空间）与首行缩进、字体

```html
<head>
    <style>
        h2{color:red;text-align:cente;border:2px blue solid;}

        #d1{border:6px blue dotted;width:400px;height:300px;padding:50 }
    /* 用padding指定内边距 */
    /* padding-left:50 距离左边50*/
        #d2{border:2px red solid;width:200px;height:100px;
        margin-left:30px;
        margin-top:30px;
        overflow:auto}
        /* 处理溢出，超出的地方不显示 或者拉动*/
        p{text-indent:30px;font-weight:700}
   /* text-indent 首行缩进 加粗*/
   span{font-family:'Times New Roman'，'xx';font-size:64px}
   /* 字体的定义 */   /*多个字体是从第一个开始找直到找到电脑上有的字体为止*/
   /* 加粗 400是正常粗细 700是加粗 只能选择加粗或者不加粗 */
   </style>
</head>
    <body>
     <h2>西南石油大学</h2>
        <div id="d1"><input type='button' value="确定"/></div>
        <div id="d2"><input type='button' value="取消"/></div>
        <p>西南石油大学创建于1958年，原名四川石油学院，校址位于四川省南充市，1970年更名为西南石油学院，
            2002年学校主体搬迁到成都市新都区。2004年原四川省政法管理干部学院并入。
            2005年学校更名为西南石油大学。2013年入选“国家中西部高校基础能力建设工程”。2017年入选国家首批世界一流学科建设高校，2022年入选国家新一轮“双一流”建设高校。</p>
        <span>G</span>
    </body>
    <!-- 里面有一个内环区域变成不可用 -->
<!-- css的应用 -->
```

***

* 学习布局

* 绝对定位：相对于第一个设置了postion属性的父辈定位
* 相对定位：该元素相对于自己原来位置的定位
* 文档流：从左到右从上到下的排列
* 固定定位：相对于浏览器的定位

```html
<html>

<head>
<style>
        #d1{width:800px;height:400px;border:2px red solid;position:relative;}
        /* 父辈必须要设置position属性 */
        #d2{width:400px;height:300px;border:2px green solid;
        position:absolute;top:40px;left:60px}
        #d3{width:200px;height:100px;border:2px blue solid;
        position:relative;top:30px;left:70px}
          /* 相对定位 */
        #d4{width:100px;height:50px;border:2px yellow solid;
        position:fixed;top:64px;right:40px}
        /* 固定定位 空间也会跑掉 固定在浏览器某一位置 滑动时候位置不变*/
        #d5{width:100px;height:50px;border:2px pink solid;
        ;top:64px;right:40px;float:right}
        /* 浮动 空间会被挤占 右浮动：一直往右边飘，
        直到碰到边界或者另外一个右浮动元素为止*/

</style>
</head>

<body>
        <div id="d1">
                <div id="d2">
                </div>
                <div id="d3">
                </div>
                <div id="d4">
                </div>
                <div id="d5">
                </div>
        </div>
</body>
<!-- 绝对定位 和 margin有点类似 绝对定位会脱离文档流，其他元素会顺势挤占空间 -->
<!-- 相对定位不会挤占空间 蓝框并不会上去，有隐形空间，位置还在那里-->
</html>
```

* 浮动

```html
<html>
<head>
<style>
 		ul{list-style-type:none;padding:0}
        /* li浮动 没空间了 */
 		li{border:1px black solid;width:80px;float:left;}
        
    /* margin: 0 atuo 自动左右居中*/
</style>
</head>

<body>
        <div>
                <ul>
				<li>校情总览</li>
				<li>机构设置</li>ne
				<li>师资队伍</li>
				<li>教育教学</li>
				</ul> 
        </div>
</body>
<!-- 浮动 -->
 <!-- hight和line-hight一样自动据中 -->
</html>
```

* 变色
  
```html
li:hover{background:black;line-height:45px;}
```

* 点上去有鼠标

```html
li:{cursor:pointer}
```

***

```html
<html>
	<head>
	<style>
        #d1{width:100%;height:100%;background:red
        margin:0 auto;position:relative}
        /* 左右居中 和父亲宽度是百分百占比 绝对定位*/
        #d2{width:400px;height:60px;background:blue;position:absolute;top:20px;left:30px}
        /* 上下左右居中 绝对定位 top:0px;left:0px;right:0px;bottom:0px;margin:auto; */

	</style>
	</head>

	<body>
        <div id='d1'>
            <div id="d2">
                <input type="text">
            </div>
        </div>
    </body>
</html>
<!--  -->
```

* display:none 不显示不存在，空间也会被挤掉
* display:block 行内元素变成块元素
* display:inline 变成行内元素
* display:inline-block 行内元素，并且可以改变宽高宽度
* border-radius:18px 有圆角

* 选择器
  
 ``` html
<html>
	<head>
	<style>
      /*.d1 .p1{color:red}*/
      /*只有第一个北京红色*/

      /*.d1 .p1+p+p+p{color:red}*/
      /*只有第一个上海红色*/

      /*.p1+p+p+p{color:red}*/
      /*所有上海红色*/

      /*.p1+p+p+p:not(.d1 .p1+p+p+p){color:red;}*/

      /*.d1+div .p1+p+p+p{color:red;}*/
      /*只有最后一个上海红色*/

       div:last-child p:last-child{color:red;}   

       :nth-child(3){background-color:blue;}
       /*选中第几个儿子*/
	</style>
	</head>

	<body>
        <div class='d1'>
            <p class="p1">北京</p>
            <p>沈阳</p>
            <p>北京</p>
            <p>上海</p>  
        </div>
        <div>
            <p class="p1">北京</p>
            <p>沈阳</p>
            <p>北京</p>
            <p>上海</p>  
        </div>
    </body>

    
</html>
```

* 左右布局可以设置左右浮动
* 居中的方法

```html
<!-- 1.文本 -->
 左右居中text-align
 上下居中height=line-height

<!-- div -->
左右居中 margin 0 auto
上下左右居中 父亲设置postion儿子绝对定位，上下左右0 margin：auto

```


***

# javascript

* 语句推荐写在 body 结束语句之前
* 语法和c#有一点类似
  
```javascript
    <!-- 变量类型可以直接改变，实时 -->
    var c=0;c=1.2;c="ddd"
    c=[2,3,4,5];
    c=['micro','google']

    //window.alert('请确认收到货再收货')
    // 弹窗
    //window.open('https://www.swpu.edu.cn/')
    // 打开新的网址
    //screen.width
    //location.href='https://www.swpu.edu.cn/'
    //window.alert(geolocation);

    var d1=document.getElementById('d1');
    // 此时d1为element对象
    alert(d1.tagName);
    // 返回标签属性
    //innerHTML 开始标签和结束标签之间的内容 非常重要
```

***

```html
<html>

<head>
</head>

<body>

<div id="d1">
	<p>666</p>
    <p>南京大学</p>
	<p>四川大学</p>
</div>

<script>
  var d1=document.getElementById('d1');
  var d2=d1.lastElementChild.innerHTML;
  alert(d2);
  //获取四川大学字符的思路
   var d2=d1.lastElementChild.previousElementSibling.innerHTML;
    //获取南京大学的思路    
      alert(d1.childNodes.length());
    //如果没有elment的方法获取所有的儿子  包括空格等 返回7

    //事件
    <input type="button" value="OK" onclick='alert("hello")'>

    	<p>666</p>
	<p>南京大学</p>
	<p>四川大学</p>
	<input type="text" id="t1"/>
	<input type="button" value="OK" onclick='alert(document.getElementById("t1").value);        '/>.
</script>
</body>

</html>
```

* 函数表达

```javascript
<div id="d1">
	<p>666</p>
	<p>南京大学</p>
	<p>四川大学</p>
	<input type="text" id="t1"/>
	<input type="button" value="OK" onclick='FF()'/>.
</div>

<script>
  function FF()
  {
  	alert(document.getElementById("t1").value)
  }
 </script>
```

* 全部写在< script >里面

```javascript
  //匿名函数
  w.onclick=function(){
     alert(document.getElementById("t1").value)
  };
  w.onmouseover=function(){
  	document.getElementById("d1").style.backgroundColor="red";
  };
    w.onmouseout=function(){
  	document.getElementById("d1").style.backgroundColor="white";
  };
//练习
    var w=document.getElementById("b1");
  w.ondblclick=function(){
     var a=document.getElementById("d1");
     a.lastElementChild.previousElementSibling.previousElementSibling.previousElementSibling.innerHTML ="东南大学";
  };
  w.onmouseover=function(){
  	  document.getElementById("t1").style.border = "1px  red solid";
  };
   w.onmouseout=function(){
  	  document.getElementById("t1").style.border = "1px blue solid ";
  };
  //获取字符串
   w.onclick=function(){
     var a=document.getElementById("t1").value;
     var a1=a.substring(0,3);
     var a2=a.charAt(0);
     var a3=a.charAt(a.length-1);
     alert(a3);    
     //isNaN(5)判断是不是数字 false是数字   true是非数字

    t1.oninput=function(){
     var a=document.getElementById("d1").firstElementChild.innerHTML=t1.value;  
  };
```

***

```javascript
<html>
<head>
    
</head>
<body>
    <input type="button" id="b1"/>
       <input type="button" id="b1" value="增加"/>
    <div id="d1">
        <input type="text" id="t1"/>
    </div>
<script>

    var btn=document.getElementById('b1');
    var d1=document.getElementById("d1");
    <!-- 最好不要直接b1.xxx -->
    btn.onclick=function(){
        //输出到控制台
        console.console.log();
        
        //keyup 键盘抬起
        //keydown 键盘按下

        //event事件
        //we随便命名是系统给我们的参数
        //比如和keyup相关的kyboardevent
        //target表明是哪个控件触发的事件
        btn.onclick=function(e){
        //e.preventDefault();阻止默认事件
        
        window.setTimeout(function(){
            t1.value="西南石油大学";
        }, 2000);
        //定时器2s
        //creatElement();
        var n = document.creatElement("input");
        n.type="text";
        d1.appendChild(n);
    }


</script>
</body>
</html>
```

***

