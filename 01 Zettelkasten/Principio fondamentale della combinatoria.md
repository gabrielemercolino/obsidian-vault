---
tags:
  - unfinished
  - calcolo-probabilità
links: 
cssclasses:
---
## Principio fondamentale della combinatoria

> [!error] Def
> Supponiamo di avere $r$ esperimenti. Il primo ha $n_1$ esiti possibili. Qualunque esso sia il secondo ne ha $n_2$, il terzo $n_3$ ecc.
> Allora il numero delle possibili stringhe $(a_1, a_2, ... , a_r)$, dove $a_i$ è l'esito dell'$i$-esimo esperimento, è $n_1*n_2*...*n_r$ 

> [!example] Esempio
Supponiamo di avere $120$ ragazzi e $20$ ragazze.
Ora si vuole trovare il modo in cui poter **scegliere 2 persone** di **sesso diverso**.
La prima persona può essere scelta su $120+20=140$ persone siccome il vincolo non c'è, tuttavia per la seconda scelta bisogna sapere il risultato della prima. Questo **sembrerebbe non rispettare** il [[Principio fondamentale della combinatoria|principio]], tuttavia possiamo tranquillamente dire che il numero delle combinazioni possibili è dato dalla somma delle due casistiche di scelta del genere, ovvero considerando il caso in cui venga scelto prima maschio-femmina e poi femmina-maschio e infine sommare. Questo significherebbe calcolare $120*20 + 20*120 = 2400 * 2 = 4800$
