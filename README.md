# Biblio

gestion bibliotheque

lancer : python biblio.py

Biblio est une application qui permet à une bibliothèque associative de gérer les emprunts, les membres, et les livres
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
## Structure du projet
## Contribuer
## Auteurs
