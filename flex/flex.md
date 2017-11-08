# Flex 布局
任何一个容器（包括行内元素）都可以指定为 Flex 布局

## 效果demo



## 容器属性
以下6个属性设置在容器上：
- flex-direction
- flex-wrap
- flex-flow
- justify-content
- align-items
- align-content

#### flex-direction（主轴的方向-即项目的排列方向）
```
row（默认值）：主轴为水平方向，起点在左端。
row-reverse：主轴为水平方向，起点在右端。
column：主轴为垂直方向，起点在上沿。
column-reverse：主轴为垂直方向，起点在下沿。
```
#### flex-wrap（一条轴线排不下，如何换行）
```
nowrap:默认，不换行。
wrap：换行，第一行在上方
wrap-reverse：换行，第一行在下方
```
#### flex-flow（flex-direction属性和flex-wrap属性的简写形式）
```
flex-direction 
flex-wrap
```
####  justify-content（项目在主轴上的对齐方式）
```
flex-start（默认值）：左对齐
flex-end：右对齐
center： 居中
space-between：两端对齐，项目之间的间隔都相等。
space-around：每个项目两侧的间隔相等。所以，项目之间的间隔比项目与边框的间隔大一倍。
```

#### align-items(项目在交叉轴上如何对齐)
```
flex-start：交叉轴的起点对齐。
flex-end：交叉轴的终点对齐。
center：交叉轴的中点对齐。
baseline: 项目的第一行文字的基线对齐。
stretch（默认值）：如果项目未设置高度或设为auto，将占满整个容器的高度。
```
#### align-content(多根轴线的对齐方式。如果项目只有一根轴线，该属性不起作用)

```
flex-start：与交叉轴的起点对齐。
flex-end：与交叉轴的终点对齐。
center：与交叉轴的中点对齐。
space-between：与交叉轴两端对齐，轴线之间的间隔平均分布。
space-around：每根轴线两侧的间隔都相等。所以，轴线之间的间隔比轴线与边框的间隔大一倍。
stretch（默认值）：轴线占满整个交叉轴。
```

[参考链接](http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html)




