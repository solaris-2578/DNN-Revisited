# DNN Regularization

## [Distance metrics][1]

Comparing similarities between objects is an essential component of machine learning. Feature vectors allow us to represent objects so that we may compare them in a variety of ways. 

Suppose that we have two feature vectors, $x = (x_1, x_2, ..., x_n)$ and $y = (y_1, y_2, ..., y_n)$. 

There are different norms to measure distance, such as $\rm{L_0}$,  $\rm{L_1}$,  $\rm{L_2}$. Among these norms, $\rm{L_2}$, the ***Euclidian distance*** is a standard approach.

### $\rm{L_0}$ norm

The $\rm{L_0}$ norm, $\left \| \cdot  \right \|_0$,counts the total nonzero elements of a vector. 

The $\rm{L_0}$ distance between the origin (0, 0) and vector (0, 5) is 1, for example, because there’s only one nonzero element. The $\rm{L_0}$ distance between (1, 1) and (2, 2) is 2, because neither dimension matches up. Imagine that the first and second dimensions represent username and password, respectively. If the L0 distance between a login attempt and the true credentials is 0, the login is successful. If the distance is 1, either the username or password is incorrect, but not both. Finally, if the distance is 2, neither username nor password is found in the database.

### $\rm{L_1}$ norm

The $\rm{L_1}$ norm, shown in figure 1.8, is defined as $\sum x_n$. The distance between two vectors under the $\rm{L_1}$ norm is also referred to as the ***Manhattan distance***. 

Imagine living in a downtown area like Manhattan, where the streets form a grid. The shortest distance from one intersection to another is along the blocks. Similarly, the $\rm{L_1}$ distance between two vectors is along the orthogonal directions. The distance between (0, 1) and (1, 0) under the $\rm{L_1}$ norm is 2. Computing the L1 distance between two vectors is the sum of absolute differences at each dimension, which is a useful measure of similarity.

![image-20211024113239275](C:\Users\solaris2578\AppData\Roaming\Typora\typora-user-images\image-20211024113239275.png)

### $\rm{L_2}$ norm

The $\rm{L_2}$ norm, shown in figure 1.9, is the Euclidian length of a vector, mathematically expressed as

$$\left \| x-y  \right \|_2 = \sqrt{(x_1-y_1)^2 + (x_2-y_2)^2+\dots+(x_n-y_n)^2}$$

It’s the most direct route you can possibly take on a geometric plane to get from one point to another. $\rm{L_2}$ norm is the shortest distance between two points in space.

![image-20211024113704376](C:\Users\solaris2578\AppData\Roaming\Typora\typora-user-images\image-20211024113704376.png)

[1]: https://livebook.manning.com/book/machine-learning-with-tensorflow-second-edition/chapter-1/101 "Machine Learning with TensorFlow, 2e, Chapter 1.3"



