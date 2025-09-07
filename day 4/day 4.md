# TensorFlow入门(7月21日)
## 1.参数初始化
![alt text](image.png)
### 1.1 随机初始化(很少使用)
![alt text](image-1.png)
### 1.2 标准初始化（很少使用）
![alt text](image-2.png)
### 1.3 Xaiver初始化
#### 1.3.1 正态化Xavier初始化
![alt text](image-3.png)    
**实现方法：**    
![alt text](image-4.png)    
**输出结果：**    
![alt text](image-5.png)
#### 1.3.2 标准化Xavier初始化
![alt text](image-6.png)    
**实现方法：**    
![alt text](image-7.png)    
**输出结果：**    
![alt text](image-8.png)
### 1.4 He初始化
![alt text](image-9.png)
#### 1.4.1 正态化He初始化
![alt text](image-10.png)   
**实现方法：**    
![alt text](image-11.png)    
**输出结果：**    
![alt text](image-12.png)
#### 1.4.2 标准化He初始化
![alt text](image-13.png)  
**实现方法：**    
![alt text](image-14.png)
## 2.神经网络的搭建
![alt text](image-15.png)
![alt text](image-16.png)
![alt text](image-17.png)
### 2.1 通过Sequential()搭建神经网络
![alt text](image-18.png)
![alt text](image-19.png)
### 2.2 通过function API搭建神经网络    
**原理：将<font color = red>层</font>作为可调用<font color = red>对象</font>并返回<font color = red>张量</font>,并将输入向量和输出向量提供给`tf.keras.Model`的`imputs`和`outputs`参数**<br>    
![alt text](image-20.png)
### 2.3 通过model的子类构建
![alt text](image-21.png) <br>   
**复习：call()方法**    
![alt text](image-22.png)    

#### 2.3.1 实现方法：
> 1. 定义一个model的子类，继承tf.keras.Model
> 2. 定义__init__()方法，初始化model的层结构
> 3. 定义call()方法，定义网络的前向传递

## 3. 神经网络的优缺点
![alt text](image-23.png)