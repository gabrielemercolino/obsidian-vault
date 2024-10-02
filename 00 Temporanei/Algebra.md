---
tags:
  - unfinished
  - algebra
  - temporaneo
links: 
cssclasses:
---
# Algebra
> [!error] Def
> Unfa funzione $f:X\longrightarrow Y$ è **biiettiva** se è allo stesso tempo [[suriettiva]] e  [[iniettiva]]

> [!example] Dimostrazione
> $f$ iniettiva <-> $\forall y \in Y, f^{-1}(\{y\}) = \emptyset$ oppure è un [[singleton]]
> $f$ [[suriettiva]] <-> $\forall y \in Y, f^{-1}(\{y\}) \neq \emptyset$
> *Quindi* $f$ biiettiva <-> $\forall y \in Y, f^{-1}({y})$ è un [[singleton]]

> [!example] Esempio
> $X$ insieme $\neq \emptyset$, $Id:=(X,X,\delta_{x})$ 
> $\delta_{x}=\{(x,x):x\in X\} \forall x Id_x(x)=x$
> Questo si chiama **sottoinsieme diagonale**  

### Notazione
![[Pasted image 20241001140352.png]]

---
### Diagrammi
>[!error] Def
>Un diagramma è una collezione di insiemi *non vuoti* collegati da [[funzioni|applicazioni]]

> [!example] Esempi
> ![[Pasted image 20241001140738.png]]
> ![[Pasted image 20241001140752.png]]
> ![[Pasted image 20241001140801.png]]
> ![[Pasted image 20241001140811.png]]
> ![[Pasted image 20241001140846.png]]

---
### Operazioni sulle funzioni
#### Composizione
>[!error] Def
![[Pasted image 20241001140846.png]]
Si definisce **funzione composta** come la 
![[Pasted image 20241001140943.png]]
funzione definita da $(g \circ f)(x)=g(f(x))$

> [!info] Proprietà
> **associatività**: $(h \circ g) \circ f = h \circ (g \circ f)$

---

> [!warn] Proposizione
> $f$ biiettiva <-> $\exists g:Y \longrightarrow X: f \circ g = id_Y, g \circ f = id_X$
> g è chiamata **funzione inversa**

> [!info] Dimostrazione
> ![[Pasted image 20241001141839.png]]

Supponiamo adesso che sia dato il diagramma ![[Pasted image 20241001142358.png]]
con 
1) $f\circ g = id_Y$ 
2) $g \circ f = id_X$
Mostriamo che $g$ è **suriettiva**. Sia $x \in X$ e poniamo $y = f(x)$. Allora $g(y)=g(f(x))=(g\circ f)(x) = x$ per via di **2** $\longrightarrow g^{-1}(x)\neq \emptyset$ 
Mostriamo che $g$ è **iniettiva**. Siano $y, y^i \in Y$ tali che $g(y)=g(y^i)=x$. Allora applicando $f$ a tutti ottengo $f(g(y))=f(g(y^i))=f(x) \longrightarrow y=(f\circ g)(y)=(f\circ g)(y^i)$  

---
Se $f:X\rightarrow Y$ è biiettiva si denota la sua **inversa** con $f^{-1}:Y\rightarrow X$
Notare che $f^{-1}$ è ugualmente *biettiva*

---
Se $f$ e $g$ sono biiettive
![[Pasted image 20241001143537.png]]
$(g \circ f)^{-1} = f^{-1}\circ g^{-1}$

---
### Teorema di strutture per le applicazioni
![[Pasted image 20241001143919.png]]
Si pone $x, x^i\in X, x \tilde x^i <-> f(x) = f(x^i)$ dove $\tilde$ è una relazione di equivalenza
- **riflessiva**: $x \tilde x^i : f(x) = f(x^i)$
- **simmetrica**: $x \tilde x^i <-> f(x) = f(x^i) <-> f(x^i)=f(x) <-> x^i=x$
- **transitiva**: $x \tilde x^i, x^i\tilde x^{ii} <-> f(x) = f(x^i), f(x^i)=f(x^{ii}) -> f(x)=f(x^{ii}) <-> x \tilde x^{ii}$

Consideriamo l'insieme quoziente $\frac{X}{\tilde}$
![[Pasted image 20241001144613.png]]
![[Pasted image 20241001144700.png]]
![[Pasted image 20241001144735.png]]
![[Pasted image 20241001145352.png]]
>[!error] Def
>L'applicazione $\phi$ è ben definita *(l'immagine di una classe dipende dalla scelta di un rappresentante)* è biiettiva e permette di calcolare $f$ fattorizzandola con il diagramma seguente 
>![[Pasted image 20241001150023.png]]

---
![[Pasted image 20241002171807.png]]
