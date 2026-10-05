# ADR 0004 : convention de nommage des branches

- Statut : accepté
- Date : 2026-10-05
- Décideurs : Asma-Mouhli, rubitombe, avrilbrngnzz-boop

## Contexte
Plusieurs membres travaillent sur Biblio en parallèle.
Des noms de branches différents rendent difficile la compréhension
des modifications et le lien avec les issues.
Une convention commune permet de retrouver rapidement le sujet
et l’issue concernés.

## Options envisagées

1. Choisir librement le nom de chaque branche.
   - Avantage : rapide, sans règle à apprendre.
   - Inconvénient : noms incohérents et lien avec l’issue peu visible.

2. Utiliser le format type/numero-mots-cles pour les branches
   liées à une issue, et docs/adr-numero pour les ADR.
   - Avantage : le nom indique le type de travail et son sujet.
   - Inconvénient : chacun doit respecter le format et retrouver
     le numéro de l’issue avant de créer sa branche.

## Décision
Nous utilisons le format type/numero-mots-cles pour les branches liées à une issue et docs/adr-numero pour les ADR.
## Conséquences
- Les branches sont plus faciles à identifier dans GitHub Desktop.
- Le numéro permet de retrouver l’issue concernée.
- Exemples : fix/1-recherche-apostrophe, docs/10-readme
  et docs/adr-0004.
- Les contributeurs doivent apprendre et respecter la convention.
- Les noms sont plus longs et leur conformité doit être vérifiée
  pendant la relecture.