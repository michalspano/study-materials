---
title: Translating Mathematical Functions To Code With Time Asymptotic Analysis
author: Michal Špano
date: 2022-04-19
papersize: a4
fontsize: 11.5pt
colorlinks: true
geometry: margin=1.25cm
output: pdf_document
---

Suppose the following for some finite $k$, $M=\{m_{1},m_{2},\dots,m_{k}\} \land N=\{n_{1},n_{2},\dots,n_{k}\}$:

$$
f(k)=\prod_{i=1}^{k}\sum_{j=1}^{k} \Big( m_{i} \times n_{j} \Big)
$$

The given **function** can be similarly expressed as:

$$
f(k)=\Big( \sum_{j=1}^{k} m_{1}\times n_j \Big)\times \Big( \sum_{j=1}^{k} m_{2}\times n_{j} \Big)\times \dots \times \Big( \sum_{j=1}^{k} m_{k-1}\times n_{j} \Big)\times \Big( \sum_{j=1}^{k} m_{k}\times n_j \Big)
$$

Or even more explicitly:

$$
f(k)=\Big[(m_{1} \times n_{1}) + (m_{1} \times n_{2}) + \dots + (m_{1} \times n_{j})] + \dots + [(m_{i} \times n_{1}) + (m_{i} \times n_{2}) + \dots + (m_{i} \times n_{j}) \Big]
$$

### Code translation in `Python3`
The proposed function $f(k)$ is implemented below.

```py
"""
Code translation in Python3
Suppose M, N are lists of some fixed size k
"""

product: int = 1
for m_i in M:
	sum_buffer: int = 0.
	for n_j in N:
		sum_buffer += (m_i * n_j)
	product *= sum_buffer
	
```

### Code analysis
Let `product` be $1$ in the initial state, that is, for some value $v_1$ computed in the first iteration of the outer `for` loop holds: `product` $=v_1$. Thus, `product` $=\prod_{i=0}^{k} v_{i}$ for $k$-th iteration. Furthermore, let `sum_buffer` (previously indicated as $v_i$) be initially $0$ in each iteration of the outer `for` loop, so for each iteration in the inner `for` loop, `sum_buffer` equals to the sum of all terms of $N$, namely $n_j$, multiplied by some current constant $m_{c}$, thus `sum_buffer` $=\sum_{j=1}^{k} m_{c} \times n_{j}$, where $c$ is a constant and $c\leq k$. 

### Time complexity
According to **asymptotic analysis**, the lower and the upper bounds of such algorithm remain **identical**, and, undeniably, any case holds the same running time complexity. Thus, we compute the average (and, frankly, the only possible) running time  as $\Theta(k^2)$ where the only variable affecting the real running speed is the value of $k$. Assume the parabolic function $g(k)=k^2$, where $k$ is an integer and $k\geq1$.