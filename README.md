# 泰坦尼克可视化展示


## 总结

该项目使用了泰坦尼克号人员生还情况的舱位等级、性别、年龄等数据创建了3张图表：

1. 泰坦尼克号乘客生还情况（按舱位等级分类）： 舱位等级越高的乘客，其生还几率越高。
2. 泰坦尼克号乘客生还情况（按年龄分类）： 越年轻的乘客（比如孩子）生还几率越高。
3. 泰坦尼克号乘客生还情况（按性别和舱位等级分类）：女性的生还几率要高于男性，越高等级的乘客生还几率越高。

## 设计思路
* 图表类型： 数据集包含了不同类型乘客的信息，所以条形图是一个比较好的选择。
* 布局： 生还人员有超过2个以上的类别信息，所以用堆积条形图会是不错的布局。
* 图例： 数据以比例方式呈现，因此堆积图具有同样的高度，图例设置在右上角。
* 视觉编码：x轴代表不同的类别信息，y轴代表乘客的比例信息；不同的颜色用来代表生还或者死亡的乘客。


## 反馈
### 1
第一张图的颜色对比有些奇怪，可以尝试下优化颜色配比。

### 2
NA数据组可以直接被删除掉，它并没有传递更多的信息。

### 3
可以尝试更多维度的呈现方式，是否有其他的呈现方法？

###4
只是在纵轴采用了生存率的比例，但是比例的单独存在并不具有实际意义。在悬浮的tooltip上，我加上了数字的显示。

### 最后展示链接
https://github.com/GooseHuang/P6.git

### 参考资源
* [D3js](https://github.com/d3/d3/wiki)
* [D3BarChart](https://vegibit.com/create-a-bar-chart-with-d3-javascript/)
* [Color Brewer](http://colorbrewer2.org/#type=sequential&scheme=BuGn&n=3)