[TOC]


$$
\lim_{x \rightarrow 0}\int_0^{g(x)} f(x) dx \sim x^n \\
\lim_{x \rightarrow 0} f(x) \sim x^m \\
\lim_{x \rightarrow 0} g(x) \sim x^l \\
n = m + l \\
$$


$$
\lim_{x \rightarrow 0}\int_{h(x)}^{g(x)} f(x) dx \sim x^n \\
\lim_{x \rightarrow 0} f(x) \sim x^m \\
\lim_{x \rightarrow 0} g(x) \sim x^l \\
\lim_{x \rightarrow 0} h(x) \sim x^k \\
x^n \sim x^{m + 1}(g^{'}(x) - h^{'}(x))
$$
.



可以将极限各个部分分开计算



# 极限

$$
\ln (x + \sqrt{1 + x^2}) \sim x \\
\lim_{x \rightarrow 0^+} x^\alpha \ln^\beta f(x) = 0 \\
\alpha \sim \beta \rightarrow 0^+ \Rightarrow \ln\alpha \sim \ln\beta \rightarrow -\infty \\
$$

- 添加项或减少项

- 将等价无穷小逆用
  $$
  \lim_{x \rightarrow 1} x - 1 = \ln x
  $$

- 遇到幂指函数取指对数

- 中值定理

- 将有ln的等价无穷大替换



# 泰勒展开

泰勒展开式相乘应保证展开的最低次乘展开的最高次等于目标次数
$$
f(x_0 + h) = f(x_0) + f'(x_0)h + f''(x_0)h^2 + \dots
$$


# 连续性

判断连续性

- 先判断分母为0
- 在判断子函数原本就不存在的点



# 导数

$$
f(x) = |\phi(x)|g(x) 不可导点在\phi(x_0) = 0处，当g(x_0) = 0时是可到的
$$

导数题注意函数连续性，导函数连续性

若奇阶导数为零，则下个不为零的偶阶导数大于零为最小值，小于零为最大值

偶阶导数不为零判断极值，奇阶导数不为零判断拐点

在可导的条件下，拐点与极值点不能是同一点



若$$f'(a)>0$$不能判断$$x = a $$附近单调递增，但是可以判断$$f(a + 0) > f(a)$$



# 单调性

$$
f'(x) > 0 \Rightarrow f(x)单调递增 \\
f(x)单调递增 \Rightarrow f'(x) \ge 0 \\
$$





## 反例

$$
f(x) = \begin{cases}
1,x\ne 0 \\
0, x = 0 
\end{cases}
$$





# 高阶微分





# 不等式

$$
\frac{x}{1 + x} \le \ln(x + 1) \le \frac{1}{x}
$$







# 原函数存在定理

连续函数存在原函数

不连续函数但存在震荡间断点可能存在原函数
$$
F(x) = \left\{
\begin{matrix}
	x^2 \sin \frac{1}{x} ,\ x \ne 0 \\
	0, \ x = 0
\end{matrix}
\right.
$$




# 微分中值定理


$$
f(\xi)f''(\xi) - n(f'(\xi))^2 = 0 \Rightarrow F(x) = \frac{f'(x)}{f^n(x)}
$$


- 罗尔定理

$$
f'(\xi) + p(\xi)f(\xi) = q(\xi) \\
F(x) = f(x) e^{\int p(x) dx} - \int q(x) e^{\int p(x) dx} dx \\
F'(x) = e^{\int p(x) dx}[f'(x) + p(x)f(x) - q(x)]
$$



- 辅助多项式

若存在$f^{(k)}(x) = A$，则构造$F(x) = f(x) - a_kx^k + \cdots + a_0$



- 双函数





- 双中值

1. 不相等，可以设$\mu = a + b - \lambda$
1. $存在af(b) + bf(a)除以ab$
1. 注意是否有等于零的点，有则用罗尔定理



虚假的双中值定理可以从两个方向化简



# 不等式证明

- 倒代换
- 求出若干阶导数使用泰勒公式







# 有理积分

$$
\int \frac{Ax + B}{x^2 + px + q} dx =
$$



**留数法**

- 将有理分式拆分
- 让各个项的值为0，得到解
- 在原式中去除对应项在带入解



# 区间再现

$$
\int_a^b f(x) dx = \int_a^b f(a + b - x) dx
$$





# 积分奇偶性


$$
f(-x) = -f(x) \\
F(x) = \int_a^x f(t) dt \\
F(x) - F(-x) = \int_a^x f(t) dt - \int_a^{-x} f(t) dt =  \int_a^x f(t) dt + \int_{-x}^a f(t) dt = \int_{-x}^x f(t) dt = 0
$$

