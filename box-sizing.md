# box-sizing 

box-sizing 属性用于更改用于计算元素宽度和高度的默认的 CSS 盒子模型。

### 值

##### content-box
默认值，标准盒子模型。 width 与 height 只包括内容的宽和高， 不包括边框（border），内边距（padding），外边距（margin）

###### 尺寸计算公式：
```
width = 内容的宽度

height = 内容的高度。
```

宽度和高度都不包含内容的边框（border）和内边距（padding）。

##### border-box（IE的怪异盒模型）
 width 和 height 属性包括内容，内边距和边框，但不包括外边距。

###### 尺寸计算公式：
```
width = border + padding + 内容的width，

height = border + padding + 内容的height。
```

### 兼容性：
IE8及以上版本支持该属性

### 应用场景：三栏布局
```
//html
<div class="left"></div>
<div class="cent"></div>
<div class="right"></div>


//css
div{
    height:500px;
    float:left;
}
div.left{
    width:25%;
    background:red;
}
div.cent{
    width:50%;
    background:green;
    padding:0 20px;  // padding或border 会使内容溢出
    box-sizing:border-box; //解决padding或border使内容溢出
}
div.right{
    width:25%;
    background:blue;
}
```