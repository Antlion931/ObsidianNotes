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
  - $h$ - machine returns a belt

## Example
[[deterministic Turing machine]] to recognise palindrom in alphabet $\{0, 1\}$. Let's represent it with a tabel of transition function.

| $\sigma$ |            $0$<br>             |              $1$               |          $\sqcup$<br>          |
|:---------|:-------------------------------|:-------------------------------|:-------------------------------|
|  $q_0$   |  $(q_1, \sqcup, \rightarrow)$  |  $(q_2, \sqcup, \rightarrow)$  |             $yes$              |
|  $q_1$   |    $(q_1, 0, \rightarrow)$     |    $(q_1, 1, \rightarrow)$     |  $(q_3, \sqcup, \leftarrow)$   |
|  $q_2$   |    $(q_2, 0, \rightarrow)$     |    $(q_2, 1, \rightarrow)$     |  $(q_4, \sqcup, \leftarrow)$   |
|  $q_3$   |   $(r, \sqcup, \leftarrow)$    |              $no$              |             $yes$              |
|  $q_4$   |              $no$              |   $(r, \sqcup, \leftarrow)$    |             $yes$              |
|  r       |      $(r, 0, \leftarrow)$      |      $(r, 1, \leftarrow)$      |  $(q_0, \sqcup, \rightarrow)$  |     
-  Check what is the first element?  
   - If $0$, delete it, go to end.  
     - If $0$, delete it, return to beginning.  
     - If $1$, isn't a palindrom.  
     - If $\sqcup$, precious element was the last, odd length, palindrom  
   - If $1$, delete it, go to end.  
     - If $1$, delete it, return to beginning.  
     - If $0$, isn't a palindrom.  
     - If $\sqcup$, precious element was the last, odd length, palindrom  
   - If $\sqcup$, it is a palindrom

Solution: $(\{q_0, q_1, q_2, q_3, q_4, r\}, \{0, 1\}, \sigma, q_0\}$
Time complexity: $O(|x|^2)$

  

