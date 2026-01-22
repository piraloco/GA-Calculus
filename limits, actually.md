
$$\lim_{h\to 0} \frac{f(x + h) - f(x)}{h}$$

We say that $\lim_{x→a} f(x) = L$ if: For every $\epsilon > 0$, there exists a $\delta > 0$ such that whenever $0 < |x - a| < \delta$, we have $|f(x) - L| < \epsilon$.

$$\forall \epsilon > 0\ \exists \delta > 0\ (0 < |x - a| < \delta) \implies |f(x) - L| < \epsilon$$

$\forall \epsilon > 0 \ \exists \delta > 0 (0 < |h| < \delta) \implies |\frac{f(x + h) - f(x)}{h} - f'(x)| < \epsilon$

$\frac{f(x + \epsilon) - f(x)}{\epsilon}$
$\frac{f(x + \epsilon)\epsilon - f(x)\epsilon}{0}$
$\frac{f(x)\epsilon + f'(x)\epsilon^2 - f(x)\epsilon}{0}$

$f(0) = 1$
$f'(0) = 0$
$f''(t) = -f(t)$

$f(0) = 1$
$f(\epsilon) = 1$
$f(t + 2\epsilon) - f(t + \epsilon) - f(t + \epsilon) + f(t) = -f(t)\epsilon^2$
$f(t + 2\epsilon) + f(t) + f(t)\epsilon^2 = 2f(t + \epsilon)$

$f(0) = 1$
$f(\epsilon) = 1$
$f(t + 2\epsilon) + (1 + \epsilon^2)f(t) = 2f(t + \epsilon)$
$f(\frac{1}{\epsilon} + 2\epsilon) + (1 + \epsilon^2)f(\frac{1}{\epsilon}) = 2f(\frac{1}{\epsilon} + \epsilon)$
$f(\frac{1 + 2e^2}{\epsilon}) + (1 + \epsilon^2)f(\frac{1}{\epsilon}) = 2f(\frac{1 + \epsilon^2}{\epsilon})$
$f(\frac{1}{\epsilon}) + (1 + \epsilon^2)f(\frac{1}{\epsilon}) = 2f(\frac{1}{\epsilon})$
$x + x + x\epsilon^2 = 2x$

$f(5) = 2f(5 - \epsilon) - (1 + \epsilon^2)f(5 - 2\epsilon)$
$f(5 - \epsilon) = 2f(5 - 2\epsilon) - (1 + \epsilon^2)(5 - 3\epsilon)$
$f(5) = 2(2f(5 - 2\epsilon) - (1+\epsilon^2)f(5 - 3\epsilon)) - (1+\epsilon^2)f(5 - 2\epsilon)$
$f(5) = 4f(5 - 2\epsilon) - (1 + \epsilon^2)f(5 - 3\epsilon)  - (1 + \epsilon^2)f(5 - 2\epsilon)$
$f(5) = 4f(5 - 2\epsilon) - (1 + \epsilon^2)(f(5 - 3\epsilon) - f(5 - 2\epsilon))$
$2f(t-\epsilon) - (1 + \epsilon^2)f(t - 2\epsilon) = 4f(t - 2\epsilon) - (1 + \epsilon^2)(f(t - 3\epsilon) - f(t - 2\epsilon)$
$2f(t - \epsilon) + (1 + \epsilon^2)(f(t - 3\epsilon) - f(t - 2\epsilon)) = 4f(t - 2\epsilon) + (1+\epsilon^2)f(t - 2\epsilon)$
$2f(t - \epsilon) + f(t - 3\epsilon) - f(t - 2\epsilon) + f(t- 3\epsilon)\epsilon^2 - f(t - 2\epsilon)\epsilon^2 = 4f(t - 2\epsilon) + f(t - 2\epsilon) - f(t - 2\epsilon)\epsilon^2$
$2f(t - \epsilon) + f(t- 3\epsilon) + f(t - 3\epsilon)\epsilon^2 + f(t - 2\epsilon)\epsilon^2 = f(t - 2\epsilon )+ f(t-2\epsilon)\epsilon^2 + 4f(t-2\epsilon) + f(t - 2\epsilon)$
$2f(t - \epsilon) + f(t - 3\epsilon) + \epsilon^2(f(t - 3\epsilon + f(t - 2\epsilon))$


$2f(5-\epsilon) = 4f(5 - 2\epsilon)$
$f(5-2\epsilon) = f(5 - 3\epsilon) - f(5 - 2\epsilon)$
$2f(5 - 2\epsilon) = f(5 - 3\epsilon$)

$2f(5-\epsilon) = 2f(5 - 3\epsilon)$

$2f(t) = 2f(t - 2\epsilon)$

---

$f(t) = f(t - 2\epsilon)$

$f(0) = 1$
$f(\epsilon) = 1$
$f(t) + f(t) + f(t)\epsilon^2 = 2f(t + \epsilon)$
$(2 + \epsilon^2)f(t) = 2f(t + \epsilon)$
$f(t) = \frac{2f(t + \epsilon)}{2 + \epsilon}$
$f(t) = \frac{(2 - \epsilon)2f(t + \epsilon)}{4}$
$f(t) = f(t + \epsilon) - \frac{1}{2}\epsilon f(t + \epsilon)$
$f(t) = (1 - \frac{1}{2}\epsilon)f(t + \epsilon)$
$f(t) = (1 - \epsilon)f(t + 2\epsilon)$
$f(t) = (1 - \epsilon)f(t)$

$f(t + \epsilon) = \frac{(2 + \epsilon^2)f(t)}{2}$
$f(t + \epsilon) = f(t) + \frac{\epsilon^2}{2}f(t)$

---

$f(0) = 1$
$f'(0) = 0$
$f''(t) = -f(t)$

$f(0) = 1$
$f(\epsilon) = 1$
$f'(t + \epsilon) - f'(t) = -f(t)\epsilon$
$f'(t + \epsilon) + f(t)\epsilon = f'(t)\epsilon$

$f(0) = 1$
$f(\epsilon) = 1$
$f(t + 2\epsilon) - f(t + \epsilon) + f(t)\epsilon^2 = f(t + \epsilon) - f(t)$
$f(t + 2\epsilon) + f(t)\epsilon^2 + f(t) = 2f(t + \epsilon)$
$f(t) = 2f(t - \epsilon) - (1 + \epsilon^2)f(t - 2\epsilon)$

---

$f''(t) = -f(t)$

$\nabla^2f(t) = -f(t)$

$f(t) = t$
$\nabla f(t) = 1$

$f = t_1$
$\nabla t_1 = t_0$
$\nabla t_2 = 2t_1$

$\nabla t_0 = 0$
$t_0^2 = 0$

$\nabla f_1 = f_0$
$\nabla = f_{01}$

$\nabla t_0 = 0$
$\nabla t_1 = t_0$
$\nabla t_2 = 2t_1$

$\nabla t_0 \nabla = 0$
$\nabla t_1 \nabla = t_0$

$\nabla t_{n+1} = (n+1)t_n$
$t_n = \frac{\nabla t_{n+1}}{n+1}$
$t_{n+1} = \nabla^{-1}(n+1)t_n$

$t_{n+1} = (n+1)St_n$

$e_t, S$

$Se_t + 2S^2e_t$
$t_1 + t_2$

$s + 2s^2$ represents $x + x^2$

$1 + 2s$

$St + 2S^2t$
$t + 2St$

$t$
$St$
$S^{-1}(St) = t$
$S^{-1}(t) = 0$

$s^2 + 2s^3$ represents $x + x^2$
$s + 2s^2$ represents $1 + 2x$
$1 + 2s$ represents $2$

$1 \Rightarrow 0$
$s \Rightarrow 1$
$s^2 \Rightarrow x$
$2s^3 \Rightarrow x^2$
$6s^4 \Rightarrow x^3$
$24s^5 \Rightarrow x^4$
$n!s^{n+1} = x^n$

$s^{n+1} = \frac{x^n}{n!}$
$\exp = s + s^2 + s^3+\dots$

$\exp s = \text{exp} - s$

$\exp = (1 + \exp)s$

$\exp^2 = \cosh$
$\exp^2s = \sinh$

$\cosh s = \sinh$

$\exp^2i = \cos$
$\exp^2is = \sin$

$ks^2 = -k$
$(s - s^3 + s^5 - \dots)s^2 = s^3 - s^5 + \dots$




$s^n \Rightarrow \frac{x^n}{n!}$
$s^{-n} \Rightarrow 0$

$\exp =\ \dots\,+ s^{-1} + 1 + s + s^2 + \dots$

$\cosh = \exp^2$
$\sinh = \exp^2 s$

$\cos = (\exp i)^2$
$\sin = (\exp i)^2 s$

$\cos = \exp^2i$

$s_n(x) = \frac{x^n}{n!}$

$\exp_0 = 1$
$\exp_{n+1} = s\exp_n$

$\exp = \sum s^n$
$\cosh = \sum s^{2n}$
$\sinh = \sum s^{2n+1}$

$\exp = 1 \odot n$
$\cosh = 1 \odot 2n$
$\sinh = 1 \odot (2n + 1)$
$\cos = i \odot 2n$
$\sin = i \odot (2n + 1)$

$\cosh + \sinh = 1\odot 2n + 1 \odot (2n + 1)$
$1\odot n = 1 \odot 2n + 1\odot (2n + 1)$

$\sum s^n = (\sum s^{2n})(1 + s)$
$\sum s^n = \sum s^{2n} + s^{2n + 1}$

$\sum s^n = \sum_2 s^n + s^{n+1}$

$\exp = 1 + s + s^2 + s^3 + s^4 + \dots$

$\exp = 1 + s\exp$
$\cosh = 1 + s^2\cosh$
$\sinh = s + s^2\sinh$
$\cosh + \sinh = 1 + s^2\cosh + s + s^2\sinh$
$\cosh + \sinh = 1 + s(1 + s(\cosh + \sinh))$
$\cosh + \sinh = 1 + s + s^2(\cosh + \sinh)$

$\exp = \boxed{1 + s \square}$

$\cosh + \sinh = \boxed{1 + s^2\square} + \boxed{s + s^2\square}$
$\cosh + \sinh = 1 + s^2\cosh + s + s^2\sinh$
$\cosh + \sinh = 1 + s(1 + s(\cosh + \sinh))$

$x = 1 + s + s^2x$
$x(1 - s^2) = 1 + s$
$x(1 + s)(1 - s) = 1 + s$
$x(1 - s) = 1$
$x - sx = 1$
$x = 1 + sx$


$\cos + \sinh = 1 - s^2\cos + s + s^2\sinh$
$\cos + \sinh = 1 + s + s^2(-\cos + \sinh)$
$\cos + \sinh = 1 + s + s^2(s^2\cos - 1 + s + s^2\sinh)$
$\cos + \sinh = 1 + s + s^2(-1 + s + s^2(\cos + \sinh))$
$\cos + \sinh + s^2(1 - s - s^2(\cos + \sinh)) = 1 + s$
$\cos + \sinh + s^2 - s^3 - s^4(\cos + \sinh) = 1 + s$
$(\cos + \sinh)(1 - s^4) = 1 + s + s^2 - s^3$
$(\cos + \sinh)(1 + s^2)(1 - s^2) = 1 + s + s^2 - s^3$
$(\cos + \sinh)(1 - s^2) = \frac{1 + s + s^2 - s^3}{1 + s^2}$
$\cos + \sinh = \frac{1 + s + s^2 - s^3}{1 + s^2} + s^2(\cos + \sinh)$
$\cos + \sinh = \frac{1 + s + s^2 - s^3 + (s^2 + s^4)(\cos + \sinh)}{1 + s^2}$


$\frac{1 + s + s^2 - s^3 + s^2x + s^4x}{1 + s^2}$
$\frac{1 + s + (1 + x)s^2 - s^3 + xs^4}{1 + s^2}$

$(1 + s^2)p = 1 + s + (1 + x)s^2 - s^3 + xs^4$
$p + s^2p = 1 + s + (1 + x)s^2 - s^3 + xs^4$
$1 + s - p + (1 + x - p)s^2 - s^3 + xs^4$
$1 + s - p + s^2((1 + x - p) - s + xs^2)$
$k + s + s^2(k + x - s + xs^2) = 0$
$s^2(k + x - s + xs^2) = -k - s$
$

$(1 + s^2)p = 1 + (1 + x)s^2 + xs^4 + s - s^3$


$(1 + s^2)(1 + p) = 1 + (1 + x)s^2 + xs^4 + s - s^3$
$p + ps^2 = s^2 + xs^4 + s - s^3$
$p +(p - 1)s^2 - xs^4 = s - s^3$
$(p + s^2)(1 - s^2) = s - s^3$

$2p

$(1+ s^2)(p + xs^2) = 1 + s + s^2 + xs^2 - s^3 + xs^4$





$p + ps^2 = 1 + s^2 - s^3$
$p(1 + s^2) = 1 + s^2 - s^3$

$(1 + s^2)(1 + p) = 1 + s^2 - s^3$
$p + s^2p = -s^3$
$p(1 + s^2) = -s^3$


$1 + s + s^2 - s^3$
$(1 + s^2) - (s^3 - 1)$

$ab = 1 + s + s^2 - s^3$
$ab = 1 + s + (1 - s)s^2$
$1 + a + b + ab = 1 + s + (1 - s)s^2$
$a + b + ab = s + s^2 - s^3$

$(1 + ai)(1 - bi) = 1 + s + s^2 - s^3$
$1 - bi + ai + ab = 1 + s + s^2 - s^3$
$ai + ab - bi = s + s^2 - s^3$
$a = s/i$
$\frac{sb}{i} - bi = s^2 - s^3$
$sb + b = s^2i - s^3i$
$b(s + 1) = s^2i - s^3i$
$b = \frac{s^2i - s^3i}{s + 1}$




$\text{cosih} = \frac{1 + s + s^2 - s^3}{1 + s^2} + s^2\text{cosih}$

$\text{cosih}(1 - s^2)(1 + s^2) = 1 + s + s^2 - s^3$
$\text{cosih}(1 - s^4) = 1 + s + s^2 - s^3$

$\text{cosih} + s^3 = 1 + s + s^2 + s^4\text{cosih}$

$F = 1 + s + s^2 - s^3 + s^4F$

$F = 1 + s + s^2 - s^3 + s^4 + s^5 + s^6 - s^7 + s^8 + \dots$




$\exp = 1 + s \exp$
$\cosh = 1 + s^2\cosh$
$\sinh = s + s^2\sinh$
$\cos = 1 - s^2\cos$
$\sin = s - s^2\sin$


$\cos = 1 - s^2 + s^4 - s^6 + s^8 - \dots$
$\sin = s - s^3 + s^5 - s^7 + s^9 - \dots$

$\cos^2 = (1 - s^2 + s^4 - \dots)(1 - s^2 + s^4 - \dots)$
$\cos^2 = (


$\cos^2 + \sin^2 = 1 - 2s^2\cos + s^4\cos^2 + s - 2s^3\sin + s^4\sin^2$
$\cos^2 + \sin^2 = 1 - 2s^2\cos + s^4\cos^2 + \sin^2$
$\cos^2(1 - s^4) + \sin^2 = 1 - 2s^2\cos + \sin^2$
$\cos^2(1 - s^4) + \sin^2(1 - s^4) = 1 + s^2 -  2s^2\cos - 2s^3\sin$
$(\cos^2 + \sin^2)(1-s^4) = 1 + s^2 - 2s^2(\cos + s\sin)$
$(\cos^2 + \sin^2)(1-s^4) + 2s^2(\cos + s^2\cos) = 1 + s^2$
$(\cos^2 + \sin^2)(1 - s^4) + 2s^2\cos(1 + s^2) = 1 + s^2$
$(\cos^2 + \sin^2)(1 - s^2) + 2s^2\cos = 1$
$-2s^2\cos = (\cos^2 + \sin^2)(1-s^2) - 1$
$2\cos = (\cos^2 + \sin^2)(1 - s^2) + 1$
$\cos^2 + \sin^2 + 1 = 2\cos + s^2(\cos^2 + \sin^2)$




$(\cos^2 + \sin^2)(1 - s^4) + 2s^2 = 1 + s^2$
$(\cos^2 + \sin^2)(1 - s^4) = 1 - s^2$
$(\cos^2 + \sin^2)(1 + s^2) = 1$
$(\cos^2 + \sin^2) = 1 - s^2(\cos^2 + \sin^2)$



$\cos^2 + \sin^2 = 1 + s - 2s^2\cos - 2s^3\sin + s^4(\cos^2 + \sin^2)$
$(\cos^2 + \sin^2)(1 - s^4) = 1 + s - 2s^2\cos - 2s^3\sin$
$(\cos^2 + \sin^2)(1 - s^2)(1 + s^2) = 1 - 2s^2\cos + s(1 - 2s^2\sin)$
$(\cos^2 + \sin^2)(1-s^2)(1





---


$\cos^2 = 1 - \frac{2^1x^2}{2!} + \frac{2^3x^4}{4!} - \dots$

$\boxed{\cos^2(x) = 1 - \frac{2x^2}{2!} + \frac{8x^4}{4!} - \frac{32x^6}{6!} + \frac{128x^8}{8!} - \cdots}$

$\cos^2(x) = 1 - 2^1s^2 + 2^3s^4 - 2^5s^6 + 2^7s^8 + \dots$
$2\cos^2 = 1 + \cos$
$4\cos^4 = 1 + 2\cos + \cos^2$




$Sx = \frac{x^2}{2}$

$$Sx^n = \frac{x^{n+1}}{n+1}$$

$F = 2s^2$

$0 \circ (1 + s + s^2) = 1$


$\text{exp} - s\,\text{exp} = 1$
$\exp(1 - s) = 1$
$\exp = 1 - \frac{1}{1 - s}$

$\exp = \frac{1}{1 - s}$

$\lim_{n\to\infty}s^n = 0$
$s^0 = 1$ 

$\exp^2 = \frac{1}{1-2s-s^2}$
$\exp^2(1 - s)(1 - s) = 1$
$\exp^2(1 - s) = \exp$
$\exp^2 - s\exp^2 = \exp$
$\exp^2 = \exp + s\exp^2$



$e = \frac{1}{1 - s}$
$e - se = 1$
$s = \frac{e - 1}{e}$




$\lim_{n\to-\infty}s^n = \frac{0}{\infty}$


$f(x + e_0v) = f(x) + e_0(v\cdot \nabla f(x))$
$f(x) = x + e_0$

$(x + e_0v) + e_0 = x + e_0 + e_0(v \cdot \nabla f(x))$
$e_0(\nabla f(x) \cdot v) = e_0v$
$\nabla f(x) \cdot v = 1 \cdot v$
$\nabla f(x) = 1$

$DSf = f$

$p = a_0 + a_1x + a_2x^2 + a_3x^3 + \dots$

$D : f \Rightarrow f'$
$DS = 1$
$a : x \Rightarrow ax$

$(Dx - xD)f = f$
$D(xf) - xDf = f$
$f + xDf = D(xf)$

$f(x) + kf'(x) = D(kf(x))$
$f(x) + kf'(x) = (kf(x))'$
$f + kf' = (kf)'$

$(kf)' = f + kf'$

$(Sf)' = f + Sf'$
$f = f + Sf'$
$Sf' = 0$


$(DX - XD)f(x) = g(x)$
$DXf(x) - XDf(x) = g(x)$

$g(x) + ABf(x) = BAf(x)$
$g + ABf = BAf$

$1 + D(xf) = x(Df)$

$f(x + e_0v) = f(x) + e_0(v\cdot \nabla f(x))$
$f(x + \epsilon v) = f(x) + \epsilon(v \cdot Df(x))$
$DS = 1$

$\text{exp}\circ 0 = 1$
$\text{exp}\circ(x + \epsilon a) = \text{exp}\circ x + \epsilon(a \cdot \text{exp} \circ x)$

$\exp(x + \epsilon a) = \exp(x) + \epsilon(a \cdot \exp(x))$
$\exp(\pi e_{12}) = e_0\exp(\pi e_{12}) - \exp(\pi e_{12} + e_0)$
$\exp(\pi e_{12}) = e_0(e_0 \exp(\pi e_{12}) - \exp(\pi e_{12} + e_0)) - \exp(\pi e_{12})$
$\exp(\pi e_{12}) = -(1 + e_0)\exp(\pi e_{12} + e_0)$
$1 + e_0 = -\frac{\exp()}

$m = 1 + (\pi e_{12}s)m$

$m = 1 

$\pi e_{12}s = \frac{m - 1}{m}$
$\pi = \frac{m - 1}{m e_{12} s}$
