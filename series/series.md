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
