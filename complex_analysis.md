[TOC]



# 复数运算


$$
z = x + yi  \\
z = r(\cos\theta + i\sin\theta), r = |z| = \sqrt{x^2 + y^2}, \tan \theta = \frac{y}{x} \\
z = re^{i\theta}
$$

$$
z = x + yi \\
\bar{z} = x - yi \\
Re(z) = x \\
Im(z) = y
$$

$$
z_1 + z_2 = (x_1 + x_2) + (y_1 + y_2)i \\
z_1 - z_2 = (x_1 - x_2) + (y_1 - y_2)i \\
z_1z_2 = (x_1x_2 - y_1y_2) + (x_1y_2 + x_2y_1)i \\
\frac{z_1}{z_2} = \frac{(x_1 x_2 + y_1 y_2) + (x_2 y_1 - x_1 y_2)i}{x_2^2 + y_2^2}
$$

$$
z_1z_2 = r_1r_2e^{i(\theta_1 + \theta_2)} \\
\frac{z_1}{z_2} = \frac{r_1}{r_2}e^{i(\theta_1 - \theta_2)}
$$

$$
z^n = e^{in\theta} = \cos n\theta + i\sin n\theta
$$

$$
\sqrt[^n]{z} = \sqrt[^n]re^{i\frac{\theta + 2k\pi}{n}}
$$




$$
z = \frac{1 - \sqrt{3}i}{2},求|z|, Arg z \\
|z| = \sqrt{(\frac{1}{2})^2 + (-\frac{\sqrt{3}}{2})^2} = 1 \\
Arg z = \arctan \frac{-\frac{\sqrt{3}}{2}}{\frac{1}{2}} + 2k\pi = -\frac{\pi}{3} + 2k\pi, k\in\mathbb{Z}
$$



$$
z_1 = \frac{1 + i}{\sqrt{2}}, z_2 = \sqrt{3} - i,用指数形式表示z_1 z_2, \frac{z_1}{z_2} \\
z_1 = e^{\frac{\pi}{4}i} \\
z_2 = 2e^{-\frac{\pi}{6}i} \\
z_1 z_2  =2e^{\frac{\pi}{12}i} \\
\frac{z_1}{z_2} = \frac{1}{2}e^{\frac{5\pi}{12}i}
$$



$$
证明 \ |z_1 + z_2|^2 + |z_1 - z_2|^2 = 2(|z_1|^2 + |z_2|^2) \\
z\bar{z} = |z|^2 \\
|z_1 + z_2|^2 = (z_1 + z_2)(\bar{z_1} + \bar{z_2}) = |z_1|^2 + |z_2|^2 + z_1\bar{z_2} + \bar{z_1}z_2 \\
|z_1 - z_2|^2 = (z_1 - z_2)(\bar{z_1} - \bar{z_2}) = |z_1|^2 + |z_2|^2 - z_1\bar{z_2} - \bar{z_1}z_2 \\
$$



$$
证明: z平面上的直线方程可以写为 \quad a\bar{z} + \bar{a}z = c \\
a = a_1 + a_2i \\
z = z_1 + z_2 i \\
a\bar{z} + \bar{a}z = (a_1 + a_2i)(z_1 - z_2i) + (a_1 - a_2i)(z_1 + z_2i) = 2a_1z_1 + 2a_2z_2 = c \\
l:2a_1z_1 + 2a_2z_2 = c是在平面z_1Oz_2上的直线
$$



$$
将z = \frac{(\cos 5\phi + i\sin 5\phi)^2}{(\cos 3\phi - i\sin 3\phi)^3}化成指数形式和三角形式 \\
z = \frac{e^{10\phi i}}{e^{-9\phi i}} = e^{19\phi i} = \cos 19\phi + i\sin 19\phi 
$$



$$
z = e^{it}, \ 证明\ z^n + \frac{1}{z^n} = 2\cos nt, \ z^n - \frac{1}{z^n} = 2i\sin nt \\
z = \cos t + i\sin t \\
z^n = \cos nt + i\sin nt \\
z^{-n} = \cos nt - i\sin nt \\
$$

