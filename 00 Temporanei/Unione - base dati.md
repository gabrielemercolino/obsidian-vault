---
tags:
  - unfinished
  - basi-dati
links: 
cssclasses:
---
# Unione
Consente di costruire una relazione che **contiene** tutte le **n-uple** appartenenti ad almeno uno dei due operandi
Si denota con il simbolo $\cup$
> [!warning] Attenzione
> I due operandi **devono** essere **union compatibili**, ovvero:
> - avere lo *stesso numero* di attributi
> - avere gli attributi *corrispondenti* nello stesso ordine e definiti nello *stesso dominio*
>
> Tuttavia **non** è necessario che abbiano lo **stesso nome**

> [!example] Esempio
> **Docenti**
> 
> Nome | CodDoc | Dipartimento |
> ------ | --------- | ------------- |
> Rossi  |       C1      | Matematica  |
> Rossi  |       C2      | Lettere  |
> Bianchi  |       C3      | Matematica  |
> Verdi  |       C4     | Lingue  |
> 
> **Amministrativi**
> 
> Nome | CodAmm | Dipartimento |
> ------ | --------- | ------------- |
> Esposito  |       C1      | Lingue  |
> Riccio  |       C2      | Matematica  |
> Pierro  |       C3      | Lettere  |
> Bianchi  |       C4     | Lingue  |
> 
> **Personale** = $\text{Docenti} \cup \text{Amministrativi}$
> 
> Nome | Cod | Dipartimento |
> ------ | --------- | ------------- |
> Esposito  |       C1      | Lingue  |
> Riccio  |       C2      | Matematica  |
> Pierro  |       C3      | Lettere  |
> Bianchi  |       C4     | Lingue  |
> Rossi  |       C1      | Matematica  |
> Rossi  |       C2      | Lettere  |
> Bianchi  |       C3      | Matematica  |
> Verdi  |       C4     | Lingue  |

