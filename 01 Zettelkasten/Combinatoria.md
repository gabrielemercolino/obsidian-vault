La combinatoria è una branca della matematica che si occupa di studiare gli esiti degli eventi. 

Ad esempio supponiamo di voler calcolare quante possibilità uniche possono capitare lanciando un dado. Siccome ha 6 facce, ad ogni lancio può capitare con la stessa probabilità una di queste 6 facce. Siccome ci sono 2 lanci il numero delle combinazioni è $6*6=36$

---
#### **Dimostrazione**: 
- scelgo il primo: $n$ modi possibili
- scelgo il secondo: $n-1$ modi possibili
- ...
- scelgo l'ultimo: $n-n+1 = 1$ modo possibile
Allora, per il [[#**Principio fondamentale della combinatoria - esteso**|principio]], $\#permutazioni=n*(n-1)*(n-2)*$ ... $*1 = n!$

---
## **Scelta senza ripetizioni**
```ad-danger
title:
In un insieme di $n$ elementi distinti posso scegliere $k$ oggetti distinti dove non conta l'ordine con questi passi:
1) conto come se l'ordine ci fosse (distinguo le ripetizioni)
2) elimino le ripetizioni

$$\frac{n*(n-1)*(n-2)*...*(n-k+1)}{k!}=\left( \begin{array}{c} n \\ k \end{array} \right)$$
```
Questo è il [[coefficiente binomiale]]

---
## **Partizioni**
```ad-danger
title:
Per $n$ oggetti da ripartire in $r$ modi distinti in modo tale che, con $\forall i$ $1 \leq i \leq r$,  per ogni partizione ci siano $n_i$ oggettin tale che $n_1+n_2+...+n_r=n$:
$$\#partizioni=\frac{n!}{n_1!*n_2!*...*n_r!}=:\left( \begin{array}{c} n \\ n_1 n_2...n_r\end{array} \right)$$
```
Questo è il [[coefficiente multinomiale]]