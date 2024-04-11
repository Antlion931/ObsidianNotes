#programmingParadigms #pwr 

[Exercises](https://cs.pwr.edu.pl/gebala/dyd/jpp2024/labor1.pdf)
## Notes
- Make documentation for every library, with examples and edge cases
- For every language use some build tool, like cmake or cargo
- Every exercise is composed of two implementations, so just make two libraries with one testing code.
- linear Diophantine equation $aX + bY = c$, has only solutions when $gcd(a, b) | c$, and if so, there are infinite solutions to this equation. You can find one by using:
  - using extended $gcd(a,b)$, to find solutions of $ax + by = gcd(a,b)$.
  - check if $gcd(a,b)|c$, and if so find $k$ such that $gcd(a,b) \times k = c$.
  - solutions to original equation are in form of $X = kx, Y = ky$.

- [ ] #todo write function to resolve Diophantine equation in C based on extended gcd.
- [ ] #todo make a structure that will represents a solution of this equation.