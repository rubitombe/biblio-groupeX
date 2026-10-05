# Biblio

Biblio est une application qui permet à une bibliothèque associative de gérer ses emprunts, ses membres, et ses livres.

## Prérequis

- GitHub Desktop pour cloner le depot
- Un terminal
- Python 3 installé

Sous macos ou linux utiliser `python3` à la place de `python`
Sous windows utiliser `py` si `python` ne fonctionne pas

## Installation
On commence par cloner le dépôt dans Github desktop:
    - Aller dans File > Clone repository 
    - Selectioneer l'onglet URL
    -Entrer l'URL du dépôt

Ouvrir le terminal du projet:
    -Aller dans Repository > Open in Command Prompt

Base de démonstration: 
```text
python biblio.py init .
```
Le résultat obtenu doit etre:
Base initialisee : 6 livres, 3 membres.

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
## Structure du projet
## Contribuer
## Auteurs
