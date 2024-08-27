[TOC]



# 傅里叶级数

$$
f(t) = \frac{a_0}{2} + \sum_{n = 1}^\infty (a_n\cos n\omega t + b_n \sin n\omega t)
$$

$$
Dilchlet: \\
有限间断点 \\
有限个极值
$$


$$
f(t) = \frac{f(t^-) + f(t^+)}{2}
$$

$$
\sin z = \frac{e^{iz} - e^{-iz}}{2i}, \ \cos z = \frac{e^{iz} + e^{-iz}}{2} \\
\sin \omega t = \frac{e^{i\omega t} - e^{-i\omega t}}{2i} , \ \cos \omega t = \frac{e^{i\omega t} + e^{-i\omega t}}{2} \\
f(t) = \sum_{n = -\infty}^{+\infty}c_n e^{i n \omega t}
$$


$$
\int_{-\frac{T}{2}}^{\frac{T}{2}} f(t) e^{-i m \omega t} dt = \sum_{n = - \infty} ^{+\infty} c_n\int_{-\frac{T}{2}}^{\frac{T}{2}} e^{i n \omega t}e^{-i m \omega t} dt = \sum_{n \ne m} c_n \int_{-\frac{T}{2}}^{\frac{T}{2}}e^{i(n - m)\omega t} dt + Tc_m \\
\int_{-\frac{T}{2}}^{\frac{T}{2}} e^{i(n - m)\omega t} dt = \frac{e^{i(n - m)\omega t}}{i(n - m)\omega} |^{\frac{T}{2}}_{-\frac{T}{2}} = \frac{2}{(n - m)\omega}\frac{e^{[(n - m)\omega\frac{T}{2}]i} - e^{-[(n - m)\omega\frac{T}{2}]i}}{2i} = \frac{2}{(n - m) \omega} \sin[(n - m)\omega \frac{T}{2}] = \frac{2}{(n - m) \omega} \sin[(n - m)\pi] = 0 \\
c_n = \frac{1}{T} \int_{-\frac{T}{2}}^{\frac{T}{2}} f(t) e^{-i n \omega t} dt
$$

$$
f(t) = \lim_{T \rightarrow \infty} \sum_{n = -\infty}^{+\infty} c_n e^{in\omega t} = \lim_{T \rightarrow \infty} \sum_{n = -\infty}^{+\infty} \frac{1}{T}(\int_{-\frac{T}{2}}^{\frac{T}{2}} f(t) e^{-i n \omega t} dt) e^{in\omega t} = \lim _{w\rightarrow 0} \frac{1}{2\pi} \omega\sum_{n = -\infty}^{+\infty}\phi(\omega)e^{in\omega t} = \frac{1}{2\pi} \int_{-\infty}^{+\infty} (\int_{-\infty}^{+\infty}f(\tau)e^{-i\omega \tau} d\tau) \ e^{i\omega t} d \omega
$$



$$
F(\omega) = \int_{-\infty}^{+\infty} f(\tau) e^{-i\omega \tau} d \tau \\
f(t) = \frac{1}{2\pi} \int_{-\infty}^{+\infty} F(\omega) e^{i \omega t} d \omega \\
$$

$$
f(-t) = f(t) \\
\\
F(\omega) = \int_{-\infty}^{+\infty} f(\tau) (\cos \omega \tau - i \sin \omega \tau) d\tau = \int_{-\infty}^{+\infty} f(\tau) \cos \omega \tau d\tau = 2\int_{0}^{+\infty} f(\tau) \cos \omega \tau d\tau \\
F(-\omega) = F(\omega) \\
\\
f(t) = \frac{1}{2\pi} \int_{-\infty}^{+\infty} F(\omega) (\cos \omega t + i\sin \omega t) d \omega = \frac{1}{2\pi} \int_{-\infty}^{+\infty} F(\omega) \cos \omega t d \omega = \frac{2}{\pi}\int_{0}^{+\infty}(\int_{0}^{+\infty}f(\tau) \cos \omega \tau d \tau) \cos \omega t d \omega
$$

$$
f(-t) = f(t) \\
\\
f(t) = \frac{2}{\pi} \int_{0}^{+\infty} (\int_{0}^{+\infty} f(\tau) \sin \omega \tau d \tau) \sin \omega t d \omega
$$





$$
f(t) = 
\left \{
\begin{matrix}
1 \ , \quad |t| \leq 1 \\
0 \ , \quad other
\end{matrix}
\right.
\\
\\
T = 2\\
F(\omega) = \int_{-1}^{1} e^{-i\omega \tau} d \tau  = \frac{2}{\omega} \sin \omega\\
f(t) = \frac{1}{2\pi} \int_{-\infty}^{+\infty} \frac{2}{\omega} \sin \omega e^{i \omega t} d \omega = \frac{2}{\pi}\int_{0}^{+\infty} \frac{\sin \omega \cos \omega}{\omega} d\omega \\
\\
\frac{2}{\pi}\int_{0}^{+\infty} \frac{\sin \omega \cos \omega}{\omega} d\omega = 
\left \{
\begin{matrix}
1 \ , \quad |t| < 1 \\
\frac{1}{2} \ , \quad t = \pm 1 \\
0 \ , \quad other
\end{matrix}
\right.
\\
\\
\int_{0}^{+\infty} \frac{\sin \omega}{\omega} d \omega = \frac{\pi}{2}
$$







$$
f(t) = 
\left \{
\begin{matrix}
\begin{aligned}
&1 \ , \quad 0 \le t \le 1 \\
&0 \ , \quad t > 1
\end{aligned}
\end{matrix}
\right.
\\
\\
f_{e}(t) = 
\left \{
\begin{matrix}
\begin{aligned}
1& \ , \quad &0 \le t \le 1 \\
-1& \ , \quad &-1 \le t < 0 \\
0& \ , \quad &t > 1
\end{aligned}
\end{matrix}
\right.
\\
\\
F(\omega) = \frac{1 - \cos \omega}{\omega} \\
f_e(t) = \frac{\pi}{2} \int_{0}^{+\infty} \frac{1 - \cos \omega} {\sin \omega}  \omega t d \omega
$$



$$
\mathcal{F}(\alpha f(t) + \beta g(t)) = \alpha\mathcal{F}(f(t)) + \beta \mathcal{F} (g(t)) \\
\mathcal{F(f(t - t_0))} = e^{-i \omega t_0}\mathcal{F(f(t))} \\
\mathcal{F(f'(t))} = (i\omega) \mathcal{F(\omega)}
$$
