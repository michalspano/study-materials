# Integrals exercise 1

Given is the function $f(x)=\frac{1}{4}\sin(2x)+3$.

a) Evaluate the **indefinite** integral
b) Evaluate the **definite** integral over a period
___

a) The **indefinite** integral

$\int f(x) dx=\int [\frac{1}{4}\sin(2x)+3]dx=\int [\frac{1}{4}\sin(2x)]dx + \int[3]dx=\frac{1}{4}\int [\sin(2x)]dx + \int[3]dx$

1.  Evaluate $\frac{1}{4}\int [\sin(2x)]dx$

Let $u=2x$, thus $\frac{1}{4}\int [\sin(u)]dx$.  

$\cfrac{du}{dx}=2x$
$du = [2x]dx$
$du = 2 dx$
$\frac{1}{2}du = dx$

$\Rightarrow \frac{1}{8}\int [\sin(u)]du$
$\frac{1}{8}\int [\sin(u)]du=\frac{1}{8}\int -\cos(u)=\frac{1}{8}\int -\cos(2x)=-\frac{1}{8}\int \cos(2x)$

2. Evaluate $\int[3]dx=\int 3x$

Lastly, evaluate the complete integral, $\int f(x)=-\frac{1}{8}\int \cos(2x) + \int 3x = 3x -\frac{1}{8}\cos(2x)+c$

**Solution**: $\int f(x) = 3x -\frac{1}{8}\cos(2x)+c$
___

b) The **definite** integral over a period

The period of $f(x)$ is $\pi$, since  $\sin(2x) \iff period=\frac{2\pi}{2}=\pi$

$\int_{0}^{\pi} f(x) = \int_{0}^{\pi} [\frac{1}{4}\sin(2x)+3]dx = -\frac{1}{8}\int_{0}^{\pi} \cos(2x) + \int_{0}^{\pi} 3x = -\frac{1}{8} \big[ \cos(2x) \big]_{0}^{\pi} + \big[3x \big]_{0}^{\pi}=-\frac{1}{8} [0\pi] + [3\pi - 0\pi]$

$=3\pi$

**Solution**: $3\pi$
