[TOC]



# 集合论

$$
\{A_k\} \\
A_1 \supset A_2 \supset \cdots \supset A_k \supset \cdots \Rightarrow \lim_{k \rightarrow  \infty} \{A_k\} = \bigcap_{k = 1}^\infty A_k \\
A_1 \sub A_2 \sub \cdots \sub A_k \sub \cdots \Rightarrow \lim_{k \rightarrow  \infty} \{A_k\} = \bigcup_{k = 1}^\infty A_k \\
$$



$$
B_j = \bigcup_{k = j}^\infty A_k \\
B_j \supset B_{j + 1} \\
\lim_{k \rightarrow \infty} B_k = \bigcap_{j = 1}^\infty B_j = \bigcap_{j = 1}^\infty \bigcup_{k = j}^\infty A_k \\
\overline{\lim_{k \rightarrow \infty}} A_k = \bigcap_{j = 1}^\infty \bigcup _{k = j}^\infty A_k \\
\mathop{\underline{\lim}}_{k \rightarrow \infty} A_k = \bigcup_{j = 1}^\infty \bigcap _{k = j}^\infty A_k \\
$$


$$
f(\bigcup_{a \in I} A_a) = \bigcup_{a \in I} f(A_a) \\
f(\bigcap_{a \in I} A_a) \sub \bigcap f(A_a) \\
f^{-1}(\bigcup_{a \in I} B_a) = \bigcup_{a \in I} f(B_a) \\
f^{-1}(\bigcap_{a \in I} B_a) = \bigcap_{a \in I} f(B_a) \\
$$



$$
Cantor-Bernstein:\\
X'\sub X, Y' \sub Y, X \sim Y', Y \sim X' \Rightarrow X \sim Y
$$

$$
A_i = \{x \ | \ - \frac{1}{i} < x < 1 + \frac{1}{i}\} \\
\bigcap_{n = 1}^\infty A_i = (-1, 2) \cap (-\frac{1}{2}, \frac{3}{2}) \cap \cdots = [0, 1]
$$

$$
A_{2m} = B, A_{2m + 1} = C, \overline{\lim_{n \rightarrow \infty}} A_n = B \cup C
$$

$$
A_n = [\frac{1}{n}, 1 - \frac{1}{n}], \lim_{n \rightarrow \infty} A_n = (0, 1)
$$


$$
单射: x\ne y \Rightarrow \phi(x) \ne \phi(y) \\
满射: \forall y \in B , \exist x \in A, \Rightarrow y = \phi(x)
$$

$$
对等(等势): A,B两个集合存在一一映射, A \sim B \\
\phi\sim\phi
$$



$$
有限集: A \sim \{1, 2, \cdots n\} , n < +\infty \\
$$



$$
\mathbb{Z} \sim \{\pm1, \pm3, \pm5, \cdots \} \\
\phi: n \mapsto 2n + 1
$$

$$
无限集与它的一个真子集等势
$$

$$
基数: \bar{\bar{A}}
$$

$$
伯恩斯坦定理: \bar{\bar{A}} \le \bar{\bar{B}}, \bar{\bar{A}} \ge \bar{\bar{B}} \Rightarrow \bar{\bar{A}} = \bar{\bar{B}}
$$

$$
(0, 1) \sim (0, 1] \\
\\
\phi_1: x \mapsto x , (0, 1) \mapsto (0, 1) \subset (0, 1] \\
\bar{\bar{A}} \le \bar{\bar{B}} \\
\\
\phi_2: x \mapsto \frac{x}{2} , \ (0, 1] \mapsto (0, \frac{1}{2}] \subset (0, 1) \\
\bar{\bar{B}} \le \bar{\bar{A}} \\
\\
\bar{\bar{A}} = \bar{\bar{B}} \\
(0, 1) \sim (0, 1]
$$



$$
可数集合: A \sim \mathbb{Z}_+
$$

$$
任何无限集都至少包含一个可数集，可数集合是最小的无限集合
$$

$$
可数集的任何无限集都是可数集
$$

$$
至多可数集的并仍然是至多可数集
$$


$$
有限个至多可数集的直积仍然是至多可数集
$$


$$
集合M的幂集记为2^M,有\bar{\bar{2^M}} > \bar{\bar{M}}
$$

$$
A_i = \{\frac{1}{i}, \frac{2}{i}, \cdots  \}是至多可数集 \\
\phi: x \mapsto ix \\
A_i \mapsto \mathbb{Z}_+ \\
$$

$$
广义距离: \\
\forall x, y \in X , \ d(x, y) \ge 0 \\
\forall x, y \in X, \ d(x, y) = d(y , x) \\
\forall x, y, z \in X, \ d(x, z) + d(y, z) \ge d(x, y) \\
(X, d)称为度量空间
$$






