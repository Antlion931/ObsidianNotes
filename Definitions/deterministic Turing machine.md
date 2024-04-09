#math #theoreticalInformatics #pwr 

|       |          |          | $\downarrow$ |     |          |          |       |
|:------|:---------|:---------|:-------------|:----|:---------|:---------|:------|
| $...$ | $\sqcup$ | $\sqcup$ | $a$          | $b$ | $\sqcup$ | $\sqcup$ | $...$ |  

 Deterministic Turing machine is infinity belt and $(Q, \Sigma, \sigma, q_0)$ where:
- $Q$ - finite collection of states.
- $\Sigma$ - finite alphabet (there exist a $\sqcup$ (blank) symbol that is a default symbol on belt).
- $q_0$ - first state (Head is always on the first character of input).
- $\sigma$ - transition function is form $Q \times (\Sigma \cup \{\sqcup\}) \implies (Q \cup \{ yes, no, h\})\times(\Sigma \cup\{\sqcup\}) \times (\leftarrow, \rightarrow, \_)$
  
  You can think about it like function that takes two arguments, current state and symbol under head, returning new state (or special states), what symbol to write under head and where to move head.
  
  special symbols:
  - $yes$ - machine returns **true**
  - $no$ - machine returns **false**
  - $h$ - 

- [ ] #todo Watch lecture from 16 minute, and note what $h$ is, should be in shown in some example
  

