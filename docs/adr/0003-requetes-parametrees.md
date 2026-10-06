# ADR 0000 : Requête SQL paramètres obligatoires 

- Statut : accepté 
- Date : 2026-10-05
- Décideurs : avrilbrngnzz-boop

## Contexte

Dans une bibliothèque, l'application doit rechercher des livres et gérer les emprunts avec des requêtes SQL. Les textes saisis par les utilisateurs peuvent contenir des caractères particuliers, comme des apostrophes. Il faut donc choisir une méthode qui évite de modifier ou de construire directement les requêtes SQL avec les données saisies.

## Options envisagées
1. Requêtes SQL paramétrés
-Avantage : les données saisies sont séparés de la requête SQL
-Inconvénient : il faut utiliser cette méthode pour chaque requête qui reçoit des données
2. Nettoyer le texte saisi avant de construire la requête
-Avantage : cela permet de modifier les caractères problèmatiques avant de les utiliser
-Inconvénients : il faut prévoir correctement les caractères à traiter et cela peut laisser passer certains cas 

## Décision

Nous choisissons d'utiliser obligatoirement des requêtes SQL paramétrées pour les requêtes qui utilisent des données saisies par l'utilisateur.
## Conséquences

Les requêtes SQL sont plus sûres et les recherches avec des caractères particuliers,sont mieux gérées. Mais les requêtes doivent être écrites avec des paramètres et cette règle doit être respectée partout dans le projet.