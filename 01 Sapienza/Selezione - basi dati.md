---
tags:
  - basi-dati
  - finished
links: 
cssclasses:
---
# Selezione
La selezione consente di prelevare solo le **tuple** che soddisfano la condizione specificata
Si denota con $\sigma$

> [!example] Esempio
>  Nome    | C#  | Città  |
| ------- | --- | ------ |
| Rossi   | C1  | Roma   |
| Rossi   | C2  | Milano |
| Bianchi | C3  | Roma   |
| Verdi   | C4  | Roma   |
> Query = *Clienti risiedenti a Roma* = $\sigma_{\text{Città} = \text{'Roma'}}(\text{Cliente})$
>   
>   |   |   |
| ------- | --- | ------ |
| Rossi   | C1  | Roma   |
| Bianchi | C3  | Roma   |
| Verdi   | C4  | Roma   |
> Query = *Clienti risiedenti a Roma e si chiamano Rossi* = $$\sigma_{\text{Città} = \text{'Roma'} \land \text{Nome}=\text{'Rossi'}}(\text{Cliente})$$
>
|   |   |
| ------- | --- | ------ |
| Rossi   | C1  | Roma   |




