# Problem Stopu
## Def
Zdecydować czy dla danej maszyny Turinga $M$ oraz słowa $x$, nasza maszyna się zatrzyma czy też nie.

$H = \{ M;x : M(x) \neq \nearrow\}$

## Twierdzenia i Lematy
1. $H$ jest rozpoznawalny.
2. $H$ nie jest rozstrzygalny.
   ### Dowód
   Przypuśćmy że maszyna $M_H$ która potrafi rozstrzygać $H$ istnieje. Na jej podstawie Zbudujmy nową maszyne:
   $D(M) = if \ M_H(M;M) = tak \ \{ return\nearrow \}  \ else \  \{ return \ tak\}$
   Rozpatrzmy teraz następujące przypadki:
   $D(D) = \nearrow \implies M_H(D;D) = tak \implies D;D \in H \implies D(D) \neq \nearrow$
   $D(D) = tak \implies M_H(D;D) = false \implies D;D \notin H \implies D(D) = \nearrow$
   Dostajemy w każdym przypadku sprzeczność, nie może więc taka maszyna istnieć.
3. Dopełnienie H nie jest rozpoznawalny.
4. Jeśli H byłby rozstrzygalny, to każdy problem rozpoznawalny byłby rozstrzygalny.
5. Język $L = \{ M : M \ zatrzymuje \ się \ na \ wszystkich \ słowach\}$ nie jest rozstrzygalny.