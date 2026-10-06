# ADR 0002 : SQLite plutôt qu'un serveur de base de données

- Statut : proposé 
- Date : 2026-10-05
- Décideurs :  Asma-Mouhli, avrilbrngnzz-boop et rubitombe 

## Contexte

Biblio est une application destinée à une  bibliothèque associative. Elle doit permettre aux bénévoles de gérer simplement les livres, les membres et les emprunts.

La solution choisie doit être simple à installer et à utiliser, car les bénévoles ne disposent pas forcément de compétences techniques avancées et requises. Il faut donc éviter une installation et une maintenance trop complexes.

## Options envisagées
1. Option A SQLite:
 Avantages :
 -Pas besoin de serveur a installer ou a gerer
 -Instalation et sauvegarde simple
 -Compatible à une petite et simple application 

 Inconvénients:
 -Pas adapté pour un grand nombre d'utilistauers en simultanées
 -Pas adpaté si l'application venait à evoluer vers une architecture serveur

2. Option B PostegreSQL
Avantages:
-Adapté pour un grand nombre d'utilistauers en simultanées
-Systeme de base de données complet et puissant
Incovénients:
-Maintenace complexe
- Difficile d'utulisation sans compétences techniques

## Décision
Nous choisisions SQLite car elle permet à l'association d'utiliser une base de données sans installer ou admkinistrer de serveur.

## Conséquences
<!-- Ce que la décision rend plus facile, et ce qu'elle rend plus difficile. -->
- L'installation du projet est simple
- Aucun besoin de serveur 
- La base peut être facilement sauvegardée sous forme de fichier
- La solution est adaptée aux besoins d'une petite bibliothèque
- SQLite est moins adaptée à un grand nombre d'utilisateurs qui accéderaient simultanément à la base.
- Une évolution vers une application nécessitant un serveur pourrait demander une migration vers une autre solution de base de données.