---
tags:
  - unfinished
  - temporaneo
links: 
cssclasses:
---
# Sistemi operativi
![[Pasted image 20241001151703.png]]
**service call** (*system call*) è in realtà esso stesso un interrupt

Il sistema viene visto come una serie di livelli e ogni livello effettua un sottoinsieme delle funzioni del sistema
![[Pasted image 20241001151848.png]]
![[Pasted image 20241001152051.png]]
![[Pasted image 20241001152214.png]]
Ogni livello va ad utilizzare le primitive del livello precedente

Per UNIX (in realtà un pò per tutti):
![[Pasted image 20241001152356.png]]
Una vista del kernel UNIX:
![[Pasted image 20241001152526.png]]
![[Pasted image 20241001152709.png]]
![[Pasted image 20241001152826.png]]

---

## Processi
Il compito fondamentale del sistema è la gestione dei processi
- permettere l'esecuzione alternata
- assegnare le risorse ai processi e proteggere dagli altri processi
- permettere lo scambio di informazioni

#### Cos'è un processo
![[Pasted image 20241001153324.png]]
![[Pasted image 20241001153705.png]]
Quando un utente richiede l'esecuzione di un processo può crearsi più di un processo a seconda dell'applicazione
![[Pasted image 20241001153944.png]]
![[Pasted image 20241001154425.png]]
Queste informazioni vengono mantenute nel **process control block** che è unico per processo
![[Pasted image 20241001154954.png]]

---
## Traccia di un processo
![[Pasted image 20241001155146.png]]

---
## Esecuzione di un processo
![[Pasted image 20241001155430.png]]
![[Pasted image 20241001155522.png]]
Dal punto di vista dei singoli processi non ci sono interruzioni di esecuzione
![[Pasted image 20241001155651.png]]
Ovviamente dal punto di vista del SO è più complesso. Tramite il **dispatcher** si passa tra un processo all'altro

---
## Stati di un processo
![[Pasted image 20241001160214.png]]
![[Pasted image 20241001160356.png]]
Tramite una (in realtà più generalmente) il **dispatcher** prende il processo da eseguire
### Creazione
![[Pasted image 20241001160602.png]]

### Terminazione
![[Pasted image 20241001160900.png]]

---
## Modello dei processi a 5 stati
![[Pasted image 20241001160950.png]]
Abbiamo quindi ora 2 code:
![[Pasted image 20241001161601.png]]
Ancora meglio, separando la causa del blocco:
![[Pasted image 20241001161741.png]]

---
## Processi sospesi
![[Pasted image 20241001161829.png]]
![[Pasted image 20241001162049.png]]
Un pò meglio:
![[Pasted image 20241001162342.png]]