$$
f(-x) = f(x) \\
F(x) = \int_a^x f(t) dt \\
F(x) + F(-x) = \int_a^x f(t) dt + \int_a^{-x} f(t) dt = \int_a^x f(t) dt - \int_{-x}^a f(t) dt = \int_{-x}^x 0 dt = 0 \\
F(0) = \int_a^0 f(t) dt \neq 0
$$


# 反常积分收敛性


$$
\int_a^{+\infty}\frac{1}{x^p} dx = \begin{cases}
	收敛 \qquad p > 1 \\
	发散 \qquad p \le 1
\end{cases}
\qquad a>0
$$

$$
\int_0^1\frac{1}{x^q} dx = \begin{cases}
	收敛 \qquad p < 1 \\
	发散 \qquad p \ge 1
\end{cases}
$$

- 无穷小替换同敛散性

$$
\int_{a}^{+\infty}\frac{1}{\ln ^\alpha x} dx = \infty \\
\int_{0}^{a}\ln ^\alpha x dx = A \\
$$







# 留数定理





# 无理积分

$$
\int \sqrt{\frac{1 + x}{1 - x}} dx = -\sqrt{1 - x^2} + 2 \arctan \sqrt{\frac{1 + x}{1 - x}} + C
$$





# 可微

一阶偏导连续推可微

可微推偏导存在和连续

连续推极限存在


$$
z = \sqrt{x^2 + y^2}在(0, 0)连续但偏导不存在 \\
f(x, y) = \frac{xy}{x^2+ y^2} (x, y) \ne (0, 0), 0 ,(x, y) = (0, 0) 偏导存在不连续
$$




# 隐函数存在定理



# 偏导线性变换





# 方向导数

$f'_x存在，沿着x轴正向的方向导数存在$

$沿着x轴正向的方向导数存在，f'_x不一定存在$



$\frac{\part u}{\part l} = (u_x, u_y, u_z) (\cos \alpha, \cos \beta, \cos \gamma)$



# 重积分计算

1. 轮换对称性
2. 对称性



# 空间解析几何

平行平面距离
$$
d = \frac{|D_0 - D_1|}{\sqrt{A^2 + B^2 + C^2}}
$$


直线与直线的夹角
$$
\cos \phi = \frac{|m_1 m_2 + n_1 n_2 + p_1 p_2|}{\sqrt{m_1^2 + n_1^2 + p_1^2}\sqrt{m_2^2 + n_2^2 + p_2^2}}
$$


平面与直线夹角
$$
\sin \phi = \frac{|Am + Bn + Cp|}{\sqrt{A^2 + B^2 + C^2}\sqrt{m^2 + n^2 + p^2}}
$$


行列式展开第二项为负



柱面方程
$$
圆柱面 \qquad x^2 + y^2 = 1 \qquad 母线平行z轴 \\
椭圆柱面 \qquad \frac{y^2}{2} + z^2 = 1 \qquad 母线平行z轴的椭圆 \\
双曲柱面 \qquad z^2 - x^2 = 1 \qquad 母线平行于y轴的双曲 \\
抛物柱面 \qquad x^2 = y
$$



# 微分算子

$$
f(x) = e^{kx} \\
y'' + 3y' + 2y = 5e^{3k} \Rightarrow y^* = \frac{1}{D^2 + 3D + 2}5e^{3k} = \frac{5e^{3k}}{3^3 + 3 \times 3 + 2} = \frac{e^{3k}} {4} \\
y* = \frac{x^n}{(G(D|_{D = k}))^{(n)}}e^{kx} \\
\\
f(x) = \sin ax / \cos ax \Rightarrow D^2 \rightarrow a^2\\
$$

# 微分方程

由解推原方程最好化为只有$e^{kx}$形式



# 无穷级数

$$
n! \approx \sqrt{2\pi n} (\frac{n}{e})^n \\
\lim_{n \rightarrow \infty} \frac{\sqrt[n]{n!}}{n} = \frac{1}{e}
$$







# 三重积分

- 投影法

- 截面法

- 球坐标

  $\iiint_\Omega f(\rho, \phi, \theta) \rho^2 \sin \phi d\rho d\phi d\theta$

- 柱坐标



**中值定理**
$$
\iiint_\Omega f(x, y ,z) dV = f(\xi, \eta, \zeta)\iiint_\Omega dV
$$




# 第一类曲线积分

