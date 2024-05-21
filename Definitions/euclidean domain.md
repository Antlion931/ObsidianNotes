#algebra  #pwr 

[[integral domain]] $(X, +, \times)$ is [[euclidean domain]] if there exist $N: X\\\{0\} \implies \mathbb{N}$ such that:
1. $(\forall a,b) (b \ne 0 \implies (\exists q,r)(a = q \times b + r \land (r = 0 \lor ( r \ne 0 \land N(r) < N(b)))))$
2. $(\forall a,b \ne 0)(N(a) \le N(a \times b))$

You can think about it as a [[integral domain]] where we have defined division with remainder.

## Examples
- For $\mathbb{z}$, $N(k) = |k|$
- For $\mathbb{Z}[i]$ ([[Gaussian integers]]), $N(a + bi) = a^2 + b^2$
  In proof we need to consider to which point we will round.

- [ ] #todo Continue lecture from 32 minute, and another example
