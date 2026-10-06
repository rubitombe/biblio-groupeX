# Contribuer à Biblio

## Avant de coder
Avant de commencer à modifier le code, vérifier d'abord les issues existantes et créer une issue pour décrire le problème ou l'évolution souhaitée.
Utiliser le modèle "Signaler un bug" pour signaler un problème, "Proposer une évolution" pour demander une évolution et "Poser une question" lorsqu'une clarification est nécessaire.
Récupérer les dernières modifications de `main` avant de créer sa branche.

## Branches  
Ne jamais travailler directement sur `main`.
Créer une branche dédiée à chaque tâche en utilisant un nom explicite, avec ce modèle : `type/n°-mots-clés` , par exemple `fix/12-description`.
Pour les ADR, utiliser le format `docs/adr-numero` , conformément à l'ADR 0004.

## Commits
Faire des commits clairs et courts qui décrivent la situation réalisée.
Le message du commit doit permettre de comprendre rapidement ce qui a été modifié.
Utiliser le format `type: message`, par exemple `docs: ajouter les règles de contribution`

## Pull requests 
Toute modification doit passer par une Pull Request avant d'etre fusionnée dans `main`.
La Pull Request doit être liée à l'issue correspondante avec `Closes #n`.
Demander des corrections si les tests échouent ou si les critères de l'issue ne sont pas respectés.

## Review 
Chaque Pull Resquest doit etre relue et approuvée par au moins une personne du groupe avant d'être fusionnée.
L'auteur de la Pull Request ne peut pas approuver sa propre Pull Request.

## Definition of Done 
Une tache est considéerée comme terminée lorsque:

-Les tests passent (CI verte).​

-Une review approuvée par un autre membre.​

-La PR a une description et Closes #n.​

-Le README ou un ADR est à jour si besoin.​

-Aucun secret dans le code.​
​
## Signaler un blocage le formulaire
En cas de problème qui empêche d'avancer, créer une issue avec le modèle « Signaler un blocage ».
Indiquer la tâche concernée, l'erreur exacte, les actions déjà réalisées, l'aide nécessaire et l'échéance.
