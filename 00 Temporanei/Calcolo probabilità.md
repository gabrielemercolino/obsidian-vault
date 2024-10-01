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
>Per il principio di inclusione/esclusione
>$P(e\cup F)=P(E)+P(F)-P(E\cap F) \longrightarrow 0,5+0,4-0,3=0,6$
>L'evento complementare di *"le piace almeno un libro"* è *"non le piace alcun libro"*.
>Quindi quest'ultimo è $P((E \cup F)^c) = 1-0,6 = 0,4$

---
$S$ spazio campionario
$E, F \subset S$
![[Pasted image 20241001172921.png]]
$x \in E\cup F <-> x \in E \lor x \in F$
Quindi l'evento $E\cup F$ significa *si verifica E o si verifica F* (non esclusivamente)
>[!example] Esempio
>Ho un dado truccato per cui 1 esce con probabilità $\frac{1}{2}$ e gli altri con probabilità $\frac{1}{10}$
>
>Qual è la probabilità che esca un numero dispari?
>$P(E) dove E = \{1,3,5\}$
>Per additività finita $P(E)=0,5+0,1+0,1=0,7$

---
## Spazi di probabilità con esiti equipossibili
Supponiamo che $|S|< \infty$
Scrivo $S=\{S_1,S_2,...,S_n\}$ e ho $n$ esiti
