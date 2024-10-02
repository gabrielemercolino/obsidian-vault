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

> [!example] Esempio
> ![[Pasted image 20241002153657.png]]
> Facendo $\text{Personale}=\text{Docenti} \cup \text{Amministrativi}$
> ![[Pasted image 20241002153924.png]]
> 
> Tuttavia così ci si espone a possibili *tagli*
> Una progettazione migliore dovrebbe poter prevedere questo e distinguere in modo migliore i due tipi

>[!example] Esempio
>Poniamo invece questo
>![[Pasted image 20241002154318.png]]
>Qui abbiamo l'attributo **Stip** di troppo
>Dobbiamo prima effettuare una [[proiezione]], quindi $$\phy_$$