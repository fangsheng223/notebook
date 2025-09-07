# TensorFlow入门(7月20日)
# 1.深度神经网络
## 1.1 什么是神经网络
![alt text](image.png)
树突接收信号->通过神经元处理->轴突输出结果
### 1.1.1 怎么构建人工神经网络中的神经元
![alt text](image-1.png)
![alt text](image-2.png)
![alt text](image-3.png)
### 1.1.2 神经元是如何工作的？
![alt text](image-4.png)
![alt text](image-5.png)
## 1.2激活函数
**激活函数：<font color = "red">引入非线性因素</font>**
![alt text](image-6.png)
### 1.2.1 Sigmoid函数
1. #### Sigmoid函数一般用于<font color = "red">二分类的输出层</font>
>![alt text](image-7.png)
>![alt text](image-8.png)
**实现方法：**  
![alt text](image-9.png)    
**输出结果：**
![alt text](image-10.png)
### 1.2.2 tanh函数
![alt text](image-11.png)
![alt text](image-12.png)
> 1. 收敛速度快，迭代次数少
> 2. 隐藏层使用tanh函数,输出层使用sigmoid函数    
> 
**实现方法：**    
![alt text](image-13.png)   
**输出结果：**    
![alt text](image-14.png)
### 1.2.3 relu函数
1. relu函数是<font color = "red">最常用</font>的激活函数            
![alt text](image-15.png)
![alt text](image-16.png)
2. relu的优势:    
![alt text](image-17.png)    
>1. 节省计算量
>2. 避免梯度消失
>3. 由于部分输出为0，减少参数的相互依存性，缓解过拟合    

**实现方法：**    
![alt text](image-18.png)    
**输出结果：**    
![alt text](image-19.png)    
### 1.2.4 leakrelu函数
1. leakrelu函数是<font color = "red">relu函数的变种</font>，在relu函数的左侧添加一个斜率，即<font color = "red">leak</font>    
>![alt text](image-20.png)    

**实现方法：**    
![alt text](image-21.png)    
### 1.2.5 softmax函数
1. softmax函数用于<font color = "red">多分类问题</font>,是二分类函数sigmoid函数的推广，目的是将多分类的结果以概率的形式展现出来。
![alt text](image-22.png)
![alt text](image-23.png)

**实现方法：**    
![alt text](image-24.png)
### 1.2.6 其他激活函数
![alt text](image-25.png)
## 1.3 如何选择激活函数
![alt text](image-26.png)