---
tags:
  - basi-dati
  - finished
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
> **Query** = *"Nomi dei clienti"* = $\pi_{\text{Nome}}(\text{Cliente})$
> 
|              | 
| ------- |
| Rossi   | 
| Bianchi | 
| Verdi   | 
> > [!note] Nota
> > Selezionando solo il *Nome*, Rossi appare solo una volta perchè un'istanza di relazione non può avere *duplicati*
> > Per questo motivo bisogna selezionare anche la [[chiave]] in modo da essere sicuri che non ci si perda qualcosa in questi casi
> > $\pi_{\text{Nome, C\#}}(\text{Cliente})$
> >   
|     |
> >    --- | --- |
> >    Rossi | C1 |
> >    Rossi | C2 |
> >    Bianchi | C3 |
> >    Verdi | C4 |



