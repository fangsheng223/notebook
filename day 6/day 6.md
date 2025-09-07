# TensorFlow入门(7月23日)
## 1.深度学习的优化方法
### 1.1 梯度下降算法（使损失函数最小化）
![alt text](image.png)
![alt text](image-1.png)
![alt text](image-2.png)
![alt text](image-3.png)
![alt text](image-4.png)
![alt text](image-5.png)
### 1.2 反向传播算法（BP算法）
![alt text](image-6.png)
#### 1.2.1 前向传播与反向传播
![alt text](image-7.png)
![alt text](image-8.png)
#### 1.2.2 链式法则
![alt text](image-9.png)
![alt text](image-10.png)
![alt text](image-11.png)
![alt text](image-12.png)
![alt text](image-13.png)
### 1.3 梯度下降优化算法
![alt text](image-14.png)
#### 1.3.1 动量算法
**动量算法主要解决<font color = red>鞍点</font>问题**

##### 1. 指数加权平均
![alt text](image-15.png)
![alt text](image-16.png)
![alt text](image-17.png)
![alt text](image-18.png)
##### 2. 动量梯度下降算法（对梯度进行修正）
![alt text](image-19.png)
![alt text](image-20.png)
![alt text](image-21.png)
![alt text](image-22.png)
#### 1.3.2 AdaGrad算法
![alt text](image-23.png)
![alt text](image-24.png)
![alt text](image-25.png)
#### 1.3.3 RMSprop算法（对学习率进行修正）
![alt text](image-26.png)
![alt text](image-27.png)
#### 1.3.4 Adam算法（对梯度和学习率进行修正）
![alt text](image-28.png)
![alt text](image-29.png)
![alt text](image-30.png)
### 1.4 学习率退火
![alt text](image-31.png)
#### 1.4.1 分段常数衰减
![alt text](image-32.png)
![alt text](image-33.png)
![alt text](image-34.png)
#### 1.4.2 指数衰减
![alt text](image-35.png)
![alt text](image-36.png)
![alt text](image-37.png)
#### 1.4.3 1/t衰减
![alt text](image-38.png)
![alt text](image-39.png)
![alt text](image-40.png)
