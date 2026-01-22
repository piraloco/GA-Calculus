$d \times f'(x) = f(x + d) - f(x)$
$d^2 = 0$

$e_0^2 = 0$
$e_{n}^2 = 1$

$\text{boost}(e_2^{\frac1 2})e_1$
starts at $e_1$
velocity is $e_2^{\frac 1 2}v$

$e_1e_2^{\frac 1 2}$
$d_1^2= e_1$

$(1 + e_1)^2 = 2 + 2e_1$

$\text{boost}(1 + e_1)\times e_1$
starts at $e_1$
velocity is $1 + e_1$

$\text{boost}(e_1 + e_1e_2)e_1$
$\text{boost}(e_1) \text{boost}(e_1e_2)e_1$

$e_1\text{boost}(\pi (e_1e_2 + e_2e_3))$
$e_1\text{boost}(\pi e_1e_2)\text{boost}(\pi e_2e_3)$
$-e_1 \text{boost}(\pi e_2e_3)$


$(e_1 + e_2)^2$
$1 + e_1e_2 + e_2e_1 + 1$
$2$

$(e_1 + e_2e_3e_4)^2$
$1 + e_1e_2e_3e_4 - e_1e_2e_3e_4 - 1$
$0$

For **PGA**:

$e_1$, $e_2$, $e_3$, $e_4 + e_1e_2e_3$

$e_1(e_4 + e_1e_2e_3)$
$e_1e_4 + e_2e_3$


$V_1(v) = e_1 - \frac{1}{2}(v \cdot e_2)e_3$
$V_2(v) = e_2 + \frac{1}{2}(v \cdot e_1)e_3$
$V_3(v) = e_3$

$V(v) = e_1 + e_2 + (1 + v\cdot \frac{1}{2}(e_1 - e_2))e_3$

$d = e_0e_1$
$dV'(v) = V(v + d) - V(v)$
$dV'(v) = (1 + v \cdot \frac{1}{2}(e_1 - e_2) + d\cdot \frac{1}{2}(e_1 - e_2))e_3 - (1 + v \cdot \frac{1}{2}(e_1 - e_2))e_3$
$dV'(v) = e_3 + \frac{1}{2}(v \cdot e_1)e_3 - \frac{1}{2}(v \cdot e_2)e_3 + \frac{1}{2}(e_0e_1 \cdot e_1)e_3 - \frac{1}{2}(e_0e_1 \cdot e_2)e_3$
$e_0e_1V'(v) = \frac{1}{2}e_0e_3$
$e_1V'(v) = \frac{1}{2}e_3$
$V'(v) = 


$V(v) = e_1 \wedge e_2 \wedge (e_3 + (v \cdot e_1)e_3 - (v \cdot e_2)e_3)$
$V(v) = e_1 \wedge e_2 \wedge (1 + v\cdot e_1 - v \cdot e_2)e_3$
$V(v) = e_1 \wedge e_2 \wedge (v \cdot e_1)e_3 - e_1 \wedge e_2 \wedge (v \cdot e_2)e_3$
$V(v) = e_1 \wedge e_2 \wedge (v\cdot e_1 - v\cdot e_2)e_3$

$e_0e_1V'(v) = V(v + e_0e_1) - V(v)$

$e_1 \wedge e_2 \wedge (v \cdot e_1 - v \cdot e_2 + e_0)e_3$
$e_1 \wedge e_2 \wedge e_0e_3$
$V'(v) = e_2\wedge e_3$
---

Let's say we have vectors $a$ and $b$, how do we find the geodesic between them? How do we even express a trajectory path in GA??

The thing that comes to mind is exponentials... Since they do represent a path with a velocity related to the position...

For example: a circular trajectory can be represented as:

$$F(t) = \text{boost}(t \cdot e_1e_2) e_1$$
$e_1$ is the initial condition, $e_1e_2$ is the span where the boost takes place, and $t$ is time.

$F(0) = a$
$F(t + \epsilon) = F(t) + \epsilon(V(F(t) + \epsilon(b - a)) - V(F(t)) \circlearrowleft (F(t) + \epsilon(b - a)))$

$F_0 = a$
$F_\prime = R\ d\ R^\dagger$
$R = \text{boost}(V(F + d) - V(F))$
$d^2 = 0$

$Q_0 = 0$
$Q_\prime = F_\prime^2$

$\mathbf{L}^2 = \text{min}(Q(t) : F(t) = b)$


---
---
---
---
---
---
---



$$
\begin{align}
&\gamma(0) = a\\
\\
&\frac{d^2\gamma^k}{dt^2} + \Gamma^k_{ij}\frac{d\gamma^i}{dt}\frac{d\gamma^j}{dt} = 0\\
\\
&\Gamma^k_{ij} = \frac{1}{2}g^{kl}\left(\frac{\partial g_{jl}}{\partial x^i} + \frac{\partial g_{il}}{\partial x^j} - \frac{\partial g_{ij}}{\partial x^l}\right)\\
\\
&\gamma_{l+1} = \gamma_l + \Delta t \cdot v_l + \frac{(\Delta t)^2}{2}a_l\\
\\
&v_{l+1} = v_l + \Delta t \cdot a_l\\
\\
&a^k_l = -\Gamma^k_{ij}(\gamma_l)\, v^i_l\, v^j_l\\
\\
&g_{ij}(\gamma(t))\frac{d\gamma^i}{dt}\frac{d\gamma^j}{dt} = c\\
\\
&Q_l = \sum_{k=0}^{l-1} \sqrt{g_{ij}(\gamma_k)\,\Delta\gamma^i_k\,\Delta\gamma^j_k}\\
\\
&\Delta\gamma^i_k = \gamma^i_{k+1} - \gamma^i_k\\
\\
&\min_{v_0} \|\gamma(T;v_0) - b\|^2\\
\\
&\gamma(T) = \gamma(0) + \int_0^T v(t)\,dt\\
\end{align}$$

