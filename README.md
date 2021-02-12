# Kenyon’s Tilings From Free Group Endomorphisms
* This project isinspired by the paper [The Construction of Self-Similar Tilings](https://arxiv.org/pdf/math/9505210.pdf).

## Methodology
1. Input three integers $p,q,r$. These define the polynomial:
$\lambda^n -p\lambda^{n-1} + q\lambda + r = 0$
2. Find the complex Perron number for the given polynomial.
3. Using this root, construct the free group (and the resulting parallelograms) given by: 
$F(a_1,a_2, \cdots, a_n)$ where $a_1=1, a_2=\lambda, \cdots, a_n = \lambda^{n-1}$.
4. Solve the endomorphism $\phi (F(a))$:

$\phi(a_i) = 
\begin{cases}
\phi(a_i) = a_{i+1},\quad \text{for } 1 \leq i \leq n - 1\\
\phi(a_i) = a_n^p a_1^{-r} a_2^{-q},\quad \text{for } i = n
\end{cases}$

5. Use repeatedly applying this endomorphism to a parallelogram in the free group (such as $[a_1,a_2]$), we can approximate the translation-self-similar tiles (and graph them).
