## Dirac 表示法

### Ket 标记

$$
|0\rangle:=\begin{pmatrix}1\\0\end{pmatrix}\\
|1\rangle:=\begin{pmatrix}0\\1\end{pmatrix}
$$

我们管这种**列**向量叫做 **Ket**，把它们的共轭转置向量叫做 **Bra**，类似 $\langle 0|$ 形式。

**Braket：**长成 $\langle 1 |1\rangle$ 形式，其实就是乘积。

### Bra-Ket 的性质

主要特性：

+ 所有 Ket 都有对应的 Bra
+ 常量乘法
+ 共轭对称性
+ 线性
+ 模是正的

其它特性：

- 三角不等式
- 施瓦茨不等式（Schwartz）
- 判断正交（Othonormal）

## 量子比特（Qubits）

### Measurement

### Normalization

### Qubits States

- $|+ \rangle = (|0\rangle +|1\rangle) / \sqrt{2}$

- $|- \rangle = (|0\rangle -|1\rangle) / \sqrt{2}$

## 布洛赫球（Bloch Sphere）

## 量子操作（Quantum Operators）

### 逻辑门

逻辑门 = 酉矩阵 = 基的改变
$$
U=\sum|\psi_k\rangle\langle\psi_k| \quad (\langle\psi_j|\psi_k\rangle=\delta_{jk})
$$

### 量子寄存器（Register）

量子寄存器是张量积。

### 电路线（Circuit Wires）

- Pauli X：NOT
- 
