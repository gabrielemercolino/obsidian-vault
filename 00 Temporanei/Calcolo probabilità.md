---
tags:
  - unfinished
  - temporaneo
links: 
cssclasses:
---
# Calcolo probabilità
## Principio di inclusione/esclusione
$$P(e\cup F)=P(E)+P(F)-P(E\cap F)$$
>[!example] Esempio
>G. porta con sè 2 libri $\{L_1, L_2\}$ per le vacanze
>E="le piace $L_1$", F="le piace $L_2$"
>$P(E)=0,5$ e $P(F)=0,4$
>"le piacciono entrambi i libri" = $E\cap F$
>$P(E\cap F)=0,3$
>
>Quant'è la probabilità che non le piaccia nessun libro?
>
>$E\cup F$="le piace almeno uno dei libri"
>Per il principio di inclusione/esclusione $P(e\cup F)=P(E)+P(F)-P(E\cap F) \longrightarrow 0,5+0,4-0,3=0,6$
>L'evento complementare di *"le piace almeno un libro"* è *"non le piace alcun libro"*.
>Quindi quest'ultimo è $p((E \cup F)^c) = 1-0,6 = 0,4$