- 直角坐标系
  $$
  y = y(x) \\
  \int_L f(x,y) ds = \int_L f(x, y(x)) \sqrt{1 + y'^2(x)} dx
  $$
  
- 参数方程
  $$
  \left\{
  \begin{matrix}
  	x = \phi(t) \\
  	y = \psi(t) \\
  	z = \omega(t) \\
  \end{matrix}
  \right.
  \\
  \int_L f(x, y , z) ds = \int_L f(\phi(t), \psi(t), \omega(t)) \sqrt{\phi'^2(t) + \psi'^2(t) + \omega'^2(t)} dt
  $$
  
- 极坐标
  $$
  r = r(\theta) \\
  \int_L f(x, y) ds = \int_L f(r(\theta)\cos\theta, r(\theta)\sin\theta)\sqrt{r^2(\theta) + r'^2(\theta)}d\theta
  $$
  



# 斯托克斯公式

$$
\int_\sum \begin{vmatrix}
	dydz &\ dzdx &\ dxdy \\
	\frac{\part}{\part x} &\ \frac{\part}{\part y} &\ \frac{\part}{\part z} \\
	P &\ Q &\ R
 \end{vmatrix}
$$



# 场论

- 散度
  $$
  \pmb{A}(x, y, z) = P(x, y, z)\pmb{i} + Q(x, y, z)\pmb{j} + R(x, y, z)\pmb{k} \\
  \text{div} \pmb{A} =\nabla \cdot \pmb{A} = \frac{\part P}{\part x} + \frac{\part Q}{\part y} + \frac{\part R}{\part z}
  $$
  
- 旋度

$$
\text{rot} \pmb{A} = (\frac{\part R}{\part y} - \frac{\part Q}{\part z})\pmb{i} + (\frac{\part P}{\part z} - \frac{\part R}{\part x})\pmb{j}  +(\frac{\part Q}{\part x} - \frac{\part P}{\part y})\pmb{k}
$$



- 











# 行列式计算



当遇到$$A^TA = E$$，计算$|A +kE| = |A + kAA^T| = |A||E + kA^T| = |A||(E + kA)^T|$



# 矩阵计算

存在$$E + Q^{-1}P$$变为$$Q^{-1}(Q + P)$$

证明矩阵等式两边相似时，将两边分别转换为一个中间式子


$$
A,B,A+B,A^{-1}+B^{-1},求(A^{-1} + B^{-1})^{-1} \\
\\
S = (A^{-1}+B^{-1}) \\
S^{-1} = Q = (A^{-1}+B^{-1})^{-1} \\
Q = AQ' \\
SQ = E \\
SAQ' = E \\
(E + B^{-1}A)Q' = E \\
Q' + B^{-1}AQ' = E \\
B^{-1}AQ' = E - Q'\\
Q' = A^{-1}B(E - Q') \\
Q' = A^{-1}B - A^{-1}BQ' \\
(E - A^{-1}B)Q' = A^{-1}B \\
Q' = (E - A^{-1}B)^{-1}A^{-1}B \\
S^{-1} = Q = AQ' = A(E - A^{-1}B)^{-1}A^{-1}B
$$






# 矩阵的秩

$$
0 \le r(A_{m\times n}) \le min\{m,n\} \\
r(kA) = r(A), (k\ne 0) \\
r(A) = r(PA) = r(AQ) = r(PAQ) \\
r(A) + r(B) - n \le r(AB) \le min\{r(A), r(B)\} \\
r(A + B) \le r([A, B]) \le r(A) + r(B) \\
r(\begin{bmatrix}
A \ O \\
O \ B 
\end{bmatrix}) = r(A) + r(B) \\
r(A) + r(B) \le r(\begin{bmatrix}
A \ O \\
C \ B 
\end{bmatrix}) \le r(A) + r(B) + r(C) \\
r(A) = r(A^T) = (AA^T) \\
r(A^*) = \left\{\begin{matrix}
n , \ r(A) = n \\ 
1 , \ r(A) = n - 1 \\
0 , \ r(A) < n - 1 
\end{matrix}\right. \\
A^2 = A \Rightarrow r(A) + r(A - E) = n \\
A^2 = E \Rightarrow r(A + E) + r(A - E) = n \\
AB = O \Rightarrow r(A) + r(B) \le n
$$



左边乘上列满秩或右边乘行满秩矩阵秩不变



# 线性相关

$$
\alpha_1...\alpha_n 线性无关 \\
[\beta_1...\beta_n]^T = [\alpha_1...\alpha_n]^TC 线性无关 \\
|C| \ne 0
$$

$$
\alpha_1...\alpha_n与\beta_1...\beta_m等价\Leftrightarrow等秩且一个向量组可以被另一个表示
$$





# 矩阵相似

判断矩阵是否相似

- 相似矩阵对角线元素和是特征值和
- 判断特征值重数与特征向量个数
- 若不相似与对角矩阵，则判断特征值矩阵的秩是否相等



相似的性质

- 两者的迹相等



可推出相似

- 一个二次型经过正交变换变另一二次型





# 二次型

- 从$x_1, x_2 \cdots x_n$到$y_1, y_2 \cdots y_n$的线性变换：$\pmb{x} = C \pmb{y}$



若$A$是正定矩阵，则存在$B = A^k$是正定矩阵，$B = Q^T\Lambda^k Q$



# 正定矩阵

正定矩阵的任一主子矩阵也是正定矩阵



# 矩阵结论

$$
AB = A + B \Rightarrow (A - E)(B - E) = E
$$

$$
A^n = O \ \ \Rightarrow \\
\lambda_1 = \lambda_2 = \cdots = \lambda_n = 0 \\
|f(A)| = |\sum_{k = 0}^{m}a_kA^k| \ne 0
$$










# 古典概率



概率为1或0的事件与所有事件都相互独立


$$
P(X \le a) = F(a) \\
P(X > a) = 1 - P(X \le a) = 1 - F(a) \\
P(X < a) = F(a - 0) = \lim_{x \rightarrow a^-} F(x) \\
P(X = a) = P(X \le a) - P(X < a) = F(a) - F(a - 0) \\
P(a < X \le b) = P(X \le b) - P(X \le a) = F(b) - F(a) \\
P(a < X < b) = P(X < b) - P(X \le a) = F(b - 0) - F(a) \\
P(a \le X \le b) = P(X \le b) - P(X < a) = F(b) - F(a - 0) \\
P(a \le X < b) = P(X < b) - P(X < a) = F(b - 0) - F(a - 0) \\
$$



# 正太分布

$$
\Phi(\mu - a) + \Phi(\mu + a) = 1
$$

# 独立性



离散双变量相互独立的充要条件是概率矩阵秩为1，成比例

二元正太分布的相关性和独立性的等价的



# $\Gamma$

$$
\Gamma(\alpha) = \int_0^{+\infty} x^{\alpha - 1} e^{-x}dx  \\
\Gamma(n + 1) = n! \\ 
\Gamma(n + 1) = n\Gamma(n)\\
\Gamma(\frac{1}{2}) = \sqrt{\pi}
$$



# 概率函数

$$
Z = \max\{X, Y\} = \frac{X + Y + |X - Y|}{2} \\
Z = \min\{X, Y\} = \frac{X + Y - |X - Y|}{2} 
$$





# 大数定律

切比雪夫

- 独立同分布
- 方差存在且有一致上界



伯努利

- n重伯努利试验中



辛钦

- 独立同分布
- 数学期望存在且一致



# 中心极限定律

列维—林德伯格

- 独立同分布
- 期望、方差存在

$$
\lim P\{\frac{\sum_{i = 1}^n X_i - n\mu}{\sqrt{n}\sigma} \le x\} = \Phi(x)
$$





棣莫弗—拉普拉斯

- 服从n重伯努利分布

$$
\lim P\{\frac{Y_n - np}{\sqrt{np(1 - p)}} \le x\} = \Phi(x)
$$



# 样本

$$
\frac{(n - 1)S^2}{\sigma^2} \sim \chi^2(n - 1) \\ \\
\frac{{S_1^2} / {S_2^2}}{{\sigma_1^2} / {\sigma_2^2}} \sim F(n_1 - 1, n_2 - 1) \\ \\
\sigma_1 = \sigma_2 = \sigma \Rightarrow \frac{(\bar{X} - \bar{Y}) - (\mu_1 - \mu_2)}{S_w\sqrt{\frac{1}{n_1} + \frac{1}{n_2}}} \sim t(n_1 + n_2 - 2) \qquad Sw = \sqrt{\frac{(n_1 - 1)S_1^2 + (n_2 - 1)S_2^2}{n_1 + n_2 - 2}} \\ \\
$$





# 参数估计

不是无偏估计不参与有效性比较

一致性由切比雪夫不等式证明



# 置信区间

$$
置信水平为 1 - \alpha \\
\\
对\mu估计 \\
若\sigma^2已知 \Rightarrow (\bar{X} - \frac{\sigma}{\sqrt{n}}z_\frac{\alpha}{2}, \bar{X} + \frac{\sigma}{\sqrt{n}}z_\frac{\alpha}{2})
对\mu估计 \\
若\sigma^2未知 \Rightarrow (\bar{X} - \frac{S}{\sqrt{n}}t_\frac{\alpha}{2}(n - 1), \bar{X} + \frac{S}{\sqrt{n}}t_\frac{\alpha}{2}(n - 1)) \\
\\
对\sigma^2估计 \\
若\mu已知 \Rightarrow () \\
若\mu未知 \Rightarrow (\frac{(n - 1)S^2}{\chi^2_{\frac{\alpha}{2}}}, \frac{(n - 1)S^2}{\chi^2_{1 - \frac{\alpha}{2}}})\\
\\
\\
对\mu_1 - \mu_2估计 \\
\sigma_1^2,\sigma_2^2已知 \Rightarrow  (\bar{X} - \bar{Y} - z_\frac{\alpha}{2}\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}, \bar{X} - \bar{Y} + z_\frac{\alpha}{2}\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}) \\ \\

\sigma_1^2,\sigma_2^2未知，但\sigma_1^2 = \sigma_2^2 = \sigma^2 \Rightarrow  (\bar{X} - \bar{Y} - t_\frac{\alpha}{2}(n_1 + n_2 - 2)S_w\sqrt{\frac{1}{n_1} + \frac{1}{n_2}}, \bar{X} - \bar{Y} + t_\frac{\alpha}{2}(n_1 + n_2 - 2)S_w\sqrt{\frac{1}{n_1} + \frac{1}{n_2}}) \\ \\

对\frac{\sigma_1^2}{\sigma_2^2}估计 \\ \\
\mu_1,\mu_2未知 \Rightarrow (\frac{S_1^2}{S_2^2}\frac{1}{F_{\frac{\alpha}{2}}(n_1 - 1, n_2 - 1)}, \frac{S_1^2}{S_2^2}\frac{1}{F_{1 -\frac{\alpha}{2}}(n_1 - 1, n_2 - 1)})
$$



# 两类错误



第一类错误是弃真错误

第二类错误是取伪错误





单边检验

- 右边检测
  $$
  \bar{x} \ge \mu_0 + \frac{\sigma}{\sqrt{n}}Z_\alpha \\
  z = \frac{\bar{x} - \mu_0}{\frac{\sigma}{\sqrt{n}}} \ge Z_\alpha
  $$

- 单个$\sigma$已知检测$\mu$，$Z$检验

  |                  检验                  | 检验统计量 |            拒绝域            |
  | :------------------------------------: | :--------: | :--------------------------: |
  | $H_0: \mu = \mu_0, H_1: \mu \ne \mu_0$ |    $Z$     | $|z| \ge Z_\frac{\alpha}{2}$ |
  | $H_0: \mu \le \mu_0, H_1: \mu > \mu_0$ |    $Z$     |       $z \ge Z_\alpha$       |
  | $H_0: \mu \ge \mu_0, H_1: \mu < \mu_0$ |    $Z$     |      $z \le -Z_\alpha$       |

- 单个$\sigma$未知检测$\mu$，$t$检验

  |                  检验                  | 检验统计量 |               拒绝域                |
  | :------------------------------------: | :--------: | :---------------------------------: |
  | $H_0: \mu = \mu_0, H_1: \mu \ne \mu_0$ |    $t$     | $|t| \ge t_\frac{\alpha}{2}(n - 1)$ |
  | $H_0: \mu \le \mu_0, H_1: \mu > \mu_0$ |    $t$     |       $t \ge t_\alpha(n - 1)$       |
  | $H_0: \mu \ge \mu_0, H_1: \mu < \mu_0$ |    $t$     |      $t \le -t_\alpha(n - 1)$       |

- 单个$\mu$未知检测$\sigma$

  |                        检验                        |   检验统计量    |                            拒绝域                            |
  | :------------------------------------------------: | :-------------: | :----------------------------------------------------------: |
  | $H_0: \sigma = \sigma_0, H_1: \sigma \ne \sigma_0$ | $\chi^2(n - 1)$ | $\frac{(n - 1)S^2}{\sigma_0} \le \chi^2_{1 - \frac{\alpha}{2}}(n - 1) | \frac{(n - 1)S^2}{\sigma_0} \ge \chi^2_\frac{\alpha}{2}(n - 1) $ |
  | $H_0: \sigma \le \sigma_0, H_1: \sigma > \sigma_0$ | $\chi^2(n - 1)$ |   $\frac{(n - 1)S^2}{\sigma_0} \ge \chi^2_{\alpha}(n - 1)$   |
  | $H_0: \sigma \ge \sigma_0, H_1: \sigma < \sigma_0$ | $\chi^2(n - 1)$ | $\frac{(n - 1)S^2}{\sigma_0} \le \chi^2_{1 - \alpha}(n - 1)$ |

- 两个$\sigma$相等未知检测$\mu_1 - \mu_2$

  

# 公式使用条件

拐点和驻点的判断当点存在时需要为0，不存在直接比较两边





# 三角公式

$$
sin(A + B) = sinAcosB + cosAsinB \\
sin(A - B) = sinAcosB - cosAsinB \\
cos(A + B) = cosAcosB - sinAsinB \\
cos(A - B) = cosAcosB + sinAsinB \\
tan(A + B) = \frac{tanA + tanB}{1 - tanAtanB} \\
tan(A - B) = \frac{tanA - tanB}{1 + tanAtanB} \\
cot(A + B) = \frac{cotAcotB - 1}{cotB + cotA} \\
cot(A - B) = \frac{cotAcotB + 1}{cotB - cotA} \\
\\
tan2A = \frac{2tanA}{1 - tan^2A} \\
sin2A = 2sinAcosA \\
cos2A = 2cos^2A - 1 = 1 - 2sin^2A \\
\\
sin3A = 3sinA - 4sin^3A \\
cos3A = 4cos^3A - 3cosA \\
tan3A = tanA tan(\frac{\pi}{3} + A) tan(\frac{\pi}{3} - A) \\
\\
sinA + sinB = 2sin\frac{a + b}{2}cos\frac{a - b}{2} \\
sinA - sinB = 2cos\frac{a + b}{2}sin\frac{a - b}{2} \\
cosA + cosB = 2cos\frac{a + b}{2}cos\frac{a - b}{2} \\
cosA - cosB = -2sin\frac{a + b}{2}sin\frac{a - b}{2} \\
tanA + tanB = \frac{sin(A + B)}{cosAcosB} \\
\\
sinAsinB = -\frac{1}{2}[cos(a + b) - cos(a - b)] \\
cosAcosB = \frac{1}{2}[cos(a + b) + cos(a - b)] \\
sinAcosB = \frac{1}{2}[sin(A + B) + sin(A - B)] \\
cosAsinB = \frac{1}{2}[sin(A + B) - sin(A - B)] \\
\\
sin(-A) = -sinA \\
cos(-A) = cosA \\
sin(\frac{\pi}{2} - A) = cosA \\
cos(\frac{\pi}{2} - A) = sinA \\
sin(\frac{\pi}{2} + A) = cosA \\
cos(\frac{\pi}{2} + A) = -sinA \\
sin(\pi - A) = sinA \\
cos(\pi - A) = -cosA \\
sin(\pi + A) = -sinA \\
cos(\pi + A) = -cosA \\
tan(\pi + A) = tanA \\
cot(\pi + A) = cotA \\
\\
sinA = \frac{2tan\frac{A}{2}}{1 + tan^2\frac{A}{2}} \\
cosA = \frac{1 - tan^2\frac{A}{2}}{1 + tan^2\frac{A}{2}} \\
tanA = \frac{2tan\frac{A}{2}}{1 - tan^2\frac{A}{2}} \\
\\
asinA + bcosA = \sqrt{a^2 + b^2}sin(A + B) \ (tanB = \frac{b}{a}) \\
asinA - bcosA = \sqrt{a^2 + b^2}cos(A - B) \ (tanB = \frac{a}{b}) \\
\\
arctanx = arccot\frac{1}{x} \\
arccotx = arctan\frac{1}{x} \\
arcsinx + arccosx = \frac{\pi}{2} \\
$$



# 积分公式

$$
\int \frac{dx}{1 + x^2}  = arctanx + C \\
\int \frac{dx}{\sqrt{1 - x^2}}  = arcsinx + C \\
\int sec^2x dx = tanx + C \\
\int csc^2x dx = -cotx + C \\
\int secxtanx dx = secx + C \\
\int cscxcotx dx = -cscx + C \\
\int a^x dx = \frac{a^x}{lna} + C \\
\int tanx dx = -ln|cosx| + C \\
\int cotx dx = ln|sinx| + C \\
\int secx dx = ln|secx + tanx| + C \\
\int cscx dx = ln|cscx - cotx| + C \\
\int \frac{dx}{a^2 + x^2} = \frac{1}{a}arctan\frac{x}{a} + C \\
\int \frac{dx}{x^2 - a^2} =  \frac{1}{2a}ln|\frac{a + x}{a - x}| + C \\
\int \frac{dx}{\sqrt{a^2 - x^2}} = arcsin\frac{x}{a} + C \\
\int \frac{dx}{\sqrt{x^2 + a^2}} = ln|x + \sqrt{x^2 + a^2}| + C \\ 
\int \frac{dx}{\sqrt{x^2 - a^2}} = ln|x + \sqrt{x^2 - a^2}| + C \\
\int \sqrt{a^2 - x^2} dx = \frac{1}{2}(x\sqrt{a^2 - x^2} + a^2arcsin\frac{x}{a}) + C \\
\int \sqrt{x^2 \pm a^2} dx = \frac{1}{2}(x \sqrt{x^2\pm a^2} \pm a^2ln|x + \sqrt{x^2 \pm a^2}|) + C \\
\int \frac{dx}{(a^2 + x^2)^2} = \frac{1}{2a^3}(arctax\frac{x}{a} + \frac{ax}{x^2 + a^2}) + C \\
\\
\int_0^\frac{\pi}{2}f(sinx) dx = \int_0^\frac{\pi}{2}f(cosx) dx \\
\int_0^\pi xf(sinx) dx = \frac{\pi}{2}f(sinx) dx \\
\int \sqrt{\frac{1 + x}{1 - x}} dx = -\sqrt{1 - x^2} + 2 \arctan \sqrt{\frac{1 + x}{1 - x}} + C
$$


$$
R(sinx, -cosx) = -R(sinx, cosx) \ \ => \ t = sinx \\
R(-sinx, cosx) = -R(sinx, cosx) \ \ => \ t = cosx \\
R(-sinx, -cosx) = R(sinx, cosx) \ \ => \ t = tanx \\
\\
R(sinx, cosx) = \frac{sinx}{sinx + cosx} \\
R(-sinx, -cosx) = R(sinx, cosx) \ \ => \ t = tanx \\
\int \frac{tdx}{(1 + t)(1 + t^2)} =
$$


# 级数公式

$$
\sum_{n = 1}^\infty(u_{n + 1} - u_n) 收敛 \Leftrightarrow \ \lim_{n \rightarrow \infty} u_n 存在 \\
\\
若u_n和v_n是正级数 \\
\sum_{n = 1}^\infty \frac{1}{n^p} = 
\begin{cases}
收敛, \ \ p > 1 \\
发散， \ \ p \le 1 \\
\end{cases} \\
\\
\sum_{n = 2}^\infty \frac{1}{n(lnn)^p} = 
\begin{cases}
收敛, \ \ p > 1 \\
发散， \ \ p \le 1 \\
\end{cases} \\
\\
\sum_{n = 1}^\infty (-1)^{n - 1}\frac{1}{n^p} = 
\begin{cases}
绝对收敛, \ \ p > 1 \\
条件收敛， \ \ p \le 1 \\
\end{cases} \\
\\
$$

$$
\sum_{n = 1}^\infty u_n收敛，\sum_{n = 1}^\infty|u_n|不一定收敛 \\
u_n不一定是正项 \\
u_n = (-1)^n\frac{1}{n} \\
\\ \\

\sum_{n = 1}^\infty u_n收敛，则 \begin{cases}
u_n \ge 0，\sum_{n = 1}^\infty u_n^2收敛  \qquad 存在 N，当n > N时，u_N > u_N^2 \\
u_n为任意级数，\sum_{n = 1}^\infty u_n^2 收敛性不确定 \qquad u_n = (-1)^n\frac{1}{\sqrt{n}}\\
\end{cases} \\
\\ \\

\sum_{n = 1}^\infty u_n收敛，则 \begin{cases}
u_n \ge 0，\sum_{n = 1}^\infty u_n u_{n + 1}收敛 \qquad u_n u_{n + 1} \le \frac{u_n^2 + u_{n + 1}^2}{2}\\
\\
u_n为任意级数，\sum_{n = 1}^\infty u_n u_{n + 1} 收敛性不确定 \qquad u_n = (-1)^n \frac{1}{\sqrt{n}}\\
\end{cases} \\
\\ \\

\sum_{n = 1}^\infty u_n收敛，则\sum_{n = 1}^\infty (-1)^n u_n收敛性不确定 \\
u_n = (-1)^n\frac{1}{n}
\\ \\

\sum_{n = 1}^\infty u_n收敛，则\sum_{n = 1}^\infty (-1)^n \frac{u_n}{n}收敛性不确定 \\
u_n = (-1)^n\frac{1}{lnn}
\\ \\

\sum_{n = 1}^\infty u_n收敛，则 \begin{cases}
u_n \ge 0，\sum_{n = 1}^\infty u_{2n} 和 \sum_{n = 1}^\infty u_{2n - 1}收敛 \qquad \\
\\
u_n为任意级数，\sum_{n = 1}^\infty u_{2n} 和 \sum_{n = 1}^\infty u_{2n - 1} 收敛性不确定 \qquad u_n = (-1)^n\frac{1}{n}\\
\end{cases} \\
\\ \\

\sum_{n = 1}^\infty u_n收敛，则\sum_{n = 1}^\infty (u_{2n - 1} + u_{2n})收敛 \qquad \\
\\ \\

\sum_{n = 1}^\infty u_n收敛，则\sum_{n = 1}^\infty (u_{2n - 1} - u_{2n})敛散性不确定 \\
u_n = (-1)^n \frac{1}{n}
\\ \\

\sum_{n = 1}^\infty u_n收敛，则 \begin{cases}
\sum_{n = 1}^\infty (u_n + u_{n + 1})收敛，则\sum_{n = 1}^\infty u_n + \sum_{n = 1}^\infty u_{n + 1}收敛 \\
\\
\sum_{n = 1}^\infty (u_n - u_{n + 1})收敛，则\sum_{n = 1}^\infty u_n - \sum_{n = 1}^\infty u_{n + 1}收敛 \\
\end{cases} \\
\\ \\

\sum_{n = 1}^\infty |u_n|收敛，则\sum_{n = 1}^\infty u_n收敛 \\
u_n \le |u_n|
\\ \\

\sum_{n = 1}^\infty u_n发散，\sum_{n = 1}^\infty |u_n|发散 \\
\\ \\

\sum_{n = 1}^\infty u_n^2收敛，则\sum_{n = 1}^\infty \frac{u_n}{n}绝对收敛 \\
|\frac{u_n}{n}| \le \frac{1}{2}(u_n^2 + \frac{1}{n^2})
\\ \\

a,b,c都是非零常数，且au_n + bv_n + cw_n = 0，则\sum_{n = 1}^\infty u_n,\sum_{n = 1}^\infty v_n,\sum_{n = 1}^\infty w_n中有两个收敛另一个收敛 \\
\\ \\

\sum_{n = 1}^\infty u_n和\sum_{n = 1}^\infty v_n收敛，则\sum_{n = 1}^\infty (u_n \pm v_n)收敛 \\
\\ \\

\sum_{n = 1}^\infty u_n发散，\sum_{n = 1}^\infty v_n发散，则 \begin{cases}
u_n \ge 0, v_n \ge 0，则\sum_{n = 1}^\infty (u_n + v_n)发散\\
\\
u_n,v_n任意，则\sum_{n = 1}^\infty (u_n \pm v_n) 收敛性不确定 \\
\end{cases} \\
\\ \\

\sum_{n = 1}^\infty u_n和\sum_{n = 1}^\infty v_n收敛，则\begin{cases}
u_n \ge 0, v_n \ge 0，则\sum_{n = 1}^\infty u_n v_n收敛 \qquad 存在N使n_Nv_N \le u_n\\
\\
u_n任意, v_n \ge 0，则\sum_{n = 1}^\infty |u_n| v_n收敛\\
\\
u_n,v_n任意，则\sum_{n = 1}^\infty u_n v_n 收敛性不确定 \qquad u_n = v_n = (-1)^n\frac{1}{\sqrt{n}}\\
\end{cases} \\
$$

$$
\sum_{n = 1}^\infty a_n 与 \sum_{n = 1}^\infty b_n 都发散，\sum_{n = 1}^\infty min(a_n, b_n) 不一定发散 \\
a_n = \frac{1 + (-1)^n}{2} , b_n = \frac{1 - (-1)^2}{2} \\
\\
$$

$$
e^x = \sum_{n = 0}^\infty \frac{x^n}{n!} \\ \\
\frac{1}{1 + x} = \sum_{n = 0}^\infty (-1)^nx^n \\ \\
\sin x = \sum_{n = 0}^\infty \frac{(-1)^n}{(2n + 1)!}x^{2n + 1} \\ \\
\cos x = \sum_{n = 0}^\infty \frac{(-1)^n}{(2n)!}x^{2n} \\ \\
\ln (1 + x) = \sum_{n = 1}^\infty \frac{(-1)^{n + 1}}{n}x^n \\ \\
\ln (1 - x) = -\sum_{n = 1}^\infty \frac{1}{n}x^n \\ \\
a^x = \sum_{n = 0}^\infty \frac{(x\ln a)^n}{n!} \\ \\
\arctan x = \sum_{n = 0}^\infty \frac{(-1)^n}{2n + 1}x^{2n + 1} \\ \\
(1 + x)^\alpha = 1 + \sum_{n = 1}^\infty \frac{\alpha(\alpha - 1)...(\alpha - n + 1)}{n!}x^n \\ \\
\frac{x}{(1 - x)^2} = \sum_{n = 1}^\infty nx^n
$$



# 证明

$$
数列\{x_n\}存在极限 \\
S_n = x_{n + 1} - x_n ,\ \lim_{n\rightarrow +\infty}\sum Sn = A
$$

