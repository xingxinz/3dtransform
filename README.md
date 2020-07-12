# 3dtransform
效果：https://xingxinz.github.io/3dtransform/  

# 书本翻页效果总结  
1. transform 来实现2D/3D变换  
种类：平移、放缩、旋转、倾斜、透视  
细节： 透视效果(perspective)、变换基准（transform-origin）  
2. animation 来实现周期逆放动画  

# 正方体/商品展示效果总结  
关于transform顺序的个人理解  
写在同一个transform里的变换顺序，有两种理解方式：  
1.先做的变化写在后面 （这种理解 是基于一个全局固定的坐标系）  
2.先做的变化写在前面 （这种理解 是基于变化物体的物坐标系 物坐标系会根据已有的变化而改变朝向）  

例如：写正方体的左面 即可以按第一种理解 写成  
 .left {transform: translateX(-100px) rotateY(-90deg);}  
也可按第二种理解写成  
.left{transform: rotateY(-90deg) translateZ(50px);}  





