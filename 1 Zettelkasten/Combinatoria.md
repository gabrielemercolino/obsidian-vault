La combinatoria è una branca della matematica che si occupa di studiare gli esiti degli eventi. 

Ad esempio supponiamo di voler calcolare quante possibilità uniche possono capitare lanciando un dado. Siccome ha 6 facce, ad ogni lancio può capitare con la stessa probabilità una di queste 6 facce. Siccome ci sono 2 lanci il numero delle combinazioni è $6*6=36$

---
## **Principio fondamentale della combinatoria - base**
Supponiamo di avere 2 esperimenti. Il primo ha $n_1$ esiti possibili e qualunque esso sia il secondo ha sempre $n_2$ esiti possibili.
Allora il numero delle coppie $(a_1,a_2)$ possibili è $n_1*n_2$ 

Tuttavia questo può essere ulteriormente generalizzato per più di soli due esperimenti, quindi
## **Principio fondamentale della combinatoria - esteso**
Supponiamo di avere $r$ esperimenti. Il primo ha $n_1$ esiti possibili. Qualunque esso sia il secondo ne ha $n_2$, il terzo $n_3$ ecc.
Allora il numero delle possibili stringhe $(a_1, a_2, ... , a_r)$, dove $a_i$ è l'esito dell'$i$-esimo esperimento, è $n_1*n_2*...*n_r$ 

---

A seconda del caso, può non essere possibile a prima vista applicabile il principio. Tuttavia si tratta di riuscire a dividere il problema correttamente per riuscire a risolverlo.

Supponiamo di avere questi dati:
- $120$ ragazzi
- $20$ ragazze
Ora si vuole trovare il modo in cui poter **scegliere 2 persone** di **sesso diverso**.
La prima persona può essere scelta su $120+20=140$ persone siccome il vincolo non c'è, tuttavia per la seconda scelta bisogna sapere il risultato della prima. Questo **sembrerebbe non rispettare** il [[#**Principio fondamentale della combinatoria - esteso**|principio]], tuttavia possiamo tranquillamente dire che il numero delle combinazioni possibili è dato dalla somma delle due casistiche di scelta del genere, ovvero considerando il caso in cui venga scelto prima maschio-femmina e poi femmina-maschio e infine sommare. Questo significherebbe calcolare $120*20 + 20*120 = 2400 * 2 = 4800$

---

## **Permutazioni**
Dati $n$ oggetti **distinti**, le permutazioni sono tutti i possibili allineamenti, ovvero $n!$

#### **Dimostrazione**: 
- scelgo il primo: $n$ modi possibili
- scelgo il secondo: $n-1$ modi possibili
- ...
- scelgo l'ultimo: $n-n+1 = 1$ modo possibile
Allora, per il [[#**Principio fondamentale della combinatoria - esteso**|principio]], $\#permutazioni=n*(n-1)*(n-2)*$ ... $*1 = n!$

---
## **Permutazioni senza ripetizioni**
Fin'ora sono sempre stati assunti elementi sempre diversi, infatti fin'ora se appaiono ripetizioni tutto il castello crolla perchè contiamo delle ripetizioni. Tuttavia per risolvere il problema è di fatto sufficiente applicare le cose precedentemente utilizzate e poi rimuovere le ripetizioni. 

In generale, per $n$ oggetti da ripartire in $r$ modi distinti in modo tale che, con $\forall i , 1 \leq i \leq r$,  per ogni partizione ci siano $n_i$ oggettin tale che $n_1+n_2+...+n_r=n$: 
$$\#partizioni=\frac{n!}{n_1!*n_2!*...*n_r!}=:\left( \begin{array}{c} n \\ n_1 n_2...n_r\end{array} \right)$$
Questo di chiama [[coefficiente multinomiale]]
