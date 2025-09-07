# TensorFlow入门(7月22日)
## 1.常见的损失函数
![alt text](image.png)
![alt text](image-1.png)
### 1.1 分类任务
在分类任务中，最多使用的是


<font color = red>交叉熵损失函数</font>，下面介绍这种损失函数：
#### 1.1.1 多分类任务
![alt text](image-2.png)
![alt text](image-3.png)
![alt text](image-4.png)  

在`tf.keras`中使用`CategoricalCrossentropy()`实现，如下图所示：    
<br>
![alt text](image-5.png)

#### 1.1.2 二分类任务
在二分类任务中，使用`BinaryCrossentropy()`实现，如下图所示：
![alt text](image-6.png)

### 2.1 回归任务
#### 2.1.1 MAE损失（L1 loss）
![alt text](image-7.png)
![alt text](image-8.png)    

在`tf.keras`中使用`MeanAbsoluteError()`实现，如下图所示：    
![alt text](image-9.png)

#### 2.1.2 MSE损失(L2 loss 欧氏距离)
![alt text](image-10.png)
![alt text](image-11.png)
**<font color = red>注意：</font> L2loss也常常作为正则项。当预测值与目标值相差很大时，梯度容易爆炸。**    

在`tf.keras`中使用`MeanSquaredError()`实现，如下图所示：
![alt text](image-12.png)

#### 2.1.3 smooth L1损失
![alt text](image-13.png)
![alt text](image-14.png)
![alt text](image-15.png)    

在`tf.keras`中使用`Huber()`实现，如下图所示：    
![alt text](image-16.png)