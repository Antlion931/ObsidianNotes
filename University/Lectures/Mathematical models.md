#theoreticalInformatics #pwr #math 
# Primitive recursive function

## Composition operator
We have $f: N^m \rightarrow N$ and $g_1, g_2, ..., g_m: N^k \rightarrow N$, composition of $f, g_1, g_2, ..., g_m$ we are calling a function $h: N^k \rightarrow N$ defined for those $x \in N^k$ that:
1. are defined for all $f$, $g$.
2. If $(\forall_i) y_i = g_i(x)$ then $f(g_1, ..., g_n)$ is defined

Then $h(x) = f(g_1(x), ..., g_m(x))$.

## Minimum operation
We have $f: N^{n+1} \rightarrow N$. We will define $h: N^n \rightarrow N$ as $h(x_1, ..., x_n) = (\min{y}) f(x_1, ..., x_n, y) = 0$

## Projection function
Function $I_{n,k} : N^n \rightarrow \mathbb{N}$ is projection of $k$ operand, $I_{n, k}(x_1, ..., x_n) = x_k$

## Characteristic function
Function $ch_x : \mathbb{N}_n \rightarrow \{0, 1\}$ is characteristic function of $X \subseteq N^n$ if $(\forall x \in X) x \in X \iff ch_x(x) = 0$

## Primitive recursive functions
'Klasa' function 'rekurencyjnych' is the smallest in terms of inclusion 'klasa' function 'częściowych', with 'dziedzina' 'zawartych' in 'kartezjański' product of:
- natural numbers
- 'wartościach naturalnych'
Which contains:
1. All $I_{n,k}$ functions
2. function 'charakterystyczna relacji' of minority $h: N^2 \rightarrow \{0, 1\}$
3. $+: N^2 \rightarrow N$ and $\times: N^2 \rightarrow N$ (addition and multiplication)
And doesn't contain 'złożenia' and minimum operation.

## Example
$h(x, y, z) = f(z, g(y, x), x, x)$
$h(x, y, z) = f(I_{3,3}(x,y,z), g(I_{3,2}(x,y,z), I_{3,1}(x,y,z)), I_{3,1}(x,y,z), I_{3,1}(x,y,z))$

We can do permutation of variables, skipping variable or duplicate variable.

- [ ] #todo Continue lecture and try to understand what's going on.