$$
x_n + iy_n = (1 - i\sqrt{3})^n, \ 证明\ x_n y_{n - 1} - x_{n - 1} y_n = 4^{n - 1}\sqrt{3} \\
(1 - \sqrt{3}i) = 2e^{-\frac{\pi}{3}i} = 2(\cos \frac{\pi}{3} - i\sin \frac{\pi}{3}) \\
x_n + y_n i = 2^n\cos \frac{n\pi}{3} - 2^ni\sin\frac{n\pi}{3} \\
x_n = 2^n \cos \frac{n\pi}{3} \\
y_n = -2^n \sin \frac{n\pi}{3}
$$






# 解析函数


$$
f(z) = u(x, y) + v(x, y)i \\
\lim_{z \rightarrow z_0}f(z) - f(z_0) = \lim_{z \rightarrow z_0}(u(x,y) - u(x_0, y_0)) + \lim_{z \rightarrow z_0} (v(x, y) - v(x_0, y_0))i \\
\lim_{z \rightarrow z_0} f(z) - f(z_0) = 0 \Leftrightarrow u(x,y), v(x,y)连续
$$

$$
f'(z) = \lim_{\Delta z \rightarrow 0}\frac{f(z + \Delta z) - f(z)}{\Delta z} = \lim_{\Delta z \rightarrow 0}\frac{(u(x + \Delta x, y + \Delta y) - u(x, y)) + (v(x + \Delta x, y + \Delta y) - v(x, y))i}{\Delta z} = \phi(z) + \psi(z)i \\
\\
\lim_{\Delta z \rightarrow 0}\frac{\Delta u \bar{z} + \Delta v \bar{z}i}{|\Delta z|^2} = \lim_{\Delta x \rightarrow 0 , \Delta y \rightarrow0} \frac{(\Delta u \Delta x + \Delta v \Delta y) + (\Delta v \Delta x - \Delta u \Delta y)i}{(\Delta x)^2 + (\Delta y)^2} = \frac{u_x(\Delta x)^2 + v_y(\Delta y)^2 + v_x(\Delta x)^2 - u_y(\Delta y)^2}{r^2} = \\ \frac{(\Delta x)^2(u_x + v_x) + (\Delta y)^2(v_y - u_y)}{r^2} \\
\\
\left \{
\begin{matrix}
	\frac{\part u}{\part x} = -\frac{\part v}{\part x} \\
	\frac{\part u}{\part y} = \frac{\part v}{\part y} \\
\end{matrix}
\right.
\\\\
u_x = v_y \\
u_y = -v_x \\
f'(z) = \frac{\part u}{\part x} + i\frac{\part v}{\part x} = \frac{\part u}{\part y} - i\frac{\part v}{\part y}
$$

$$
f(z) = e^z = e^x(\cos y + i\sin y) = e^{x + iy} \\
\\
\lim_{\Delta z \rightarrow 0}f(z + \Delta z) - f(z) = 0 \\
\\
u(x, y) = e^x\cos y, \ v(x, y) = e^x\sin y \\
\\
\frac{\part u}{\part x} = e^x \cos y , \ \frac{\part u}{\part y} = -e^x \sin y, \ \frac{\part v}{\part x} = e^x \sin y, \ \frac{\part v}{\part y} = e^x \cos y \\
\frac{\part u}{\part x} = \frac{\part v}{\part y}, \ \frac{\part u}{\part y} = - \frac{\part v}{\part x} \\
f'(z) = e^x\cos y + ie^x\sin y = f(z) \\
f(z + 2k\pi i) = f(z)
$$


$$
\sin z = \frac{e^{iz} - e^{-iz}}{2i}, \ \cos z = \frac{e^{iz} + e^{-iz}}{2} \\
\\
(\sin z)' = \cos z , \ (\cos z)' = -\sin z \\
\\
\sin (-z) = -\sin z, \ \cos (-z) = \cos z \\
\\
\sin(z + 2\pi) = \frac{e^{i(z + 2\pi)} - e^{-i(z + 2\pi)}}{2i} = \sin z \\
\cos(z + 2\pi) = \cos z \\
$$

$$
\sinh z = \frac{e^z - e^{-z}}{2}, \ \cosh z = \frac{e^z + e^{-z}}{2}
$$


$$
w =Ln z = x + yi\\
z = e^{Ln z} = e^w = e^{x + yi} = e^x(\cos y + i\sin y) = e^{w + 2k\pi i} = e^x e^{(y + 2k\pi)i}\\
x = \ln|z| \\
y = Arg z \\
Ln z = \ln|z| + iArg z = \ln |z| + i\arg z + 2k\pi i \\
\\
Ln(z_1 z_2) = Lnz_1 + Ln z_2 \\
Ln\frac{z_1}{z_2} = Lnz_1 - Ln z_2 \\
\\
(Ln z)' = \frac{1}{z} \\
$$



$$
w = \sqrt[^n]{z} \\
z = x + yi = |z| e^{iArgz} \\
\sqrt[^n]{z} = \sqrt[^n]{|z|} e^{\frac{iArg z}{n}} = \sqrt[^n]{|z|} e^{\frac{i\arg z}{n} + \frac{2k\pi}{n}} ,\quad k = 0,\cdots,n - 1 \\
\\
(\sqrt[^n] z) ' = \frac{1}{n}\frac{\sqrt[^n]z}{z} \\
 
$$

$$
f(z) = z^a \\
z = x + yi \\
z^a = (|z|e^{i(\arg z + 2k \pi)})^a
$$






$$
解方程 \ z^4 + a^4 = 0 \ (a > 0)\\
z = \sqrt[^4]{a^4 (-1)} = a\sqrt[^4]{-1} = a\sqrt[^4]{\cos \pi + i\sin\pi} = a\sqrt[^4]{e^{(\pi + 2k\pi)i}} = ae^{\frac{\pi + 2kpi}{4}}, \ k = 0, 1, 2, 3
$$



$$
f(z) = \frac{1}{1 - z}在|z| < 1 内是否连续, 是否一致连续 \\
\lim_{\Delta z \rightarrow 0} (\frac{1}{1 - (z + \Delta z)} - \frac{1}{1 -z}) = \frac{\Delta z}{1 - 2z+ z^2 - \Delta z + z \Delta z} = 0
$$



$$
若f(z), g(z)在z_0解析，且满足f(z_0) = g(z_0) = 0, g'(z_0) \ne 0, 证明\lim_{z \rightarrow z_0} \frac{f(z)}{g(z)} = \lim_{z\rightarrow z_0} \frac{f'(z)}{g'(z)} \\
\lim_{z \rightarrow z_0} \frac{f(z)}{g(z)} = \lim_{z \rightarrow z_0} \frac{(f(z) - f(z_0))(z - z_0)}{(g(z) - g(z_0))(z - z_0)} = \lim_{z\rightarrow z_0} \frac{f'(z)}{g'(z)}
$$



$$
f(z) = 
\left \{
\begin{matrix}
\frac{x^3 - y^3 + i(x^3 + y^3)}{x^2 + y^2}, \quad z \ne 0 \\
0, \quad z = 0
\end{matrix}
\right.
在原点满足柯西-黎曼方程但不可微 \\
当沿着实轴趋于原点 \quad u_x + iv_x = \lim_{x \rightarrow 0} \frac{x + ix}{x} = 1 + i\\
当沿着虚轴趋于原点 \quad v_y - iu_y = \lim_{y \rightarrow 0} \frac{-y + iy}{yi} = 1 + i\\
y = mx \\
\lim_{z \rightarrow 0}\frac{f(z) - f(0)}{z - 0} = \frac{1 - m^3 + i(1 + m^3)}{(1 + m^2)(1 + im)}
$$

$$
f(z) = xy^2 + ix^2y的可微性和解析性 \\
u = xy^2 , \ v = x^2 y \\
u_x = y^2, \ u_y = 2xy \\
v_x = 2xy, \ v_y = x^2 \\
u_x = v_y \Rightarrow y = \pm x \\
u_y = -v_x \Rightarrow x = y = 0 \\
f只在(0, 0)可微，(0, 0)不是区域，f在平面内处处不解析\\
$$



$$
f(z)D内解析,证明满足下列条件之一则f(z)在D内是常数: (1)f'(z) = 0\quad (2)\overline{f(z)}在D内解析 \quad (3)|f(z)|为常数 \quad (4)Ref(z)是常数 \quad (5) Imf(z) 是常数 \\
f(z) = u + vi \\
u_x = v_y , \ u_y = - v_x \\
f'(z) = u_x + v_x i = u_y - v_y i = 0 \Rightarrow u_x = u_y = v_x = v_y = 0 \Rightarrow f(z) = C \\
\overline{f(z)} = u - vi = u + v'i\\
u_x = v'_y = -v_y \\
|f(z)| \Rightarrow \overline{f(z)} = \frac{C^2}{f(z)}
$$







# 复积分

$$
z = z(t) = x(t) + iy(t) \\
f(z) = u(x, y) + iv(x, y) \\
\int_C f(z) dz = \int_C (u + iv)(dx + idy) = \int_C udx -vdy + i\int_Cvdx + udy = \int_Cf(z(t))z'(t) dt
$$


$$
\int_C f(z) dz = \int_C udx -vdy + i\int_Cvdx + udy = \oint_D -v_x - u_y dxdy + i\oint_D u_x - v_y dxdy = 0
$$

$$
\int_C \frac{d z}{(z - z_0)^n} = 
\left \{
\begin{matrix}
\begin{aligned}
& 2\pi i, \ &n = 1 \\
& 0, \ &n \in \mathbb{Z}_+ / \{1\} 
\end{aligned}
\end{matrix}
\right .
\\
\\
$$

$$
\lim_{r \rightarrow 0} \int_{|z - z_0| = r} \frac{f(z)}{z - z_0} d z = 2\pi if(z_0)
$$

$$
f(z_0) = \frac{1}{2\pi i} \int_C \frac{f(z)}{z - z_0} dz
$$

$$
f^{(n)}(z_0) = \frac{n!}{2\pi i} \int_C \frac{f(z)}{(z - z_0)^{n + 1}} dz
$$














$$
\int_C \frac{2z^2 - z + 1}{z - 1} dz , \ \int_C \frac{2z^2 - z + 1}{(z - 1)^2} dz  \quad C: |z| = 2 \\
f(z) = 2z^2 - z + 1 \\
\int_C \frac{2z^2 - z + 1}{z - 1} dz = \int_C \frac{f(z)}{(z - 1)^1}dz = 2\pi i f(1) = 4 \pi i \\
\int_C \frac{2z^2 - z + 1}{(z - 1)^2} dz = \frac{2\pi i}{1 !}f'(1) = 6 \pi i
$$





$$
\int_{C_i} \frac{\sin \frac{\pi}{4} z}{z^2 - 1} dz , \quad C_1: |z + 1| = \frac{1}{2}, \ C_2: |z - 1| = \frac{1}{2}, \ C_3 : |z| = 2 \\
\int_{C_1} \frac{\sin \frac{\pi}{4} z}{z^2 - 1} dz = \int_{C_1} \frac{\sin \frac{\pi}{4}z}{z - 1} \frac{1}{z + 1} dz = \frac{\sqrt{2}}{2} \pi i   \\
\int_{C_2} \frac{\sin \frac{\pi}{4} z}{z^2 - 1} dz = \int_{C_2} \frac{\sin \frac{\pi}{4}z}{z + 1} \frac{1}{z - 1} dz = \frac{\sqrt 2}{2}\pi i \\
\int_{C_3} \frac{\sin \frac{\pi}{4} z}{z^2 - 1} dz = \sqrt 2 \pi i 
$$



$$
求\int_{|z| = 1}\frac{e^z}{z} dz , \ 证明 \int_0^\pi e^{\cos \theta }\cos (\sin \theta) d \theta = \pi \\
\int_{|z| = 1}\frac{e^z}{z} dz = 2\pi i \\
\int_{|z| = 1}\frac{e^z}{z} dz = \int_{-\pi}^{\pi} \frac{e^{\cos \theta + i\sin \theta}}{\cos \theta + i\sin \theta} (- \sin \theta + i\sin \theta) d \theta = -\int_{-\pi}^{\pi}e^{\cos \theta}\sin(\sin\theta) d\theta + i\int_{-\pi}^{\pi}e^{\cos \theta} \cos (\sin \theta) d \theta = 0 + 2i\int_0^\pi e^{\cos \theta} \cos(\sin \theta)d\theta
$$


$$
C: x^2 + y^2 = 3, \ f(z) = \int_C \frac{3\zeta^2 + 7\zeta + 1}{\zeta - z} d\zeta, \ 求f'(1 + i) \\
|z| \ge \sqrt 3, f(z) = 0 \\
|z| < \sqrt 3 , f(z) = (3z^2 + 7z + 1)2\pi i
$$
 




# 复级数

$$
\lim_{n \rightarrow \infty} z_n = z_0 \Leftrightarrow \lim_{n \rightarrow \infty} x_n = x_0, \lim_{n \rightarrow \infty} y'_n = y_0
$$




$$
\lim_{n \rightarrow \infty} z_n = z_0 \ne \infty \Rightarrow \lim_{n \rightarrow \infty} \frac{z_1 + \cdots z_n}{n} = z_0 \\
\\
\lim_{n \rightarrow \infty} (\frac{z_1 + \cdots + z_m}{n} + \frac{z_{m + 1} + \cdots + z_n}{n}) < \lim_{n \rightarrow \infty} \frac{n - m - 1}{n}z_0 + \lim_{n \rightarrow \infty} \frac{n - m - 1}{n}\epsilon = z_0
$$



$$
f(z) = \sum_{n = -\infty}^\infty c_n (z - z_0)^n \\
c_n = \frac{1}{2\pi i} \int_C \frac{f(z)}{(z - z_0)^{n + 1}} dz
$$






$$
判断敛散性: 1. \sum_{n = 1}^\infty \frac{i^n}{n}; \quad 2.\sum_{n = 1}^\infty \frac{(3 + 5i)^n}{n!}; \quad 3.\sum_{n = 1}^\infty (\frac{1 + 5i}{2})^n; \\
 \sum_{n = 1}^\infty \frac{i^n}{n} = \sum_{n = 1}^\infty \frac{(-1)^n}{2n} + i\sum_{n = 1}^\infty\frac{(-1)^{n - 1}}{2n - 1} \\
 \sum_{n = 1}^\infty \frac{(3 + 5i)^n}{n!} < \sum_{n = 1}^\infty \frac{6^n}{n!}
$$

$$
\sum_{n = 1}^\infty \frac{z^n}{n}的收敛半径 \\
c_n = \frac{1}{n} \\
\lim_{n \rightarrow \infty}|\frac{c_{n + 1}}{c_n}| = 1 , \ R = 1
$$

$$
\frac{1}{az + b} = \frac{1}{b} \frac{1}{\frac{a}{b}z + 1} = \frac{1}{b}\sum_{n = 0}^\infty (-1)^n (\frac{az}{b})^n , \ (|z| < \frac{|b|}{|a|})
$$

$$
\frac{z + 1}{z^2(z - 1)}, \ 0 < |z| < 1, \ 1 < |z| < +\infty 展为洛朗级数 \\
0 < |z| < 1 , \ \frac{z + 1}{z^2(z - 1)} = - \frac{z + 1}{z^2} \frac{1}{1 - z} = -(\frac{1}{z} + \frac{1}{z^2})\sum_{n = 0}^\infty z^n  \\
1 < |z| < +\infty, \ |\frac{1}{z}| < 1 \\
\frac{z + 1}{z^2(z - 1)} = \frac{z + 1}{z^3} \frac{1}{1 - \frac{1}{z}} = (\frac{1}{z^2} + \frac{1}{z^3})\sum_{n = 0}^\infty (\frac{1}{z})^n
$$

$$
\frac{1}{(z^2 + 1)^2}, \ z = i \\
z = \pm i 是奇点,它们的距离是2，z = i的收敛范围内不能包含另一个奇点 \\
收敛范围是0 < |z - i| < 2或者 0 < |\frac{z - i}{2i}| < 1 \\
\frac{1}{(z^2 + 1)^2} = \frac{1}{(z - i)^2}(\frac{1}{z + i})^2 = \frac{1}{(z - i)^2}(\frac{1}{z - i + 2i})^2 = -\frac{1}{4}\frac{1}{(z - i)^2}(\frac{1}{1 + \frac{z - i}{2i}})^2 = -\frac{1}{4(z - i)^2}[\sum_{n = 0}^\infty (-1)^n (\frac{z - i}{2i})^2]^2
$$
 



# 留数



可去奇点
$$
f(z) = \sum_{n = 1}^{\infty}c_{-n}(z - z_0)^{-n} + \sum_{n = 0}^\infty c_n(z - z_0)^n \\
\sum_{n = 1}^{\infty}c_{-n}(z - z_0)^{-n} = 0 \\
\lim_{z \rightarrow z_0} f(z) = A \ne \infty
$$


极点
$$
f(z) = \sum_{n = 1}^{\infty}c_{-n}(z - z_0)^{-n} + \sum_{n = 0}^\infty c_n(z - z_0)^n \\
f(z) = \sum_{n = 1}^mc_{-n}(z - z_0)^{-n} \\
f(z) = \frac{\lambda(z)}{(z - z_0)^m} \\
\lim_{z \rightarrow z_0} f(z) = \infty
$$


本性奇点
$$
\lim_{z \rightarrow z_0}f(z) \ne C \ne \infty \\
$$



$$
\mathop{\text{Res}}_{z \rightarrow z_0} f(z) = \frac{1}{2\pi i} \int_C f(z) dz = c_{-1}\\
$$

$$
\int_C f(z) dz = 2\pi i\sum_{k = 1}^n \mathop{\text{Res}}_{z \rightarrow z_k} f(z)
$$
可去奇点留数
$$
\mathop{\text{Res}}_{z \rightarrow z_0} f(z) = 0
$$


极点留数
$$
f(Z) = \frac{\phi(z)}{(z - z_0)^m}\\
\mathop{\text{Res}}_{z \rightarrow z_0} f(z) = \lim_{z \rightarrow z_0} \frac{1}{(m - 1)!}[(z - z_0)^m f(z)]^{(m - 1)}
$$




$$

$$

$$
求\frac{z}{(z - 1)(z + 1)^2}在z = \pm1, \infty处的留数 \\
z = 1 是一阶极点\\
\mathop{\text{Res}}_{z = 1} f(z) = \lim_{z \rightarrow 1} (z - 1) f(z) = \frac{1}{4} \\
z = -1 是二阶极点 \\
\mathop{\text{Res}}_{z = -1} f(z) = \lim_{z \rightarrow -1}(z + 1)^2f(z) = -\frac{1}{4} \\
\mathop{\text{Res}}_{z = \infty} f(z) = \mathop{\text{Res}}_{z = 1} f(z) + \mathop{\text{Res}}_{z = -1} f(z)
$$






# 共型映射


$$
保域定理：w = f(z)在区域D内解析且不恒为常数，则G=f(D)也是域 \\
\\
$$

$$
保角性: w = f(z), \arg \phi = \arg f'(z) 
$$

$$
|f'(z)|
$$



$$
w = \frac{az + b}{cz + d} \\
\begin{vmatrix}
a \ b \\
c \ d 
\end{vmatrix}
\ne 0\\
z = \frac{-dw + b}{cw - a}
$$



$$
w = kz + h = \rho e^{i\alpha}z + h \\
w_1 = \rho e^{i\alpha}z \\
$$

$$
w = \frac{1}{z}
$$


$$
Az\bar{z} + \bar{\beta}z + \beta\bar{z} + C = 0 \\
A = 0是直线 \\
A \ne 0 是圆
$$


# 调和函数

$$
u_{xx} + u_{yy} = 0
$$


$$
若f = u + vi 解析u, v是调和函数 \\
\\
u_x = v_y, u_y = -v_x \\
u_{xx} = v_{yx}  = -u_{yy}\\
v_{yy} = u_{xy} = -v_{xx}\\
$$

$$
f = u + vi 且解析, 求v \\
\\
dv = v_x d + v_y dy  = -u_y dx + u_x dy \\
v = \int^{(x , y)}_{(x_0, y_0)} dv + C = \int^{(x , y)}_{(x_0, y_0)}-u_y dx + u_x dy + C = 
$$

$$
u = y^3 + 3x^2 y \\
\\
u_x = 6xy \\
u_{xx} = 6y \\
u_y = 3y^2 + 3x^2 \\
\\
v = -3\int_{x_0}^{x} x^2 + y^2 dx + 6x\int_{y_0}^{y} y dy = -x^3 - 3xy^2 + C
$$



# 解析延拓

$$
解析延拓是唯一的 \\
D \subset G,在D上存在函数f(z),若在G中存在f的解析延拓后的函数F_1 和F_2 \\
由解析函数内部唯一性定理在G上F_1和F_2相等
$$


$$
\sum_{n = 0}^\infty z^n = f(z) \ (D: |z| < 1) \\
当|z| < 1则级数收敛，否则不收敛 \\
F(z) = \frac{1}{1 - z}是出去在z = 1外的解析延拓
$$


$$
在单位元|z| < 1内的解析函数f(z) = \sum_{n = 1}^\infty z^{2^n}不能延拓到|z| = 1的外部 \\
\\
级数的收敛半径为R = 1, 在单位元|z| < 1内f(z)是唯一解析函数 \\
\lim_{z \rightarrow 1} f(z) = \infty
$$
