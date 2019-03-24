# d3学习

> 学习目标

- 柱状图，饼状图，树形图，网状图
- 平滑的线
- 动画
- 事件


### 动画

### 动画并发队列

### 多边形-地图



> select

元素选择器，类似于jquery，不做累述
- select   选择第一个
- selectAll 选择所有


> bindData

- datum  绑定一个数据
- data   绑定一个数组

*text()* 函数 参数 (data, index)


> dataArr

选择根节点 => 选择所有子节点 => data => enter => append => [attr, text]

- data后进入enter
- append会根据data补齐

> scale 

缩放是处理显示比例的工具


### Tree的使用

- 创建svg
- 使用d3.tree().size()创建 tree 布局
- size 接收两个参数设置大小 size([300, 600])
- d3.hierarchy(data) 传入符合数据的数据，返回具备同样结构的节点数据，根节点 root
- svg下构造g (group)[分组] 
- g 中 根据 tree(root).links() 返回的节点连接关系 添加 link 连线 
- g 下面 使用 g 构造节点 node  transform 属性设置位置
- node 下 增加 circle
- node 写增加 text 设置x y