---
---
---
---
---
---
---

$$\begin{align}
F_0 &= a\\
F_\prime &= \langle 1 + \epsilon V_\prime|d \rangle\\
\mathbf{T} &= \lfloor F_? = b\rfloor\\
\end{align}$$

$$\begin{align}
\mathbf{T} := \lfloor a ;\langle 1 + \epsilon V'|d \rangle = b\rfloor
\end{align}$$

---
$$\Huge\boxed{\begin{align}
P &= R\,\,p'R^\dagger\\
R &= 
1+ M(p + s d) - M(p)
\end{align}}$$


$M(p) = e_1\wedge e_2\wedge e_3$
$p(0) = 0$
$p(t + \epsilon e_u e_v) = p(t) + \epsilon e_u e_v(p(t) + \epsilon e_u e_v d)$
$p(t + \epsilon e_u e_v) = p(t) + \epsilon e_u e_v d$

$p(e_1) = e_1$
$p(e_1 + \epsilon e_1 e_2) = e_1 + \epsilon e_1 e_2 d$
$d = e_2$
$p(e_1 + \epsilon e_1 e_2) = e_1 + \epsilon e_1$

$p(e_1 + \epsilon e_1) = e_1 + \epsilon e_1 e_1 e_2$
$p(e_1 + \epsilon e_1) = e_1 + \epsilon e_2$


$M(p) = e_1\wedge e_2 \wedge e_3$
$p(t) = \text{boost}(t\ e_2)e_1$
$sp'(t) = p(t + s) - p(t)$
$sp'(t) = \text{boost}(t\ e_2)\text{boost}(s\ e_2)e_1 - \text{boost}(t\ e_2)e_1$
$sp'(t) = \text{boost}(t\ e_2)se_2e_1$
$p'(t) = e_2\text{boost}(t\ e_2)e_1$

$M(p) = e_1 \wedge e_2 \wedge (p \cdot e_1) e_3$
$R = 1 + M(p + s) - M(p)$
$R = 1 + e_1 \wedge e_2 \wedge (s \cdot e_1)e_3$
$R = 1 + e_1 \wedge e_2 \wedge e_0e_3$
$R = 1 + e_0e_1e_2e_3$

$P(t) = R\ p'(t)R^\dagger$
$P(t) = -e_1e_2\text{boost}(t e_2) + 2e_0e_3\text{boost}(t e_2)$
$P(t) = p'(t) + 2e_0e_3\text{boost}(te_2)$


$$\Huge{\begin{align}
q(x) ={g(p(x)|\epsilon)}_\Uparrow\circ p(x|\epsilon)
\end{align}}$$

$$\large \begin{align}\text{q}\ x &= k \times (\text{p}\ (x + \epsilon) - \text{p}\ x)\times k^{-1}\\ k &=\text{boost}\ (\text{g}\ (\text{p}\ x + \epsilon) - \text{g}\ (\text{p}\ x))
\end{align}$$




$q(x) = kdk^\dagger$
$d = p(x + \epsilon) - p(x)$
$k = 1 + M(p(x) + \epsilon) - M(p(x))$

$x$: manifold parameter
$p(x)$: point on the manifold
$M(v)$: curvature pseudoscalar

Alternative syntax:

$q(x) = KdK^\dagger$
$K = 1 +^\uparrow M$
$d = p(x|\epsilon)$
$M = g(p(x)|\epsilon)$



$$\Huge\boxed{{{v_g = (1 \oplus k) \triangleright v}}}$$



$v_g = (1 \oplus k) \triangleright v$



$f'(x) = g(f(x))$

$f'(x) = f(x)^2$

$f(0) = 0$
$f(x + \epsilon) = f(x) + \epsilon f(x)^2$

$f(\epsilon) = 0$

$\exp(0) = 1$
$\exp(x + \epsilon) = (1 + \epsilon)\exp(x)$

$f(x + \epsilon) = (1 + \epsilon f(x))f(x)$

$\epsilon \exp(x) = \exp(x + \epsilon) - \exp(x)$
$\epsilon f(x)^2 = f(x + \epsilon) - f(x)$
$f(x) = (\frac{1}{\epsilon}((x + \epsilon) - f(x))^\frac{1}{2}$


$f(x) = \epsilon f(x) - f(x + \epsilon)$

$f(x) = \epsilon f(x) + f(x - \epsilon)$

$f(x) = f(x - \epsilon) + \epsilon f(x - \epsilon)$
$f(x) = f(x - \epsilon) + \epsilon f(x - 2\epsilon) + \epsilon^2 f(x - 3\epsilon) + \dots$
$f(x) = f(x - \epsilon) + \epsilon f(x - \epsilon)^2$

$f = f_{-1} + \epsilon(f_{-2}^2 + 2\epsilon f_{-2}^3)$

$f(x) = f(x - \epsilon) + \epsilon f(x - 2\epsilon)^2 + 2\epsilon^2 f(x - 2\epsilon)^3$
$f(x) = f(x - \epsilon) + \epsilon(1 + 2\epsilon f(x - 2\epsilon))f(x - 2\epsilon)^2$
$f(x - \epsilon)^2 = (1 + 2\epsilon f(x - 2\epsilon))f(x - 2\epsilon)^2$

$f(x)^2 = f(x - \epsilon)^2 + 2\epsilon f(x - \epsilon)^3$





$f'(x) = f(x)^2$

$f(x + \epsilon) = f(x) + \epsilon f'(x)$

$t_n = t_{n-1} \frac{x-a}{n}\frac{f^{(n)}(a)}{f^{(n-1)}a)}$

