---
tags:
  - unfinished
  - basi-dati
links: 
cssclasses:
---
# Proiezione
La proiezione consiste nella **selezione** di solo **alcuni attributi** 
Si denota con il simbolo $\pi$

> [!example] Esempio
> **Cliente**
> 
| Nome    | C#  | Città  |
| ------- | --- | ------ |
| Rossi   | C1  | Roma   |
| Rossi   | C2  | Milano |
| Bianchi | C3  | Roma   |
| Verdi   | C4  | Roma   |
> **Query** = *"Nomi dei clienti"* = $\pi_{Nome}(Cliente)$
> 
|              | 
| ------- |
| Rossi   | 
| Bianchi | 
| Verdi   | 
> > [!note] Nota
> > Selezionando solo il *Nome*, Rossi appare solo una volta perchè un'istanza di relazione non può avere *duplicati*
> > Per questo motivo bisogna selezionare anche la [[chiave]] in modo da essere sicuri che non ci si perda qualcosa in questi case
> > $\pi_{Nome,C#}(Cliente)$
> >    |     |





