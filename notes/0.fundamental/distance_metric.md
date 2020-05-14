$L_p$距离，称为**闵可夫斯基距离** $Minkowski \ distance$
$$
L_p(x_i,x_j)=(\sum_{l=1}^n\vline x_i^{(l)}-x_j^{(l)}\vline^p)^{\frac{1}{p}} \qquad p \ge 1
$$
当 $p=1$ 时，称为**曼哈顿距离** $Manhattan \ distance$
$$
L_1(x_i,x_j)=\sum_{l=1}^n\vline x_i^{(l)}-x_j^{(l)}\vline
$$
当 $p=2$ 时，称为**欧氏距离** $Euclidean \ distance$
$$
L_2(x_i,x_j)=(\sum_{l=1}^n\vline x_i^{(l)}-x_j^{(l)}\vline^2)^{\frac{1}{2}}
$$
当 $p = \infty$ 时，称为**切比雪夫距离** $Chebyshev \  distance$
$$
L_\infty(x_i,x_j) = \mathop{max} \limits_l \vline x_i^{(l)}-x_j^{(l)}\vline
$$
![1588950885129](C:\Users\86768\AppData\Roaming\Typora\typora-user-images\1588950885129.png)



 https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.DistanceMetric.html#sklearn.neighbors.DistanceMetric 

