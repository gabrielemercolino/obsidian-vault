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
Immaginiamo che i vari esiti abbiano la stessa speranza di realizzarsi
Come materializziamo questo esperimento con uno spazio di probabilità?

Siccome gli esiti sono equipossibili, richiediamo che $P(\{S_1\})=P(\{S_2\})=...=P(\{S_n\})$
D'altro canto ho che $1=P(S)$ e $S=\{S_1,S_2,...,S_n\}$ e gli eventi sono *a 2 a 2 incompatibili* allora $\sum_{i=1}^{n}{P(\{S_i\})}=n*z$
Provato che $1=n*z$, cioè $z=\frac{1}{n}$, ovvero $P(\{S_i\}) \forall i = 1...n$

> [!danger] Proposizione
> Se $|S|=n$ e gli esiti sono equipossibili, allora $\forall E$ eventi
> $$P(E) = \frac{|E|}{|S|} = \frac{\text{esiti favorevoli a E}}{\text{esiti equipossibili}}$$

> [!example] Esempio
> Ho un'urna con 6 palline bianche e 5 nere
> Estraggo 3 palline a caso (senza rimpiazzo)
> Qual è la probabilità che tra le estratte 2 siano nere e una bianca?
> 
> Non conviene registrare solo il colore delle palline estratte siccome non c'è una simmetria
> Conviene pensare che le palline siano distringuibili (per esempio numerandole)
> $U=\{B_1,B_2,B_3,B_4,B_5,B_6,N_1,N_2,N_3,N_4,N_5\}$
> Quindi ora ho 11 palline distinguibili
> $S=\{A \subset U : |A|=3\}$
> Un esempio di esito è $\{B_2,B_4,N_3\}$
> $S$ ha esiti equiprobabili per simmetria
> Quindi $P(E)=\frac{|E|}{|S|}$
> Ora $|S|=\left( \begin{array}{c} 11 \\ 3\end{array}\right)$
> Per il [[Principio fondamentale della combinatoria|PFdC]] $$|E|=\text{modi pallina bianca} * \text{modi scegliere 2 palline nere no ordine} = 6 * \left( \begin{array}{c} 5 \\ 2\end{array}\right)$$
> Quindi $$\frac{|E|}{|S|}=\frac{6 * \left( \begin{array}{c} 5 \\ 2\end{array}\right)}{\left( \begin{array}{c} 11 \\ 3\end{array}\right)} = \frac{12}{33}$$

---
## Problema dei compleanni
Consideriamo due persone, A e B
Qual è la probabilità che abbiano lo stesso compleanno?

Per semplicità tutti gli anni hanno 365 giorni e che ci sia una simmetria tra i vari giorni dell'anno per quanto riguarda il numero delle persone nate in un dato giorno
$S\{(x_1,x_2):x_1,x_2\in \{1,2,...,365\}\}$ dove $x_1=\text{compleanno di A}$ e $x_2=\text{compleanno di B}$
$S$ ha quindi esiti equiprobabili
Allora $P(E)=\frac{|E|}{|S|}$ dove $|E|=365$ mentre $|S|=365^2$, quindi $$P(E)=\frac{365}{365^2}=\frac{1}{365}$$

Ora stesso problema ma con 3 persone, A, B e C
$S\{(x_1,x_2,x_3):x_1,x_2,x_3\in \{1,2,...,365\}\}$ e ha esiti equiprobabili
$E=\{(x_1,x_2,x_3)\in S : \exists i \neq j \text 1 \leq i,j \leq 3 \land x_i = x_j\}$
$P(E)=\frac{|E|}{|S|}$ dove però $|E|$ è complicato da calcolare
Tuttavia $P(E)=1-P(E^c)$
$E^c=\{(x_1,x_2,x_3) \in S : x_1,x_2,x_3 \text{sono distinti}\}$, quindi $|E|=365*364*363$
Infine possiamo dire che $$P(E)=1-P(e^c)=1-\frac{365*364*363}{365^3}$$
Con *n* persone per calcolare $P(E)$ procedo come sopra
$|S|=365^n$ per il [[Principio fondamentale della combinatoria|PFdC]], mentre $E^c=\{(x_1,...,x_n)\in S: x_1,...,x_n \text{diversi}\}$ e quindi $|E|=365*364*(365-n+1)$
Concludendo $$P(E)=1-P(E^c)=1-\frac{365*364*...*(365-n+1)}{365^n}$$
>[!example] Esempio
>Devo creare una commissione da 5 persone da un gruppo  di 6 uomini e 9 donne formato da 3 uomini e 2 donne
>$S=\{A\subset G : |A|=5\}$ dove $G=\text{gruppo di 15 persone}$
>Gli esiti sono equiprobabili per simmetria
>$|S|=\left( \begin{array}{c} 15 \\ 5\end{array} \right)$
>$E=\{A\subset G : |A|=5\} \land A \text{contiene 3 uomini e 2 donne}$
>$|E|=\left( \begin{array}{c} 6 \\ 3\end{array} \right)*\left( \begin{array}{c} 9 \\ 2\end{array} \right)$
>Allora $$P(E)=\frac{140}{1001}$$

