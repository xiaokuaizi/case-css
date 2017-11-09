### 未知宽高的模块水平垂直居中

[在线预览效果](https://xiaokuaizi.github.io/case-css/center/center.html)

[domo源码地址](https://github.com/xiaokuaizi/case-css/blob/master/%E6%B0%B4%E5%B9%B3%E7%AB%96%E7%9B%B4%E5%B1%85%E4%B8%AD/center.html)

#### 方案1：flex
```
display: flex; /* 使用flex布局 */
justify-content: center; /* 水平居中 */
align-items: center; /* 竖直居中 */
```

#### 方案2：translate+position

```
/* 父元素相对定位 */
position: relative;

/* 子元素 */
position: absolute;  /* 相对父元素绝对定位 */
left:50%; /* 相对父元素横向移动父元素50% */
top:50%; /* 相对父元素纵向移动父元素50% */
transform:translate(-50%,-50%); /* 相对自己横纵向移动自己的50% */

```

#### 方案3： vertical-align

```
/* 父元素 */
text-align: center； /* 子元素为行内元素时可以水平居中 */

/* 子元素 */
vertical-align: middle; /* 行内元素的基线相对于该元素所在行的基线的垂直对齐 */
display: inline-block;

/* 父元素的after */
vertical-align: middle; /* 行内元素的基线相对于该元素所在行的基线的垂直对齐 */
display: inline-block;
content: '';
height:100%

```