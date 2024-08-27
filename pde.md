[TOC]

# 波动方程

$$
Dirichlet
\left \{
\begin{matrix}
\begin{aligned}
& \frac{\part^2 u}{\part t^2} = a^2\frac{\part^2 u}{\part x^2} \\
& u|_{x = 0} = 0, u|_{x = l} = 0 \\
& u|_{t = 0} = \phi(x), u_t|_{t = 0} = \psi(x) \\ 
& 0 < x < l,\ t > 0
\end{aligned}
\end{matrix}
\right.
\\
\\
u(t, x) = T(t)X(x) \\
u_{tt} = T''X \\
u_{xx} = TX'' \\
T''X = a TX'' \\
\frac{X''}{X} = \frac{T''}{a^2T} = -\lambda \\
\left \{
\begin{matrix}
\begin{aligned}
&X'' + \lambda X = 0 \\
&T'' + \lambda a^2 T = 0 
\end{aligned}
\end{matrix}
\right.
\\
\\
\lambda < 0 \\
X(x) = C_1 e^{-x\sqrt{-\lambda}} + C_2 e^{x\sqrt{-\lambda}} \\
T(t) = C_1' e^{-xa\sqrt{-\lambda}} + C_2' e^{xa\sqrt{-\lambda}} \\
u|_{x = 0} = 0 \Rightarrow C_1 = -C_2 = C \\
u|_{x = l} = 0 \Rightarrow C(e^{-l\sqrt{-\lambda}} + e^{l\sqrt{-\lambda}}) = 0 \\
\therefore C = 0, \ X(x) = 0, u(x, y) = 0 \\
\\
\lambda = 0 \\
X(x) = C_1x + C_2 \\
T(t) = C_1't + C_2' \\
u|_{x = 0} = 0 \Rightarrow C_2 = 0 \\
u|_{x = l} = 0 \Rightarrow C_1 = 0 \\
X(x) = 0, \ u(x, y) = 0 \\
\\
\lambda > 0 \\
X(x) = C_1 \sin x\sqrt{\lambda} + C_2 \cos x\sqrt{\lambda} \\
u|_{x = 0} = 0 \Rightarrow C_2 = 0 \\
u|_{x = l} = 0 \Rightarrow C_1 \sin l\sqrt{\lambda} = 0 \Rightarrow l\sqrt{\lambda} = n\pi \Rightarrow \lambda_n = \frac{n^2\pi^2}{l^2}, \ n = 0, \pm1, \cdots \\
\left \{
\begin{matrix}
\begin{aligned}
&X(x) = C_1 \sin \frac{n\pi x}{l} \\
&T(t) = C_1' \sin \frac{an\pi t}{l} + C_2' \cos \frac{an \pi t}{l} \\ 
&n = 1, 2, \cdots \\
\end{aligned}
\end{matrix}
\right.
\\
u_n(x, y) = (C_n \sin \frac{an\pi t}{l} + D_n \cos \frac{an \pi t}{l}) \sin \frac{n\pi x}{l} \\
\\
u(x, y) = \sum_{n = 1}^{\infty} (C_n \sin \frac{an\pi t}{l} + D_n \cos \frac{an \pi t}{l}) \sin \frac{n\pi x}{l} \\
u(x, 0) = \phi(x) = \sum_{n = 1}^{\infty} D_n \sin \frac{n\pi x}{l}  \Rightarrow D_n = \frac{2}{l} \int_0^l \phi(x) \sin \frac{n \pi x}{l} dx\\
u_t(x, 0) = \psi(x) = \sum_{n = 1}^{\infty} C_n \frac{an \pi}{l} \sin \frac{n \pi x}{l} \Rightarrow C_n = \frac{2}{an\pi} \int_0^l \psi(x) \sin \frac{n\pi x}{l} dx\\
$$






$$
Neumann
\left \{
\begin{matrix}
\begin{aligned}
& \frac{\part^2 u}{\part t^2} = a^2\frac{\part^2 u}{\part x^2} \\
& u|_{x = 0} = 0, u_x|_{x = l} = 0 \\
& u|_{t = 0} = \phi(x), u_t|_{t = 0} = \psi(x) \\ 
& 0 < x < l,\ t > 0
\end{aligned}
\end{matrix}
\right.
\\
\\
u(t, x) = T(t)X(x) \\
u_{tt} = T''X \\
u_{xx} = TX'' \\
T''X = a TX'' \\
\frac{X''}{X} = \frac{T''}{a^2T} = -\lambda \\
\left \{
\begin{matrix}
\begin{aligned}
&X'' + \lambda X = 0 \\
&T'' + \lambda a^2 T = 0 
\end{aligned}
\end{matrix}
\right.
\\
\\
\lambda < 0 \\
X(x) = C_1 e^{-x\sqrt{-\lambda}} + C_2 e^{x\sqrt{-\lambda}} \\
T(t) = C_1' e^{-xa\sqrt{-\lambda}} + C_2' e^{xa\sqrt{-\lambda}} \\
u|_{x = 0} = 0 \Rightarrow C_1 = -C_2 = C \\
u_x|_{x = l} = 0 \Rightarrow C(-\sqrt{\lambda}e^{-l\sqrt{-\lambda}} + \sqrt{\lambda}e^{l\sqrt{-\lambda}}) = 0 \\
\therefore C = 0, \ X(x) = 0, u(x, y) = 0 \\
\\
\lambda = 0 \\
X(x) = C_1x + C_2 \\
T(t) = C_1't + C_2' \\
u|_{x = 0} = 0 \Rightarrow C_2 = 0 \\
u_x|_{x = l} = 0 \Rightarrow C_1 = 0 \\
X(x) = 0, \ u(x, y) = 0 \\
\\
\lambda > 0 \\
X(x) = C_1 \sin x\sqrt{\lambda} + C_2 \cos x\sqrt{\lambda} \\
u|_{x = 0} = 0 \Rightarrow C_2 = 0 \\
u_x|_{x = l} = 0 \Rightarrow C_1 \sin l\sqrt{\lambda} = 0 \Rightarrow l\sqrt{\lambda} = n\pi + \frac{\pi}{2} \Rightarrow \lambda_n = (\frac{2n + 1}{2l} \pi)^2, \ n = 0, \pm1, \cdots \\
\left \{
\begin{matrix}
\begin{aligned}
&X(x) = C_1 \sin \frac{2n + 1}{2l} \pi x \\
&T(t) = C_1' \sin \frac{2n + 1}{2l} a\pi t + C_2' \cos \frac{2n + 1}{2l} a \pi t \\ 
&n = 1, 2, \cdots \\
\end{aligned}
\end{matrix}
\right.
\\
u_n(x, y) = (C_n \sin \frac{2n + 1}{2l} a \pi t + D_n \cos \frac{2n + 1}{2l} a \pi t) \sin \frac{2n + 1}{2l} \pi x \\
\\
u(x, y) = \sum_{n = 1}^{\infty} (C_n \sin \frac{2n + 1}{2l} a \pi t + D_n \cos \frac{2n + 1}{2l} a \pi t) \sin \frac{2n+ 1}{2l}\pi x \\
u(x, 0) = \phi(x) = \sum_{n = 1}^{\infty} D_n \sin \frac{2n + 1}{2l} \pi x   \Rightarrow D_n = \frac{2}{l} \int_0^l \phi(x) \sin \frac{2n + 1}{2l} \pi x d x\\
u_t(x, 0) = \psi(x) = \sum_{n = 1}^{\infty} C_n \frac{2n + 1}{2l} a\pi \sin \frac{2n + 1}{2l} \pi x \Rightarrow C_n = \frac{4}{(2n + 1)a\pi} \int_0^l \psi(x) \sin \frac{2n + 1}{2l} \pi x dx\\
$$

$$
\left \{
\begin{matrix}
\begin{aligned}
& u_{tt} = a^2 u_{xx} + f(x, t)\\
& u(0, t) = 0, u(l, t) = 0 \\
& u(x, 0) = 0, \ u_t(x,0) = 0 \\ 
& 0 < x < l,\ t > 0
\end{aligned}
\end{matrix}
\right.
\\
\\
u_{tt} = a^2u_{xx} \Rightarrow X(x) = B_n\sin \frac{n\pi x}{l} \\
f(x, t) \in \{\sin \frac{n \pi x}{l}\}\\
u(x, t) = \sum_{n = 1}^\infty u_n(t) \sin \frac{n \pi x}{l} \\
f(x, t) = \sum_{n = 1}^{\infty} f_n(t) \sin\frac{n \pi x}{l} \\
f_n(t) = \frac{2}{l} \int_0^lf(x, t) \sin \frac{n \pi x}{l} dx \\
\sum_{n = 1}^\infty [u''_n(t) + (\frac{n \pi a}{l})^2u_n(t) - f_n(t)]\sin \frac{n \pi x}{l} = 0 \\
u_n(t) = \frac{l}{n \pi a} \int_0^l f_n(\tau) \sin \frac{n \pi a}{l} (t - \tau) d\tau \\
$$

$$
D'Alembert
\left \{
\begin{matrix}
\begin{aligned}
& u_{tt} = a^2 u_{xx} + f(x, t)\\
& u(x, 0) = \phi(x), \ u_t(x, 0) = \psi(x) \\
& -\infty < x < +\infty,\ t > 0
\end{aligned}
\end{matrix}
\right.
\\
\\
\begin{aligned}
&(1)\left \{
\begin{matrix}
\begin{aligned}
& u_{tt} = a^2 u_{xx}\\
& u(x, 0) = \phi(x), \ u_t(x, 0) = \psi(x) \\
& -\infty < x < +\infty,\ t > 0
\end{aligned}
\end{matrix}
\right.
\\
&(2)\left \{
\begin{matrix}
\begin{aligned}
& u_{tt} = a^2 u_{xx} + f(x,t)\\
& u(x, 0) = 0, \ u_t(x, 0) = 0 \\
& -\infty < x < +\infty,\ t > 0
\end{aligned}
\end{matrix}
\right.
\end{aligned}
\\
\\
(1) \\
\left \{
\begin{matrix}
\begin{aligned}
& \xi = x - at \\
& \eta = x + at
\end{aligned}
\end{matrix}
\right.
\\
\left \{
\begin{matrix}
\begin{aligned}
& x = \frac{\xi + \eta}{2} \\
& y = \frac{\eta - \xi}{2a}
\end{aligned}
\end{matrix}
\right.
\\
u(x, t) = u(\frac{\xi + \eta}{2}, \frac{\eta - \xi}{2a}) = u'(\xi, \eta) \\
\left \{
\begin{matrix}
\begin{aligned}
& u_x = u'_\xi + u'_\eta \\
& u_{xx} = u'_{\xi \xi} + 2u'_{\xi \eta} + u'_{\eta \eta} \\
& u_{tt} = a^2(u'_{\xi \xi} - 2u'_{\xi \eta} + u'_{\eta \eta})
\end{aligned}
\end{matrix}
\right.
\\
u'_{\xi \eta} = 0 \Rightarrow u' = f(\xi) + g(\eta) \\
u = f(x - at) + g(x + at) \\
u(x, 0) = 0 \Rightarrow f(x) + g(x) = \phi(x) \\
u_t(x, 0) = 0 \Rightarrow -af_t(x) + ag_t(x) = \psi(x) \Rightarrow -f(x) + g(x) = \frac{1}{a} \int_{x_0}^x \psi(z) dz + c \\
\left \{
\begin{matrix}
\begin{aligned}
& f(x) = \frac{1}{2}\phi(x) - \frac{1}{2a}\int_{x_0}^x \psi(z) dz - \frac{c}{2} \\
& g(x) = \frac{1}{2}\phi(x) - \frac{1}{2a}\int_{x_0}^x \psi(z) dz + \frac{c}{2} \\
\end{aligned}
\end{matrix}
\right.
\\
u(x, t) = \frac{\phi(x - at) + \phi(x + at)}{2} + \frac{1}{2a}\int_{x - at}^{x + at}\psi(z) dz
\\
\\
(2) \\
u(x, t) = \frac{1}{2a} \int ^t_0 \int_{x - a(t - \tau)}^{x + a(t - \tau)} f(\xi, \tau) d\xi d\tau
\\
\\
u(x, t) = \frac{\phi(x - at) + \phi(x + at)}{2} + \frac{1}{2a}\int_{x - at}^{x + at}\psi(z) dz + \frac{1}{2a} \int ^t_0 \int_{x - a(t - \tau)}^{x + a(t - \tau)} f(\xi, \tau) d\xi d\tau
$$



$$
Kirchhoff
\left \{
\begin{matrix}
\begin{aligned}
& u_{tt} = a^2(u_{xx} + u_{yy} + u_{zz}) \\
& u(x, y, z, 0) = \phi(x, y, z), \ u_t(x, y, z, 0) = \psi(x, y, z) \\
& -\infty < x, y, z < +\infty,\ t > 0
\end{aligned}
\end{matrix}
\right.
\\
$$






# 热传导方程

$$
Dirichlet
\left \{
\begin{matrix}
\begin{aligned}
& \frac{\part u}{\part t} = a^2\frac{\part^2 u}{\part x^2} \\
& u|_{x = 0} = 0, u|_{x = l} = 0 \\
& u|_{t = 0} = \phi(x) \\ 
& 0 < x < l,\ t > 0
\end{aligned}
\end{matrix}
\right.
\\
\\
u(t, x) = T(t)X(x)\\
T'(t)X(x) = a^2T(t)X''(x) \\
\frac{X''(x)}{X(x)} = \frac{T'(t)}{a^2T(t)} = -\lambda \\
\left \{
\begin{matrix}
\begin{aligned}
&X'' + \lambda X = 0 \\
&T' + \lambda a^2 T = 0 
\end{aligned}
\end{matrix}
\right.
\\
\\
X(x) = C_1 \sin \frac{n\pi x}{l} \\
T(t) = C_2e^{-\frac{a^2n^2\pi^2}{l^2}t} \\
u(x, y) = \sum_{n = 1}^\infty c_n \sin \frac{n\pi x}{l} e^{-\frac{a^2n^2\pi^2}{l^2}t} \\
u|_{t = 0} = \phi(x) \Rightarrow  c_n = \frac{2}{l}\int_{0}^{l}\phi(x) \sin \frac{n\pi x}{l} dx
$$


$$
\left \{
\begin{matrix}
\begin{aligned}
& u_t = a^2 u_{xx} + f(x, t) \\
& u(0, t) = 0, u(l, t) = 0 \\
& u(x, 0) = 0 \\ 
& 0 < x < l,\ t > 0
\end{aligned}
\end{matrix}
\right.
\\
\\
u(x, t) = \sum_{n = 1}^\infty u_n(t) \sin \frac{n \pi x}{l} \\
f(x, t) = \sum_{n = 1}^\infty f_n(t) \sin \frac{n\pi x}{l} \\
\sum_{n = 1}^\infty [u'_n(t) + (\frac{n \pi a}{l})^2u_n(t) - f_n(t)] \sin\frac{n \pi x}{l} = 0 \\
\left \{
\begin{matrix}
\begin{aligned}
& u'_n(t) + (\frac{n\pi a}{l})^2u_n(t) = f_n(t) \\
& u_n(0) = 0
\end{aligned}
\end{matrix}
\right.
\\
u_n = \int^l_0 f(\tau) e^{-\frac{n\pi a}{l}(t - \tau)} d\tau 
$$




# 拉普拉斯方程

$$
Dirichlet
\left \{
\begin{matrix}
\begin{aligned}
& \frac{\part^2 u}{\part x^2} + \frac{\part^2 u}{\part y^2} = 0 \\
& u(x, 0) = \phi(x), \ u(x, b) = \psi(x)  \\
& u(0, y) = 0, \ u(a, y) = 0 \\ 
& 0 < x < a,\ 0 < y < b 
\end{aligned}
\end{matrix}
\right.
\\
\\
u(x, y) = X(x)T(t) \\
\frac{X''}{X} = \frac{T''}{T} = -\lambda \\
\left \{
\begin{matrix}
\begin{aligned}
& X_n (x) = A_n \sin \frac{n\pi}{a} \\
& Y_n (y) = B_ne^{\frac{n\pi}{a}y} + C_ne^{-\frac{n\pi}{a}y}
\end{aligned}
\end{matrix}
\right.
\\
u(x, y) = \sum_{n = 1}^{\infty} (a_ne^{\frac{n\pi}{a}y} + b_ne^{-\frac{n\pi}{a}y})\sin\frac{n\pi}{a}x \\
u(x, 0) = \sum_{n = 1}^\infty (a_n + b_n)\sin \frac{n\pi}{a}x = \phi(x) \\
u(x, b) = \sum_{n = 1}^\infty (a_ne^{\frac{n\pi b}{a}} + b_ne^{-\frac{n \pi b}{a}})\sin \frac{n \pi}{a}x = \psi(x) \\
$$




$$
\left \{
\begin{matrix}
\begin{aligned}
& u_{rr} + \frac{1}{r}u_r + \frac{1}{r^2}u_{\theta\theta} = 0 \\
& u(r_0, \theta) = \phi(\theta) \\
& 0 < r < r_0, \ 0 < \theta < 2\pi
\end{aligned}
\end{matrix}
\right.
\\
\\
u(r, \theta) = R(r)\Phi(\theta) \\
R''\Phi + \frac{1}{r}R'\Phi + \frac{1}{r^2}R\Phi'' = 0 \\
\frac{r^2R'' + rR'}{R} = -\frac{\Phi''}{\Phi} = \lambda \\
\\
\left \{
\begin{matrix}
\begin{aligned}
& r^2R'' + rR' - \lambda R = 0 \\
& \Phi'' + \lambda \Phi = 0 \\
& \Phi(\theta + 2\pi) = \Phi(\theta) \\
& |R(0)| < +\infty
\end{aligned}
\end{matrix}
\right.
\\
\\
\lambda = 0 \\
\Phi(\theta) = A\theta + B\\
\Phi(\theta + 2\pi) = \Phi(\theta) \Rightarrow A = 0 \\
R(r) = C\ln r + D \\
|R(0)| < +\infty \Rightarrow C = 0 \\
u(r, \theta) = E \\
\\
\lambda  > 0 \\
\Phi(\theta) = A\cos \sqrt{\lambda}\theta + B\sin \sqrt{\lambda} \theta \\
\Phi(\theta + 2\pi) = \Phi(\theta) \Rightarrow \lambda = n^2 \\
\Phi_n(\theta) = A_n \cos n\theta + B_n \sin n\theta \\
R(r) = C_nr^n + D_nr^{-n} \\
|R(0)| < \infty \Rightarrow D_n = 0 \\
u(r, \theta) = \frac{1}{2}a_0 + \sum_{n = 1}^{\infty}(a_n \cos n\theta + b_n \sin n\theta)r^n \\
u(r_0, \theta) =  \frac{1}{2}a_0 + \sum_{n = 1}^{\infty}(a_n \cos n\theta + b_n \sin n\theta)r_0^n = \phi(\theta) \\
a_n = \frac{1}{\pi r_0^n}\int_0^{2\pi} \phi(\theta)\cos n\theta d\theta \\
b_n = \frac{1}{\pi r_0^n}\int_0^{2\pi} \phi(\theta)\sin n\theta d\theta \\
$$

$$
Possion
\left \{
\begin{matrix}
\begin{aligned}
& u_{xx} + u_{yy} =  \\
& u(x, 0) = \phi(x), \ u(x, b) = \psi(x)  \\
& u(0, y) = 0, \ u(a, y) = 0 \\ 
& 0 < x < a,\ 0 < y < b 
\end{aligned}
\end{matrix}
\right.
\\
\\
$$