$f(x) = f(a) + f(a)^2(x - a) + f(a)^4\frac{(x - a)^2}{2}$

$f(x) = \frac{f(a)^{2^0}(x-a)^0}{0!} + \frac{f(a)^{2^1}(x - a)^1}{1!} + \frac{f(a)^{2^2}(x - a)^2}{2!}$
$f(x) = \sum \frac{f(a)^{2^n}(x - a)^n}{n!}$

$f(0) = 2$
$f(s) = 2 + 4s + 16s^2$

# Integration!!!!

$f(0) = 0$
$f(t) = f(t - f'(\epsilon)) + \epsilon f'(t)$

$f(t + \epsilon) = f(t) + \epsilon f'(t)$


$f(t) = 3\epsilon t^2 + f(t - \epsilon)$
$f(t) = 3\epsilon t^2\frac{t}{\epsilon}$




$f(t) = f(t - 2\epsilon) + 2\epsilon t$

$f(t) = 2 \epsilon t + 2 \epsilon t + 2 \epsilon t + \dots$
$f(t) = 2\epsilon t \frac{t}{2\epsilon}$
$f(t) = t^2$



$f(x) = \sum_{t=0}^x 2t \epsilon$
$f(x) = \text{sum}(t:0\dots x \to 2t)$

$f(0) = 0$
$f(x + \epsilon) = f(x) + 2\epsilon x$

$f(x) = 0; 2x$

$\exp(x) = 1; \exp(x)$

$\exp(x) = [t:1; \exp(t)]_x$

$\exp(x) = 1 \oplus x$

$f(x) = f(0) + f'(0)x + f''(0)\frac{x^2}{2} + \dots$


$\exp = 1; \exp$
$x. x^2 = 0; x. 2x$

$4 = (0; x. 2x)(2)$



$\exp(0) = 1$
$[d;\exp](x) = d\exp(x)$
$d^2 = 0$

$\exp(d) = 1 + d$
$\exp(a + b) = \exp(a)\exp(b)$

$\text{mot}(t, x, y) = \exp(t(x\wedge y))x$

$\exp(0) = 1$
$\exp(x + h) = \exp(x) + h\exp(x)$

$\text{circ}(t) = \exp(t e_{12})$

$\text{circ}(t + h) = \exp(te_{12} + he_{12})$
$\text{circ}(t + h) = (1 + he_{12})\exp(te_{12})$
$\text{circ}(t + h) = \text{circ}(t) +he_{12}\text{circ}(t)$

$\text{circ}(t + 2h) = \text{circ}(t + h) + he_{12}\text{circ}(t + h)$
$\text{circ}'(t) = e_{12}\text{circ}(t)$

$\text{circ}'(t + h) = e_{12}\text{circ}(t) + he_{12}^2\text{circ}(t)$


# this is cool :o

$\text{mot}(a)(t) = \exp(ta)$
$\text{mot}(a)' = a\text{ mot}(a)$

$\text{circ}'' = -\text{circ}$
$\text{par}'' = 0$
$\text{hyp}'' = \text{hyp}$

$\text{circ} \supset \text{mot}(i),\quad i^2 = -1$
$\text{par} \supset \text{mot}(\epsilon),\quad \epsilon^2 = 0$
$\text{hyp} \supset \text{mot}(j),\quad j^2 = 1$

---


$$\large
\begin{align}
\text{mot}(a)(t) &= \text{exp}(at)
\\
\nabla(\text{mot}(a)) &= a\text{ mot}(a)
\end{align}
$$

$$\large
\begin{align}
f \in \text{circ} &\iff \nabla^2(f) = -f
\\
f \in \text{par} &\iff \nabla^2(f) = 0
\\
f \in \text{hyp} &\iff \nabla^2(f) = f
\end{align}
$$

$$\large
\begin{align}
i^2 = -1 &\iff \text{mot}(i) \subset \text{circ}
\\
\epsilon^2 = 0 &\iff \text{mot}(\epsilon) \subset \text{par}
\\
j^2 = 1 &\iff \text{mot}(j) \subset \text{hyp}
\end{align}
$$




# Integration 2.3.4.5.6.7.8....

$$\int dx = x + C$$

$$\begin{align}
f(x) &= \int dx \\
f(x) &= f(0) + x
\end{align}$$

$$f(x + dv) = f(x) + dv$$
$$f(x) = dv + d(x - dv)$$
$$f(x) = dv + dv + dv + \dots$$
$$f(x) = dv\frac{x}{dv} + f(0)$$

$$f(x) = f(0) + \sum_{n=0}^{x/dv} dv$$
$$f(x) = f(0) + dv\sum_{n=0}^{x/dv} 1$$
$$f(x) = f(0) + dv\frac{x}{dv}$$
$$f(x) = f(0) + x$$

---

$$f(x) = f(0) + dv\sum_{n=0}^{x/dv} 2n$$

$$S = 0 + 2 + 4 + 6 + 8 + 10 + \dots$$
$$S = 2(1 + 2 + 3 + 4 + 5 + \dots)$$
$$1 + 2 + 3 + \dots + (\frac{x}{dv}-1) + \frac{x}{dv}$$
$$(\frac{x}{dv} + 1)\frac{x}{2dv}$$
$$S = (\frac{x}{dv} + 1)\frac{x}{dv}$$
$$f(x) = f(0) + dv(\frac{x}{dv} + 1)\frac{x}{dv}$$
$$f(x) = f(0) + x^2 + \frac{x^2}{dv}$$


$$f(x) = f(0) + \sum_{n=0}^{x/d} 2n$$

$$f(x) = 2dx + 2d(x - d) + \dots + f(0)$$
$$f(x) = 2d((x + d)\frac{x}{2d}) + f(0)$$
$$f(x) = 2d(\frac{x^2}{2d} + \frac{x}{2}) + f(0)$$

$f(x) = d(2x\frac{x}{2d}) + f(0)$

$f(x) = 3dx^2 + 3d(x - d)^2$

$3d(x - d)^2 = 3dx^2 - 6d^2x$

$f(x) = 3dx^2 + 3dx^2 - 6d^2x + 3dx^2 - 12d^2x + \dots$
$f(x) = 3dx(x + x - 2d + x - 4d + \dots)$

$x - nd \times \frac{2x}{3d^2}$
$x + x - d + x - 2d + x - 3d + \dots + d + 0$
$x\frac{x}{3d^2}$

$f(x) = f(0) + 3dx\frac{x^2}{3d^2}$




$f(x) = 3dx^2 + f(x - d)$

$f(x) = 3dx^2 + 3d(x - d)^2 + 3d(x - 2d)^2 + \dots$
$f(x) = 3d(x^2 + (x - d)^2 + (x - 2d)^2 + \dots)$

$(x - nd)^2 = x^2 - 2ndx + n^2d^2$

$x^2 - 2ndx + n^2d^2 \times \frac{x}{d}$
$x^2 - 2nd(x + nd) \times \frac{x}{d}$


$\frac{x^3}{d} - 2nx(x + nd)$
$\frac{x^3}{d} - 2nx^2 + 2n^2d$




$x^2 \dots x^2 - 2\frac{x}{d}dx + x^2$
$x^2 \dots x^2 - 2x^2 + x^2$

$x^2 + 0$
$x^2 - 2dx + d^2 + x^2 - 2(\frac{x}{d}-1)dx + (\frac{x}{d}-1)^2d^2$
$x^2 - 2dx + d^2 + x^2 - 2\frac{x}{d}dx - 2dx + x^2 - d^2$
$3x^2 - 4dx - 2x^2$
$x^2 - 4dx$

$x^2 - 2x^2 - 2dx + x^2 - 2dx + d^2$
$4dx - d^2$

$x^2 - 2dx + d^2 + x^2 - 2(\frac{x}{d} - 2)dx + (\frac{x}{d} - 2)^2d^2$
$2x^2 - 2dx + d^2 - 2x^2 + 4dx + x^2 - 2dx + 4d^2$
$x^2 + 5d^2$



$x^2 - 2(\frac{x}{d} - n)dx + (\frac{x}{d} - n)^2d^2$
$x^2 - 2\frac{x}{d}dx + 2ndx + \frac{x^2}{d^2}d^2 - 2n\frac{x}{d}d^2 + n^2d^2$
$x^2 - 2x^2 + 2ndx + x^2 - 2ndx + n^2d^2$
$2ndx - 2ndx + n^2d^2$
$n^2d^2$


$x^2$

$x^2 - 2dx + d^2 + d^2$
$x^2 - 2d(x - d)$

$x^2 - 4dx + 4d^2 + 4d^2$
$x^2 - 4d(x - 2d)$

$x^2 - 6dx + 18d^2$
$x^2 - 6d(x - 3d)$


$x^2 - 2nd(x - nd) \times \frac{x}{2d}$

$x^2$

$x^2 - 2(\frac{x}{2d} - n)d(x - (\frac{x}{2d} - n)d)$
$x^2 - 2\frac{x}{2d}d(x - \frac{x}{2} + nd) + 2nd(x - \frac{x}{2} + nd)$
$x^2 - x(nd - \frac{x}{2}) + 2nd(nd - \frac{x}{2})$

$x^2 - ndx + \frac{x^2}{2} + 2n^2d^2 - ndx$
$\frac{3}{2}x^2 - 2ndx + 2n^2d^2$
$\frac{3}{2}x^2 - 2nd(x - 2nd)$

$x^2$

$x^2 - 2d(x - d) + \frac{3}{2}x^2 - 2d(x - 2d)$
$x^2 - 2dx - 2d^2 + \frac{3}{2}x^2 - 2dx - 4d^2$
$\frac{5}{2}x^2 - 4dx - 6d^2$






$f(x) = f(x - d) + df'(x)$
$f(x) = f(x - d) + 2dx$
$f(x) = 2dx + 2d(x - d) + 2d(x - 2d) + \dots + f(0)$
$f(x) = 2d(x + (x - d) + (x - 2d) + \dots) + f(0)$
$f(x) = 2d(x - nd \times_n \frac{x}{d}) + f(0)$
$f(x) = f(0) + (2d(x - nd) \times_n \frac{x}{d})$

$f(x) = f(0) + (df'(x - nd) \times_n \frac{x}{d})$


$$f(x) = f(0) + df'(x - nd) \times_n \frac{x}{d} $$

$$n \times_n 5 = 1 + 2 + 3 + 4 + 5$$

$$f(x) = f(0) + df'(dn) \times_n \frac{x}{d}$$

$f(x) = f(0) + df'(dn) \times_n \frac{x}{d}$
$n \times_n a = \frac{a(a + 1)}{2}$

$f(0) = 0$
$f'(x) = 2x$

$f(x) = 2d(dn) \times_n \frac{x}{d}$
$f(x) = 2d(d)(n \times_n \frac{x}{d})$
$f(x) = 2d(d)(\frac{x}{d}\frac{x + d}{2d})$
$f(x) = 2d(\frac{x(x + d)}{2d})$
$f(x) = x(x + d)$
$f(x) = x^2 + dx$

$df'(x) = (x + d)^2 + d(x + d) - x^2 - dx$
$df'(x) = x^2 + 2dx + dx - x^2 - dx$
$df'(x) = 2dx$
$f'(x) = 2x$




$n \times_n \frac{a}{b} = \frac{\frac{a}{b}(\frac{a + b}{b})}{2}$
$n \times_n \frac{a}{b} = \frac{a^2 + ab}{2b(b)}$
$n \times_n \frac{a}{b} = \frac{a^2}{2b(b)}$
$b^2 = 0 \implies n \times_n \frac{1}{b}a = \frac{1}{2}(\frac{1}{b})^2a^2$

$$n \otimes_n ba = \frac{b^2a^{2} + bx}{2},\quad b \in \aleph_2$$


$$\begin{align}
a &\in \aleph_{n-1}\\[0.1cm]
b^2 &= 0\\
x \in \aleph_n &\iff x = \frac{a}{b}\\
n \leq 0 &\iff \aleph_n = \{0\}
\end{align}$$

$\frac{0}{0}$

$b = \sqrt{0}$

$n \times_n \frac{a}{b} = \frac{\frac{a}{b}(\frac{a + b}{b})}{2}$
$2n \times_b^n a = \frac{a}{b}(\frac{a + b}{b})$
$2bn \times_{n,b} a = a(a + b)$

$2b(n \overset{b}{\times}_n a) = a^2 + ab$
$a^2 = (2(n \overset{b}\times_n a) - a)b$

$a^2 = 2(n \overset{1}\times_n a) - a$
$3^2 = 2(1 + 2 + 3) - 3$

$$a^2 = (2(\sum_{n+b}^a n) - a)b$$


$x^2 = (2(n \times_{n}^d x) - x)d$

$2d(n \times_n^d x) = x^2 + xd$

$f(x) = f(0) + df'(t) \times_t^d x$


$d(f'(x) \times_d x) = f(x) - f(0)$
$df'(x) = f(x + d) - f(x)$


$f(x + d) = f(x) + df'(x)$

$f(x) = f(x - d) + d'(x - d)$
$f(x) = f(0) + (df'(0) + {\dots} + df'(x - d))$



---

$f(a)(b) = a + b$

$d\nabla(f)(a) = f(a + d) - f(a)$

$d\nabla(f)(a)(b) = f(a + d)(b) - f(a)(b)$
$d\nabla(f)(a)(b) = a + b + d - a - b$
$\nabla(f)(a)(b) = 1$

$(\nabla f)ab = 1$


$fab = a \cdot b$

$h(\nabla \circ f)\circ a\circ b = f \circ (a + h) \circ b - f\circ a\circ b$
$h(\nabla \circ f)\circ a \circ b = (a + h)\cdot b - a\cdot b$
$h(\nabla \circ f)\circ a \circ b = h\cdot b$

$h(\nabla[f])[a][b] = f[a + h][b] - f[a][b]$
$h(\nabla[f])[a][b] = (a + h)\cdot b - a\cdot b$
$h(\nabla[f])[a][b] = h\cdot b$

$h\nabla(f)(a)(b) = f(a + h)(b) - f(a)(b)$
$h\nabla(f)(a)(b) = (a + h)\cdot b - a\cdot b$
$h\nabla(f)(a)(b) = h\cdot b$

$h\nabla(f(a))(b) = h\cdot a$

$\nabla(f(a))(b) = h^{-1}(h \cdot a)$
$\nabla(f(a)) = b. h^{-1}(h\cdot a)$

$f(a) = b.a \cdot b$

$\nabla(b.a \cdot b) = b.h^{-1}(h\cdot a)$

$\nabla = (b. a\cdot b).b.h^{-1}(h \cdot a)$


$\nabla \in (x. x^2). x. 2x$

$(x.x^2).x.2x = \{f\mid f(x.x^2) = x.2x\}$


$\forall n (\nabla \in (x.x^n).x.nx^{n-1})$





$^2\nabla\circ \text{circ} = x. -\text{circ} \circ x$
$^2\nabla \circ \text{par} = x. 0$
$^2\nabla \circ \text{hyp} = x. \text{hyp}\circ x$

$\text{circ} := f.\{^2\nabla \circ f = x.-(f\circ x)\}$
$\text{par} := f.\{^2\nabla\circ f = x. 0\}$
$\text{hyp} := f.\{^2\nabla \circ f = x.(f\circ x)\}$


$\text{circ} := f.\{^2\nabla = f.x.-(f\circ x)\}$

$\text{circ} := f.\{^2\nabla\circ f = x. -f\circ x\}$
$a.\,^2\nabla \circ (t.{\exp}\circ ta) = a. t. a^2({\exp}\circ ta)$
$a^2 = -1 \iff (t.{\exp}\circ ta) \in \text{circ}$


$a^2 = 1 \implies (t.{\exp} \circ ta) \subset \text{circ} \supset \text{mot}(i),\quad i^2 = -1$
$\text{par} \supset \text{mot}(\epsilon),\quad \epsilon^2 = 0$
$\text{hyp} \supset \text{mot}(j),\quad j^2 = 1$



$d. d\nabla \circ f \circ x = d. f\circ(x + d) - f\circ x$
$d. \nabla \circ f \circ x = d. d^{-1}(f \circ (x + d) - f\circ x)$
$d. \nabla = d.f.x.d^{-1}(f\circ (x + d) - f\circ x)$

$d. f\circ(x) = d. f\circ (x-d) + d(\nabla \circ f \circ (x -d))$

$d. f^x = d. f^{x - d} + d(\nabla^{f^{x- d}})$

$d. (d\nabla^{\large f^{\Large x}} = f^{\large x + d}- f^{\large x})$

$d. (d^2=0 \implies f.x.(f^{x + d} = f^x +( \nabla^f)^x))$

apply $e_0$

$e_0^2 = 0 \implies f.x.(f^{x + e_0} = f^x + e_0(\nabla^f)^x)$

if $e_0^2 = 0$:

$f.x.(f^{x + e_0} = f^x + e_0(\nabla^f)^x)$

apply $f = x.x^2$

$x.((x+e_0)^2 = x^2 + e_0(\nabla^{x.x^2})^x)$

$x.(x^2 + xe_0 + e_0x = x^2 + e_0(\nabla^{x.x^2})^x)$

$x.(xe_0 + e_0x = e_0(\nabla^{x.x^2})^x)$

if $x$ is a scalar:

$x.(2e_0x = e_0(\nabla^{x.x^2})^x)$
$x.(2x = (\nabla^{x.x^2})^x)$

"Given any $x$, $\nabla$ of the function $x.x^2$ applied to $x$ is $2x$"





# Quantifiers

"There exists an x such that $x + 1 = 0$"

$x.(x+1=0)$

$(x. (x + 1 = 0))^0 = \mathbb{F}$
$(0 + 1 = 0) = \mathbb{F}$
$(1 = 0) = \mathbb{F}$
$\mathbb{F} = \mathbb{F}$
$\mathbb{T}$

$a = b$
$a. b$
$a^b$

$a = a$
$a = b \implies x.a = x.b$
$a = b \implies a^x = b^x$

$\log_f (x) = \text{the thing(s) that you pass into f and get x}$
$Y := f.(x.f^{x^x})^{x.f^{x^x}}$
$\text{factorial} := Y (f.x.((x = 0)^{1})^{x f^{x - 1}})$

apply $3$:

$(Y(f.x.((x=0)^1)^{xf^{x-1}}))^3$
${((3 = 0)^\aleph)^{3f^{2}}}$
$(0^{\aleph})^{3f^2}$





$(0^a)^b = b$
$(\aleph^a)^b = a$

$((x.y.y)^1)^2$

$()




${((3 = 0)^\aleph)^{3f^{2}}}$

$3(2^{f})^{\aleph^{3 = 0}}$
$3(2^{f})^1$
$3(2(1^f)^{\aleph^{2=0}})$
$3(2(1^f)^1)$
$3(2(1(0^f)^{\aleph^{1=0}}))$
$3(2(1(0^f)^1))$

$0^f$

$b^{a^\aleph} = a$

$b^{a^{x. y. x}}$
$b^{y.a}$
$a$

$\text{factorial} := Y (f.x.((x = 0)^{1})^{x f^{x - 1}})$
$f; x. (x(x - 1)^f)^{\large 1^{\huge x = 0}}$

$f; x. (x = 0)[1][x f[x - 1]]$

$f; x. (x(x - 1)[f])[1[x = 0]]$




$d. f^x = d. f^{x - d} + d(\nabla^{f^{x- d}})$

$d x[f[\nabla]] = (x - d)[f] + x[f]$

$x[f[\nabla]] = d[-1]((x - d)[f] + x[f])$
$f[\nabla] = x\mapsto d[-1]((x - d)[f] + x[f])$
$\nabla = (d,f,x) \mapsto d[-1]((x - d)[f] + x[f])$


$\nabla := (d,f,x) \mapsto d[-1]((x + d)[f] - x[f])$
$\nabla := d.f.x. d[-1]((x + d)[f] - x[f])$

$\nabla := d.f.x.d^{-1}((x + d)^f - x^f)$


$-1 + 1 = 0$
$(n.m.f.x.nf(mfx))(-1)(f.x.f x) = f.x.x$
$f.x.(-1)f(fx) = f.x.x$

$(-1)f(fx) = x$

$(x^f)^{f^{-1}} = x$

$ff^{-1} = f^{-1}f = 1$






$f(a)(b) \mapsto b^{a^f}$
$x. f(x) \mapsto x.x^{f}$


# Holy shit

$(=) := a.b. b^{0\aleph b^a}$

$1 = 2 := 2^{0\aleph 2}$

$1 = 2 := 1^{\aleph 2}$

$1 = 2 := (x.1)^2$

$1 = 2 := (x.1)^{f.x.x^{ff}}$

$1 = 2 := x.x^{(x.1)(x.1)}$

$1 = 2 := x. 1^{x.1}$

$1 = 2 := x.1$

$1 = 2 := x.y.y$

$1 = 2 := 0$



#### ignore this

$1 = 2 := ((2^0)^\aleph)^{2^1}$

$1 = 2 := (1^\aleph)^2$

$1 = 2 := (x. 1)^2$

$1 = 2 := (y. 1)^{f.x.(x^f)^f}$

$1 = 2 := x.(x^{y.1})^{y.1}$

$1 = 2 := x. 1$

$1 = 2 := x.y.y$

$1 = 2 := 0$





# -1 equals itself?

$-1 = -1 := (((-1)^0)^\aleph)^{(-1)^{-1}}$
$\aleph = (1^\aleph)^{-1}$
$(1^\aleph)\aleph = 1$
$(x. 1)\aleph = 1$
$(x.1)(a.b.a) = f.f$
$f.(1)^{b.f} = f.f$
$f.f = f.f$
$\checkmark$

$\aleph = (-1 = -1)$
$\aleph = (-1)[-1][\aleph[0[-1]]$
$\aleph = (-1)[\aleph[0[-1]]]$
$\aleph = (-1)[\aleph[1]]$
$\aleph = (-1)[\aleph[1]]$
$\aleph[1]\aleph = f.f$
$f.\aleph[f](\aleph[1][f]) = f.f$
$f.f = f.f$
$\checkmark$

$\aleph = (-1 = -1)$
$\aleph = (-1)(-1)(\aleph(0(-1)))$
$\aleph = (-1)(\aleph(0(-1)))$
$\aleph = (-1)(\aleph 1)$
$(\aleph 1) \times \aleph = (\aleph 1)\times (-1)(\aleph 1)$
$(\aleph 1)\times \aleph = 1$
$f.\aleph f(\aleph 1 f) = f.f$
$f.f = f.f \quad (1 = 1)$
$\checkmark$
8




$s^1 = (x.-1)^{(-1)^{-1}}$

$s^{-1} = (x.-1)^{1}$

$s^{-1} = (x. -1)$

$1 = s(x. -1)$

$n.m.f.n f(m f)$

$1 = f.(f^s)^{-1}$

$f.f = f.(f^s)^{-1}$
$f.x.f^s = f.-1$


(assuming $s$ is $\aleph$)
$f.x.(y.f) = f.-1$

$f.x.y.f = (-1)^\aleph$
$\aleph + 1 = (-1)^\aleph$







$n.f.x.f = n.f.n^{-1}$
$n.f.n(x.f) = n.f.1$

$n.f.g.(g^n)^{f} = n.f.h.x.x^h$
$g = h$

$n.f.g.(g^n)^f = n.f.g.g$
$






$c = a^b$
$x.c = b$






$g.g = f.(f^s)^{-1}$

$g.f^sg = f.1$

$g.h.(h^g)^{h^{f^s}} = f.x.x$

$g = f,\quad h = x$

$f.x.(x^f)^{x^{f^s}}  = f.x.x$





$(f^s)^{-1} = f$

$1 = f^sf$
$f^sf = 1$

$s = -1$

$g.(g^{f^s})^{g^f} = 1$
$(g^{f^s})^{g^f} = g$




$1 + (-1) = 0$
$(+)(a.a)(-1) = f.x.x$
$f.x.(a.a)f((-1)fy) = f.x.x$
$f.x.f((-1)fx) = f.x.x$
$f.x.(f((-1)fx) = x)$



$(+) = n.m.f.x.(x^{f^m})^{f^n}$

$1 + (-1) = 0$
$1^{(-1)^{+}} = 0$
$f.x.(x^{f^1})^{f^{-1}} = f.x.x$
$f.x.((x^f)^{f^{-1}} = x)$
$f.x.(f^{-1} = x^f.x)$

$${f.x.(-1 = f.x^f.x)}$$

$-1 = 2.1.1$
$2^{-1} = 1.1$

$(1.1) + (1.1) = 1$
$f.x.(x^{f^{1.1}})^{f^{1.1}} = f.x.x^f$
$f.x.((x^{f^{1.1}})^{f^{1.1}} = x^f)$
$1.x.((x^1)^1 = x^1)$
$1.x.(x = x)$
$1.x.\aleph\quad \checkmark$

${f.x.(-1 = f.x^f.x)}$

$n.f.x(-n = n(f.x^f.x))$

$n.f.x(-n = g.(g^n)^{g^{-1}})$
$n.(-n = f.(f^n)^{f^{-1}})$

or

$n.(-n = f.(f^{-1})^{f^n})$

$n = 0^{\text{succ}^n}$

$\text{Nat} := p;n.(n = 0 \text{ or } p(n - 1))$
$\text{Nat} := p; n. ((n - 1)^{(0^{n^{=}})^\text{or}})$

$\text{Nat} := p; n. ((n - 1)[0[n[=]][\text{or}]])$

$\text{Nat} := p; n. \text{or}(=n\:0)(p(-\:n\:1))$



$\text{Nat}(2) = (0 \text{ or } 1^{p; n. (n = 0 \text{ or } p(n - 1))})$
$\text{Nat}(2) = (0 \text{ or } 0^{p;n.(n = 0 \text{ or } p(n - 1))})$
$\text{Nat}(2) = (\aleph \text{ or } (-1)^{p;n.(n=0 \text{ or } p(n-1))})$
$\text{Nat}(2) = \aleph$

$\text{Nat} := p; n. (n = 0) \text{ or } p(n - 1)$

${f.x.(-1 = f.(fx).x)}$

$(f, x) \to (-1 := (f,(fx)) \mapsto x)$

$f.x.(-1 := [f].[fx].x)$

$-1 := f.([f]x).x$

$-1 + 1$
$(f.([f]x).x) + (x.x)$
$f.x.(f.([f]x).x)f((x.x)fx)$
$f.x.(f.([f]x).x)f(fx)$
$f.x.((fx).x)(fx)$
$f.x.x$



$f((-1)f)$
$f((f.[f]x.x)f)$
$f(fx.x)$

Let $f$ = 2:

$2(2x.x)$
$(f.x.f (fx))(2x.x)$
$y.(2x.x)((2x.x)y)$
$y.(2x.x)(x[y/2x])$

$y.x[x[y/2x]/2x]$
p



$(-1) + 1$
first, add the context:
$f.x.([f].[fx].x + a.a)$
$f.x(g.y.([f].[fx].x)g((a.a)gy))$
$f.x(g.y([f].[fx].x)g(gy))$
for this to match, $g$ must equal $f$:
$f.x.(y.([f].[fx].x)f(fy))$
$f.x.(y.([fx].x)(fy))$
for this to match, $y$ must equal $x$:
$f.x.([fx].x)(fx)$
$f.x.x$
$0$

$(-1) + 2$
first, add the context:
$f.x.([f].[fx].x + a.b.a (ab))$
$f.x(g.y.([f].[fx].x)g((a.b.a (ab))gy))$
$f.x(g.y([f].[fx].x)g(g(gy)))$
for this to match, $g$ must equal $f$:
$f.x.(y.([f].[fx].x)f(f(fy)))$
$f.x.(y.([fx].x)(f(fy)))$
for this to match, $fy$ must equal $x$:
$f.x.([fx].x)(fx)$
$f.x.x$
$0$




$((a.b).c)x$
$c[x/(a.b)]$





$(-1)f \circ f = 1$
Expand $1$ and $\circ$:
$x.f((-1)fx) = x.x$
Expand $-1$:
$x.f((g.[g]y.y)fx) = x.x$
$x.f((fy.y)x) = x.x$
Expand $x$ to be $fa$:
$fa.f((fy.y)(fa)) = fa.fa$
$fa.fa = fa.fa$
$\aleph$


# We're all gonna die (eventually)

$\text{Mortal} = x.(\text{Human }x)\aleph(\text{Mortal }x)$

If the equality expression is true, then it means that $\text{Mortal}$ itself has to always return $\aleph$ if $x$ is a $\text{Human}$. If the equality expression is false, we can't say anything.

$\text{not}(\text{not}(\text{Cat }x) = x.\text{not}((\text{Cat }x)\aleph(\text{not }(\text{Orange }x))))$
$x.\text{not}((\text{Cat }x)\aleph(\text{not}(\text{Orange }x)))$
$x.\text{not}((\text{Cat }x)\aleph(\aleph (0 (\text{Orange }x))))$
$x.\aleph(0((\text{Cat }x)\aleph(\aleph(0(\text{Orange }x)))))$



$\text{Mortal} = x.(\text{Human }x)(\text{Mortal }x)0$

$\text{Mortal} \neq x.(\text{Human }x)0(\text{Mortal }x)$

$\text{Orange} \neq x.(\text{Cat }x)0(\text{Orange }x)$


$p; x. (\text{Human }x)(px)0$

$(\text{Human }x \implies \text{Mortal }x).x$

$(x. \text{Nat }x \implies \text{Nat}(2 \times x)) = \text{Nat}$

$n.(n = 0) \text{ or } \text{Nat}(n - 1) = x.(x = 0) \text{ or } \text{Nat}(x - 1) \implies (2\times x = 0) \text{ or } \text{Nat}(2\times x - 1)$
$n.\text{Nat}(n - 1) \implies \text{Nat}(2\times n - 1)$

If we know $\text{Nat}(a + b)$ implies $\text{Nat }a \text{ and } \text{Nat }b$, then if we assume $\text{Nat}(n- 1)$, and $\text{Nat }{n}$, then $\text{Nat}(2\times n - 1) = \text{Nat}(n + (n - 1))$.





$Ax(Bx)00\aleph$
If $Ax$ is $\aleph$
$\aleph(Bx)00\aleph$
$(Bx)0\aleph$



$\text{Nat} = p;n.(n = 0)\aleph(p(n - 1))$

$p; n. (\text{Nat }n)(p(n + 1))(p n)$

$X n = X (n + 1)$






$\text{Human }x \implies \text{Nat}(\text{age }x)$
$\text{Human } \text{Ian} \implies \text{Nat}(\text{age }\text{Ian})$
$\aleph \implies \text{Nat }17$
$\aleph \implies \aleph$
$\aleph$



# Tying it back to GA

$e_1^2 = 1$
$2(e_1) = 1$
$2 = e_1.1$

$e_1^{f.x.(x^f)^f} = x.x$
$x.(x^{e_1})^{e_1} = x.x$
$x.((x^{e_1})^{e_1} = x)$

$[e_1]2 = 1$
$[e_1](f.x.[[x]f]f) = 1$
$x.[[x]e_1]e_1 = x.x$
$x.([[x]e_1]e_1 = x)$


$f(t) = f(t - f'(\epsilon)) + \epsilon f'(t)$
$[t]f = [t - \epsilon]f + \epsilon [t][f]\nabla$

$f[t] = f[t - \epsilon] + \epsilon\nabla[f][t]$
$f[t] = f[0] + \epsilon\nabla[f][0] + {\dots} + \epsilon\nabla[f][t - \epsilon]$
$ft = f0 + \epsilon \times \nabla f 0 + {\dots} + \epsilon \times \nabla f (t - \epsilon)$
$f[t] = (t = 0)(f[t])(f[t - \epsilon] + \epsilon\nabla[f][t - \epsilon])$
$f = t.(t=0)(ft)(f(t - \epsilon) - \epsilon\times\nabla f(t - \epsilon))$

---
$$\large g; f.t. ((t=a)  \text{ ? }a^f \text{ : }(t - \epsilon)^g + \epsilon(t - \epsilon)^{f^\nabla})$$



