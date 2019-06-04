## 坐标

以页面的左上角为(0,0)坐标点，坐标以像素为单位，x轴正方向是向右，y轴正方向是向下

## 矩形（rect）
```
<rect x="10" y="10" width="50" height="50" rx="10" ry="10" />
```

属性 | 描述
---|---
 x | 矩形x坐标 
 y| 矩形y坐标
 width|矩形的宽度
 height|矩形的高度
 rx|圆角的x方向半径
 ry|圆角的y方向的半径

## 圆形（circle）
```
<svg width="200" height="200" style="background: #333;">
    <circle cx="100" cy="100" r="80" fill="#000"></circle>
    <circle cx="100" cy="100" r="50" fill="red"></circle>
    <circle cx="100" cy="100" r="30" fill="skyblue"></circle>
    <circle cx="100" cy="100" r="10" fill="#fff"></circle>
</svg>
```

svg里的图形是后来居上，所以上面的四个圆形按顺序，第一个在最下层显示，最后面的在最上层显示

属性 | 描述
---|---
 cx | 圆心x坐标（相对于svg x轴的距离） 
 cy| 圆心y坐标（相对于svg y轴的距离）
 r|圆的半径

## 椭圆（ellipse）
```
<svg width="200" height="200" style="background: #333;">
    <ellipse cx="100" cy="100" rx="50" ry="20" fill="red"/>
</svg>
```

椭圆的属性跟圆相似，区别是x轴半径跟y轴半径各有一个属性表达

属性 | 描述
---|---
 cx | 圆心x坐标（相对于svg x轴的距离） 
 cy| 圆心y坐标（相对于svg y轴的距离）
 rx| x轴半径
 ry| y轴半径

 ## 直线（line）

 ```
<svg width="200" height="200" style="background: #333;">
    <line x1="10" y1="10" x2="190"  y2="190" stroke="#fff" stroke-width="4"/>
</svg>
 ```
 line描述了一条直线，即从一点到另一点的线条

 属性 | 描述
---|---
 x1 | 起始点x坐标 
 y1| 起始点y坐标
 x2| 终点x坐标
 y2| 终点y坐标
 stroke|线条颜色（这是个共有属性，每个形状都有，描述了图形外轮廓的颜色）
 stroke-width| 线条的宽度 同stroke 是所有图形的共有属性

  ## 曲线（polyline）
  曲线是是一条多个点组和成的非闭合的曲线或折线
  ```
  <svg width="200" height="200" style="background: #333;">
    <polyline points="20,10 0,200 80,80" stroke="red" fill="none" />
  </svg>
  ```
  
 属性 | 描述
---|---
 points | 点的集合 即是x,y坐标的集合 [x,y x1,y1, x2,y2,....]
 fill |连线区域的填充色，默认为黑色，如果只希望现实线段则设置为none