$$
\{A_n\}是集合列, B_1 = A_1, B_n = A_n - \bigcup_{i = 1}^{n - 1}A_i,证明\{B_n\}互不相交,且\bigcup_{i = 1}^nA_i = \bigcup_{i = 1}^nB_i \\
\\
\forall j, k , B_j = A_j - \bigcup_{i = 1}^{j - 1}A_i, B_k = A_k - \bigcup_{i = 1}^{k - 1}A_i \\
若B_j与B_k相交,则\exists x, x \in B_j , x \in B_k \\
x \in A_j , x \in A_k \\
设j < k \\
\because A_j \subset \bigcup_{i = 1}^{k - 1}A_i \\
\therefore x \in \bigcup_{i = 1}^{k - 1}A_i \Rightarrow x \notin B_k
$$

$$
\{x \ | \ f(x) > g(x)\} = \bigcup_{n = 1}^\infty \{x \ | \ f(x) > g(x) + \frac{1}{n}\} \\
\\
\{\{x \ | \ f(x) > g(x) + \frac{1}{n}\}\}是递增的集合列 \\
\therefore \lim_{n \rightarrow \infty}\{x \ | \ f(x) > g(x) + \frac{1}{n}\} \subset \{x \ | \ f(x) > g(x)\} \\
???
$$

$$
f_n(x) \le f_{n + 1}(x) , \forall x \in E , A_n = \{x \ | \ f_n(x) > C\}是递增的, 且\lim_{n \rightarrow \infty} A_n = \{x\ | \lim_{n \rightarrow \infty} f_n(x) > C\} \\
\\
\lim_{n \rightarrow \infty} A_n = \bigcup_{n = 1}^\infty A_n = \{x \ | \ \sup\{f_n(x)\} > C\} = \{x \ | \ \lim_{n \rightarrow \infty} f_n(x) > C\}
$$





# 测度论

$$
外侧度: \\
E \subset \mathbb{R}^n, m^*(E) = \inf\{\sum_{i = 1}^\infty |I_i| : E \subset \bigcup_{i = 1}^\infty I_i \} , \{I_i\}的个数是可数的
$$

$$
P = \{P_1, \cdots , P_n\}, n < \infty \\
I_i = (x_i - \epsilon, x_i + \epsilon)\\
\{P_i\} \subset I_i \\
m^*(\{P_i\}) \le \epsilon \\
m^*(\{P_i\}) = 0 \\
m^*(P) = \sum_{i = 1}^n m^*(\{P_i\}) = 0
$$


$$
S可测，S^c可测
$$






$$
m^*(\mathbb{Z_+}) = 0 \\
I_i = (i - \frac{\epsilon}{2^{i + 1}}, i + \frac{\epsilon}{2^{i + 1}}) \\
|I_i| = \frac{\epsilon}{2^i} \\
\mathbb{Z}_+ \subset \bigcup_{i = 1}^\infty I_i \\
\sum_{i = 1}^\infty |I_i| = \epsilon \frac{\frac{1}{2}}{1 - \frac{1}{2}} = \epsilon \\
0 \le m^*(\mathbb{Z}_+) \le \epsilon \\
$$




# 可测函数

$$
有限函数:\\
f: E \mapsto \mathbb{R}
$$


$$
可测函数: \\
f: E \mapsto \mathbb{R} \cup \{- \infty, +\infty\} 且 \forall x \in E , f(x) > a\\
f(x) > a 记为 E[f > a]
$$

$$
可测充要条件: \\
1. E[f \le a] \\
2. E[f > a] = \bigcap_{n = 1}^\infty E[f > a - \frac{1}{n}]
$$

$$
f: E \mapsto \mathbb{R} \cup \{-\infty, +\infty\}是常值函数， f \equiv C \\
\forall a \in \mathbb{R}, E[g > a] = 
\left \{
\begin{matrix}
E, \quad a < C\\
\phi, \quad  a \ge C\\
\end{matrix}
\right. \
是可测的 \\
\therefore f是可测的
$$




$$
f可测则f + C , C\cdot f, \frac{f}{C} 可测
$$

$$
f, g可测则 f + g, f - g, f \cdot g, \frac{f}{g} 可测
$$

$$
[a, b]上单调的函数是可测函数\\
\\
设f(x)是单调递增的\\
\forall C \in \mathbb{R}, 若E[f \ge C] = \empty \\
???
$$




$$
逐点收敛: \{f_k\}是定义在E上的函数， \forall x \in E , \lim_{k\rightarrow \infty}f_k(x) = f(x), 则\{f_k\}是逐点收敛于f
$$
