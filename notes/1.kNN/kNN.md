## 0. 概述

k近邻法（k-nearest neighbor, k-NN) 是一种基本**分类**与**回归**方法

基本做法：给定一个训练数据集，其中的实例类别已定。分类时，对新的实例，根据其 $k$ 个最近邻的训练示例的类别，通过多数表决等方式进行预测

不具有显示学习的过程

 $k$ 近邻模型对应于基于训练数据集对特征空间的一个划分。$k$ 近邻法中，当训练集、距离度量、 $k$ 值及分类决策规则确定后，其结果唯一确定。 

三个基本要素： $k$ 值的选择，距离度量，分类决策规则

## 1. k值的选择

k值小时，模型变得复杂，容易发生过拟合

k值大时，模型更简单

通常采用**交叉验证法**来选取最优的k值



## 2. 距离度量

一般使用欧氏距离

[距离度量]: D:\code\ml\笔记\0.fundamental\distance_metric.md



## 3. 分类决策规则……

常用的分类决策规则是多数表决，对应于风险经验最小化



## 4. $kd$ 树……



## 5. 距离加权

首先计算每个点和测试点的距离，然后引入权重
$$
w=\left\{
\begin{array}{1}
\frac{1}{d^2} \qquad \qquad \ \ (1) \\
\frac{1}{d+c} \qquad \qquad (2) \\
ae^{-\frac{(x-b)^2}{-2c^2}} \qquad (3)
\end{array}
\right.
$$
引入权重后，距离测试点更近（代表与测试点更加相似）的点权重更大，因此对于分类更加有效，并且如果使用（1）式或（2）式，当某点与测试点距离太过于接近时，会导致该点权重过大 $\mathop{lim} \limits_{d \to \infty} \ w \to \infty $ ，而（3）式在距离接近时权重不会过大



## 6. 剪辑近邻法……



## 7. 压缩近邻法……



# 参考

 https://blog.csdn.net/v_july_v/article/details/8203674   超详细解释

  https://www.cnblogs.com/listenfwind/p/10685192.html  代码