# Super-factorials - Advanced methods of factorials
Guidance by [blackpenredpen](https://www.youtube.com/watch?v=7eboFOkRHr4)
___
0. **Standard** factorial

Suppose $n!$ that implies: 
$$n!=n \times (n-1)! \times (n-2)! \dots 2! \times 1!$$

More generally: 
$$n!=\prod_{k=0}^{n} (n-k)$$

1. **Double** factorial

The parity of $n$ affects the series. Suppose $n!!$, then:

$$n!!=
\begin{cases}
  n \times (n-2) \dots 4 \times 2 | even \\
  n \times (n-2) \dots 3 \times 1 | odd \\
\end{cases}
$$

Similarly expressed as:

$$n!!=
\begin{dcases}
 \prod_{k=0}^{n} (n -2 \times k) | even \\
 \prod_{k=0}^{n} (n -2 \times k) | odd \\
\end{dcases}
$$

2. **Subfactorial**

A subfactorial of $n$, denoted as $!n$, expresses the number of de-arrangements of a set with $n$ terms.

The following holds: $$!n = n! \times \big( 1-\frac{1}{1!}+\frac{1}{2!} \times \dots \times (-1)^{n} \times \frac{1}{n!}\big)$$

3. **Primorial**

Suppose a **primorial** of $n$, denoted as $n\#$, which express the series of prime numbers $p$:
$$n\# = \prod_{p \leq n} p$$

4. **Super** factorial (the _Sloane_ definition)

Suppose a **super** factorial of $n$, denoted as $sf(n)$, which expresses the series of all $k!$, such that $k \leq n$. That is:

$$sf(n)=n! \times (n-1)! \times (n-2)! \times \dots \times 2! \times 1!$$

Which is similarly expressed in the form:
$$sf(n)=\prod_{k=1}^{n} k!$$

5. **Exponential** factorial (also know as the **hyperpower**)

As the name suggests, the **exponential** factorial of $n$, denoted as $n\$$,  expresses $n$ raised to the power of $(n-1)$ that is raised to the power of $(n-2)$ and so forth. This relation is also defined with a **recurrent sequence**, such that $a_{n}= n^{a_{n-1}} \land a_{0}= 1$. For instance, the **exponential** factorial of $5$ is $5\$=5^{4^{3^{2^1}}}$.

6. **Hyper** factorial

A **hyper** factorial of $n$, denoted as $H(n)$, expresses the following series:
$$H(n)=n^n \times (n-1)^{n-1} \times (n-2)^{n-2} \times \dots \times 2^2 \times 1^1$$

Which is similarly expressed in the following form:

$$H(n)=\prod_{k=0}^{n} (n-k)^{n-k}$$

___
