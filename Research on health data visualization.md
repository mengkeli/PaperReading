##Research on health data visualization##
by 李孟珂

---
#### TensorFlow
tensor张量（矩阵的推广，表示更多维度的矩阵）
flow流（一层层的计算可以看作是张量在计算模型上的流动）

一个机器学习的流水线应当作为一个数据流（DataFlow）来刻画和抽象。

支持C/C++/python，python库更易用

1. 综述

- 用图(Graph)表示计算任务
- 在会话(Session)的上下文(context)中执行图
- 用tensor表示数据
- 用变量(Variables)维护状态
- 用feed和fetch为任意操作赋值，或者从其中获取数据
一个TensorFlow图描述了计算的过程，Graph必须在Session里被启动，Session将图的op分发到CPU或GPU等设备上，执行知乎返回产生的Tensor
在python中，返回tensor的是numpy(ndarray)对象，在C/C++中返回tensor的是tensorflow::Tensor实例

2. 计算图

- 构建阶段：op的执行步骤被描述成一个Graph，
- 执行阶段：使用Session来执行图中的op (例如在构建阶段创建Graph来表示和训练神经网络，然后在执行阶段反复执行图中的训练op)

3. 构建图

```
import tensorflow as tf

matrix1 = tf.constant([[3., 3.]])     //创建一个常量op，为一个1×2矩阵，即为一个节点
matrix2 = tf.constant([[2.], [2.]])   //另一个op，为2×1矩阵
product = tf.matmul(matrix1, matrix2) //创建一个矩阵乘法op，把matrix1和matrix2作为输入，返回值product为结果
```
现在已经建立好了一个图，其中有两个constant() op, 一个 matmul() op.

4. 在Session中启动图

第一步创建一个Session对象
```

```
---
#### TensorBoard
1. 可视化TensorFlow中的数据流，以及训练过程中accuracy、bias等变化的动态图
横坐标是tag，纵坐标是run，由tag和run决定呈现的内容
tag：
标量scalr:数值型变量，如accuracy/dropout/bias/weight/交叉熵等
直方图histogram：其实是数据分布随时间的变化的图形，如weight/bias/activation/pre-activation
图像images：如果是图像方面的应用，可以观察过程中的图像
图形graph：tensor张量和op操作通过边连接起来构成的图形，直观展示代码中构成的图形的连接关系

2. 代码

