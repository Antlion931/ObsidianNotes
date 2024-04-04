#math 

We have alphabet $\Sigma$ and two sequence of words from that alphabet with the same length.

$A = \{a_1, a_2, ..., a_k\}$ and $B = \{b_1, b_2, ..., b_k\}$

The question is, if there exist sequence $(i_1, i_2, ..., i_k)$ such that

$a_{i_1}a_{i_2}...a_{i_k} = b_{i_1}b_{i_2}...b_{i_k}$

we will call  $(i_1, i_2, ..., i_k)$ a solution.

## Example
### With solution

$\Sigma = \{a, b\}$
$A = (b, babbb, ba)$
$B = (bbb, ba, a)$

solution is $(2, 1, 1, 3)$

From $B$ $ba\_bbb\_bbb\_a$
From $A$ $babbb\_b\_b\_ba$

### Without solution

$\Sigma = \{a, b\}$
$A = (ba, abb, bab)$
$B = (bab, bb, abb)$

There's no solution
