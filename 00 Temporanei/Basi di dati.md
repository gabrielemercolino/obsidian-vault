---
tags:
  - unfinished
  - temporaneo
links: 
cssclasses:
---
# Basi di dati
## Unione
Costruisce una relazione che contiene tutte le n-uple che appartengono almeno a ognuno dei due operandi

Simbolo $\cup$

Può essere applicata solo ad operandi compatibili, ovvero se hanno lo *stesso numero* di attributi e quelli corrispondenti devono essere definiti sullo *stesso dominio*

> [!example] Esempio 1
> ![[Pasted image 20241002153657.png]]
> Facendo $\text{Personale}=\text{Docenti} \cup \text{Amministrativi}$
> ![[Pasted image 20241002153924.png]]
> 
> Tuttavia così ci si espone a possibili *tagli*
> Una progettazione migliore dovrebbe poter prevedere questo e distinguere in modo migliore i due tipi

>[!example] Esempio 2
>Poniamo invece questo
>![[Pasted image 20241002154318.png]]
>Qui abbiamo l'attributo **Stip** di troppo
>Dobbiamo prima effettuare una [[proiezione]], quindi $$\text{Personale}=\pi_{\text{Nome,CodDoc,Dipartimento}}(\text{Docenti}) \cup \pi_{\text{Nome,CodAmm,Dipartimento}}(\text{Amministrativi})$$

---
## Differenza
Come l'[[#Unione|unione]] si applica su operandi compatibii
Simbolo $-$
Ovviamante **non è commutativa**
![[Pasted image 20241002155752.png]]
>[!example] Esempio
>![[Pasted image 20241002155832.png]]
>![[Pasted image 20241002160025.png]]

---
## Intersezione
Come prima è applicabile con operandi compatibili
Simbolo $\cap$

>[!example] Esempio
>![[Pasted image 20241002160900.png]]
> $\text{Studenti}\cap\text{Amministrativi}$
>![[Pasted image 20241002160910.png]]

