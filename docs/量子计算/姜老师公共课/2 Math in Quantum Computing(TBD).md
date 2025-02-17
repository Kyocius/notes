## 向量

### 单位向量（Unit Vector）

$$
e_1 = \begin{pmatrix}
1 \\
0 \\
0
\end{pmatrix}, \quad e_2 = \begin{pmatrix}
0 \\
1 \\
0
\end{pmatrix}, \quad e_3 = \begin{pmatrix}
0 \\
0 \\
1
\end{pmatrix}
$$

### 向量的模（Norm）

向量的 $L^p$ 模（$L^p$-norm ）用于判断向量大小：

$$
||v||_{p}:=\left(v_{1}^{p}+v_{2}^{p}+...+v_{n}^{p}\right)^{\frac{1}{p}}
$$

P=2 时是*欧几里得距离*。

### 向量点乘/内积（Dot Product）

产生标量。

### 向量外积

$$
\begin{pmatrix}x_1\\x_2\\\vdots\\x_N\end{pmatrix}\begin{pmatrix}y_1&y_2&\cdots&y_M\end{pmatrix}=\begin{pmatrix}x_1y_1&x_1y_2&\cdots&x_1y_M\\x_2y_1&x_2y_2&\cdots&x_2y_M\\\vdots&\vdots&\ddots&\cdots\\x_Ny_1&x_Ny_2&\cdots&x_Ny_M\end{pmatrix}
$$

## 矩阵

### 常用操作符

- Pauli X operator：

$$
\sigma_x = X:=\begin{pmatrix}
0  &1\\
1  &0\\
\end{pmatrix}
$$



- Pauli Z operator：

$$
\sigma_z = Z:=\begin{pmatrix}
1  &0\\
0  &-1\\
\end{pmatrix}
$$



- Pauli Y operator：

$$
\sigma_y = Y:=\begin{pmatrix}
0  &-i\\
i  &0\\
\end{pmatrix}
$$



- Hadamard operator：

$$
H:=\frac 1 {\sqrt{2}} \begin{pmatrix}
1  &1\\
1  &-1\\
\end{pmatrix}
$$

### 转置（Transpose）

$$
A := \begin{pmatrix}
a & b \\
c & d \\
e & f
\end{pmatrix}, \quad A^T := \begin{pmatrix}
a & c & e \\
b & d & f
\end{pmatrix}
$$


$$
A \cdot A^T = 1
$$

### 共轭（Conjucate）

共轭一个矩阵就是共轭它的所有元素。

$$
\bar{C} := \begin{pmatrix}
\overline{1 + i} & \bar{0} \\
\bar{0} & \overline{1 - i}
\end{pmatrix} = \begin{pmatrix}
1 - i & 0 \\
0 & 1 + i
\end{pmatrix}
$$

$A^\dagger$ 表示共轭转置矩阵。

### 酉算子（Unitary Operator）

酉算子的逆，是它自己的共轭转置矩阵。

### 迹（Trace）

对角线之和。

$$
A = \begin{pmatrix}
1 &3 \\
8 &4
\end{pmatrix} \mapsto 1 + 4 = 5
$$

转置之后，矩阵的迹不变。

## 张量（Tensor）

### 张量乘法

$$
u \otimes v = \begin{pmatrix} a \\ b \end{pmatrix} \otimes \begin{pmatrix} c & d & e \end{pmatrix} := \begin{pmatrix} a \cdot c & a \cdot d & a \cdot e \\ b \cdot c & b \cdot d & b \cdot e \end{pmatrix}
$$

$$
\begin{pmatrix} r \\ s \\ t \end{pmatrix} \otimes \begin{pmatrix} x \\ y \end{pmatrix} := \begin{pmatrix} r \cdot x \\ r \cdot y \\ s \cdot x \\ s \cdot y \\ t \cdot x \\ t \cdot y \end{pmatrix}
$$

## 集合论（Set Theory）

### 笛卡尔积（Cartesian）

$$
S = \{1,2,3\}, \quad T=\{ 4,5 \}
$$

$$
S \times T = \{(1,4),(2,4),(3,4),~(1,5),(2,5),(3,5) \}
$$

### 关系

关系是笛卡尔积的子集。

### 映射

- 如果 f 是双射，那么 f 可逆。

## 向量空间

### 群

- 封闭性
- 结合律
- 单位元
- 逆元

详情见 `大学二年级（上）→ 离散数学 → 群论`。

### 环（Rings）

环是一个阿贝尔群加上一个运算（通常被称为乘积运算）。

### 域（Fields）

域是一个交换环加上一个运算，对于域内非零元素 x，存在 $x^{-1}$ 使得：
$$
x \ast x^{-1} = x^{-1} \ast x = 1
$$
运算满足：

- 分配律
- 结合律
- 单位元

### 向量空间

包含一堆向量的地方。向量空间是一个域。

### 展开（Span）

### 线性独立

### 基和维度

- **基（Basis）：**一个向量空间的 V 的基是一个线性独立的集合。
- **维度：**向量的基中，向量的个数。

### 正交基（Orthonormal）

- 向量正交，内积是 0：$\langle u,v \rangle = 0$。
- 施密特正交化（Gram-Schmidt Orthogonalization）。

### 矩阵就是线性变换

## 矩阵作为运算

### 行列式（Determinant）

### 伴随矩阵

### 求矩阵的逆

## 特征值和特征向量（Eigenvalue）

### 特征值











