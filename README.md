# Biblio

gestion bibliotheque

lancer : python biblio.py

Biblio est une application qui permet à une bibliothèque associative de gérer ses emprunts, ses membres, et ses livres.

## Prérequis
## Installation
## Utilisation
-Initialiser la base 
```bash 
python biblio.py init
```
>>> Base initialisee : 6 livres, 3 membres.

-Afficher les livres 
```bash 
python biblio.py livres
```
>>>[1] L'Etranger (Albert Camus) : disponible
[2] Dune (Frank Herbert) : emprunte
[3] Le Petit Prince (Antoine de Saint-Exupery) : disponible
[4] Fondation (Isaac Asimov) : disponible
[5] Les Miserables (Victor Hugo) : disponible
[6] Neuromancien (William Gibson) : disponible

-Rechercher un livre 
```bash
python biblio.py chercher Dune
```
>>>[2] Dune (Frank Herbert)

-Emprunter un livre 
```bash
python biblio.py emprunter 1 1
```
>>>Emprunt enregistre : livre 1, membre 1.

-Rendre un livre 
```bash
python biblio.py rendre 1
```
>>>Retour enregistre pour le livre 1.

-Afficher les retards 
```bash
python biblio.py retards
```
>>>Dune, emprunte par Alice Martin : 254 jours de retard
Fondation, emprunte par Bilal Haddad : 259 jours de retard
## Tests

Depuis le dossier du projet, lancer les tests :

```bash
python3 -m unittest
```

Résultat obtenu sous Ubuntu :

```text
Ran 4 tests in 0.087s

OK
```

Le temps d’exécution peut varier. `OK` indique que tous les tests passent.
Les messages comme « Erreur : livre 42 introuvable. » sont attendus :
certains tests vérifient le refus d’une opération invalide.

Selon votre installation, utilisez `python -m unittest` ou,
sous Windows, `py -m unittest`.

## Structure du projet

| Fichier ou dossier | Rôle |
|---|---|
| `biblio.py` | Programme de gestion des livres et des prêts. |
| `biblio.db` | Base SQLite créée par la commande `init`. |
| `tests/test_biblio.py` | Tests automatisés du programme. |
| `docs/circulation.md` | Organisation et règles de l’équipe. |
| `docs/adr/` | Décisions techniques et modèle d’ADR. |
| `exercices/` | Consignes des exercices. |
| `.github/ISSUE_TEMPLATE/` | Modèles pour signaler un bug, proposer une évolution ou poser une question. |
| `.github/pull_request_template.md` | Modèle de description des pull requests. |
| `.github/workflows/tests.yml` | Exécution des tests sur GitHub. |
| `README.md` | Présentation et instructions du projet. |

## Contribuer

1. Ouvrir une issue avec le modèle adapté : bug, évolution ou question.
2. Mettre à jour la branche `main`, puis créer une branche dédiée.
3. Effectuer la modification et vérifier son fonctionnement.
4. Pour une modification du code, lancer les tests avant de proposer la PR.
5. Faire un commit avec un message clair et pousser la branche.
6. Ouvrir une pull request décrivant les changements et la vérification.
   Ajouter `Closes #numero` si elle résout une issue.
7. Demander la relecture d’un autre membre et répondre à ses commentaires.
8. Après validation, fusionner la PR et supprimer la branche.

Aucun push direct sur `main` : les modifications passent par une PR relue.

Pour le README rédigé à trois, utiliser la branche commune du groupe.
Après son commit, faire Pull origin, puis Push origin.

## Auteurs

Contributeurs du groupe :

- Asma-Mouhli
- rubitombe
- avrilbrngnzz-boop
