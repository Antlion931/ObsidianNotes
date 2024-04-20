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
- ada uses `/=` instead of `!=`

## Compiling C
Although you could compile everything with just a [[gcc]] or other compiler, it could be a very cumbersome. That's why people make a [[make]], which will automate this process. And then people make [[cmake]] to automate writing a [[make]]. What a time to be alive!  

## Compiling ada
To compile ada I have used [[gnatmake]], because things that I was suppose to do were very simple.

## Compiling rust
In rust ecosystem you should use a [[cargo]] to compile your program and manage your dependencies.

- [ ] #todo Write about wrapping C, ada and rust libraries