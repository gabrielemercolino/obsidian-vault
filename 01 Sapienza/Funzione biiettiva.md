---
tags:
  - unfinished
  - algebra
links: 
cssclasses:
---
## Funzione biiettiva
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

> [!warn] Proposizione
> $f$ biiettiva <-> $\exists g:Y \longrightarrow X: f \circ g = id_Y, g \circ f = id_X$
> g è chiamata **funzione inversa**
> 