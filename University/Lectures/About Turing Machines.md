#math #pwr #theoreticalInformatics 

# Definition
![[deterministic Turing machine]]

# Definition
For [[deterministic Turing machine]] $M$, and word $x$, result of $M$ with word $x$ we indicate as $M(x)$.
- $M(x) = yes$, machine accepted word $x$.
- $M(x) = no$, machine didn't accepted word $x$.
- $M(x) = y$, machine stopped is state $h$, and returned belt without unnecessary $\sqcup$.
- $M(x) = \uparrow$, machine didn't stopped.
## Example

$M(bin(n)) = bin(n + 1)$, adding one in binary

|  $\sigma$  |           $0$           |           $1$           |           $\sqcup$           |
|:-----------|:------------------------|:------------------------|:-----------------------------|
|    $q$     |  $(q, 0, \rightarrow)$  |  $(q, 1, \rightarrow)$  |  $(s, \sqcup, \leftarrow)$   |
|    $s$     |  $(r, 1, \leftarrow)$   |  $(s, 0, \leftarrow)$   |         $(h, 1, \_)$         |
|    $r$     |  $(r, 0, \leftarrow)$   |  $(r, 1, \leftarrow)$   |  $(h, \sqcup, \rightarrow)$  |  
#### Interpretation
- $q$ - means go to end, then $s$.
- $s$ - add one from left.
- $r$ - go to the beginning if needed.

It works for $0$, and all other binary numbers that starts with $1$.

# Definition
Configuration of [[deterministic Turing machine]] $M$ we name a triple $(q, \alpha, \beta)$ where  $q \in Q \cup \{ yes, no, h\}$, $\alpha$ and $\beta \in (\Sigma \cup \{\sqcup\})^*$

- [ ] #todo Watch lecture from 43 minute,