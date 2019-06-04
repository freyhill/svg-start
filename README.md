## 坐标

以页面的左上角为(0,0)坐标点，坐标以像素为单位，x轴正方向是向右，y轴正方向是向下

## 矩形（rect）
```
<rect x="10" y="10" width="50" height="50" rx="10" ry="10" />
```

属性 | 用法
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

属性 | 用法
---|---
 cx | 圆心x坐标（相对于svg x轴的距离） 
 cy| 圆心y坐标（相对于svg y轴的距离）
 r|圆的半径

