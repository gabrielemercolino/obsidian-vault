---
tags:
  - algebra
  - finished
links: "[[Funzioni]]"
cssclasses: 
aliases:
  - applicazione inversa
  - inversa
---
# Funzione inversa
>[!error] Def
> Data $f$ [[Funzione biiettiva|biiettiva]] $\exists g:Y \longrightarrow X: f \circ g = id_Y, g \circ f = id_X$
> g è chiamata **funzione inversa**
## Dimostrazione
Con $f$ [[Funzione biiettiva|biiettiva]] $\forall y \in Y \exists ! x \in X : f(x)=y$
Poniamo $g(y)=x$ ben definita e osserviamo:
1) se $x\in X g(f(x))=g(y)$ e $x$ è l'unico elemento tale che $f(x)=y \longrightarrow g(y)=x \rightarrow g \circ f = id_x$
2) in modo simile si può verificare che $f \circ g = id_y$

Supponiamo adesso che sia dato il diagramma ![[Pasted image 20241001142358.png]]con 
1) $f\circ g = id_Y$ 
2) $g \circ f = id_X$
Mostriamo che $g$ è **suriettiva**. Sia $x \in X$ e poniamo $y = f(x)$. Allora $g(y)=g(f(x))=(g\circ f)(x) = x$ per via di **2** $\longrightarrow g^{-1}(x)\neq \emptyset$ 
Mostriamo che $g$ è **iniettiva**. Siano $y, y^i \in Y$ tali che $g(y)=g(y^i)=x$. Allora applicando $f$ a tutti ottengo $f(g(y))=f(g(y^i))=f(x) \longrightarrow y=(f\circ g)(y)=(f\circ g)(y^i)$

---
Se $f:X\rightarrow Y$ è biiettiva si denota la sua **inversa** con $f^{-1}:Y\rightarrow X$
Notare che $f^{-1}$ è ugualmente [[Funzione biiettiva|biiettiva]]

Se $f$ e $g$ sono biiettive
![[Pasted image 20241001143537.png]]
$(g \circ f)^{-1} = f^{-1}\circ g^{-1}$
