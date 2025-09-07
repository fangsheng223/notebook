# TensorFlow入门(7月18日)
## 1.初识TensorFlow
>![alt text](image.png)
## 2.张量（Tensor）
张量是一个<font color = "red">多维数组</font>
>![alt text](image-1.png)
### 2.1 TensorFlow库的导入
>![alt text](image-2.png)
`import tensorflow as tf`  
### 2.2 张量的创建
代码：
>![alt text](image-3.png)   

结果：
>![alt text](image-4.png)
>![alt text](image-5.png)

**语法：`变量名 = tf.constant(值,dtype=数据类型,shape=(维度))`**  

**【通常只用在函数内写出对应维度的值即可】**

#### 创建更高维的张量：
![alt text](image-6.png)
### 2.3 张量转换为numpy
通常由两张方式转换：
- 利用numpy：`np.array(张量)`
- 利用TensorFlow：`张量.numpy()`
### 2.4 张量的运算
#### 2.4.1 简单运算：
![alt text](image-7.png)
#### 2.4.2 聚合运算
![alt text](image-8.png)
### 2.5 变量
![alt text](image-9.png)
**变量是一种特殊的张量，形状是不可变的，但<font color = "red">可以更改其中的参数</font>**  
语法： **`变量名 = tf.Variable(初始值,dtype=数据类型)`**  
更改语法： **`变量名.assign(新的值)`**
## 3.kears介绍
>![alt text](image-10.png)
### 3.1 常用模块
>![alt text](image-11.png)
### 3.2 常用方法
#### 3.2.1 深度学习实现的主要流程
1. 获取数据
2. 数据基本处理
3. 模型创建与训练
4. 模型测试与评估
5. 模型预测
>![alt text](image-12.png)
##### 3.2.1.1 模型测试与评估
![alt text](image-13.png)
##### 3.2.1.2 回调函数
![alt text](image-14.png)
##### 3.2.1.3 模型保存与加载（参数与模型结构）
![alt text](image-15.png)