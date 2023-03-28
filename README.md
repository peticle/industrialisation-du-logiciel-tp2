# 3293.1 Industrialisation du logiciel - TP2

## Exercice 1 - GitHub Actions

### Les étapes réalisées par l'action

Le fichier de base réalise un job de _build_.
Dans ce job, on a divers étapes :

- Configuration de Python 3.10
- Installation des dépendances, `flake8`, `pytest` et requirements.txt si existant
- Linting du code avec `flake3`
- Lancer les tests du projet avec `pytest`

### Les 2 paramètres d'une étape

Chaque étape possède au minimum 2 paramètres qui sont :

- Un nom pour l'étape
- Une suite de commandes à exécuter

### Paramètre `with` de la première étape

Cette étape sert à configurer python sur le runner en utilisant l'action
`actions/setup-python@v3`, le paramètre `with` permet de spécifier quelle version de Python on veut installer.
