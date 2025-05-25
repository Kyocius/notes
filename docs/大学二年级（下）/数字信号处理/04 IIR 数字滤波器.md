## 模拟滤波器设计

1. 模拟低通滤波器的幅频响应 $|H(j\Omega)|$

    ![6.2](./images/04/pin-05-25.png){width="80%"}

2. 巴特沃斯滤波器幅频特性与 N 的关系

    ![6.2](./images/04/pin-05-25_1.png){width="80%"}

巴特沃斯归一化参数表：

![6.2](./images/04/pin-05-25_2.png)

![6.2](./images/04/pin-05-25_3.png)

??? success "例题 1"
	![6.2](./images/04/pin-05-25_4.png)
	

	1. 计算 N
	2. 查表 (表 6.2.1 之二) 求归一化低通滤波器的传输函数 $G_a(p)$
	3. 计算 3dB 截止频率 $\Omega_c$
	4. 令 $P = \frac{s}{\Omega_c}$ 代入 $G_a(p)$ 得到 $H_a(s)$ 即为所求滤波器的传输函数
	
	![6.2](./images/04/pin-05-25_5.png)
	![6.2](./images/04/pin-05-25_6.png)


??? success "例题 2"
	![6.2](./images/04/pin-05-25_7.png)	

## 数字滤波器及其原理

### 模拟与数字

![6.2](./images/04/pin-05-25_8.png)

### 模拟频率 $\Omega$ 与 $f$

![6.2](./images/04/pin-05-25_9.png)

### 模拟频率 $\Omega$ 与数字频率 $\omega$

![6.2](./images/04/pin-05-25_10.png)

![6.2](./images/04/pin-05-25_11.png)

### 模拟、数字频响特性曲线比较

![6.2](./images/04/pin-05-25_12.png)

快速判断数字滤波器类型的方法：

![6.2](./images/04/pin-05-25_13.png){width="70%"}

## 脉冲响应不变法

#### s 域和 z 域的转换

![6.3](./images/04/pin-05-25_14.png)

![6.3](./images/04/pin-05-25_15.png)
	![6.3](./images/04/pin-05-25_16.png)
	![6.3](./images/04/pin-05-25_17.png)

??? success "例题 1"
	![6.3](./images/04/pin-05-25_18.png)
	![6.3](./images/04/pin-05-25_19.png)
	![6.3](./images/04/pin-05-25_20.png)
	
??? success "例题 2"