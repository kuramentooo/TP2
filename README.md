#  Pipeline de CI/CD

## Objectif

Ce TP a pour but d'automatiser la mise à jour d'une Web App Azure.

## Mise en place

### Requirement

Créer web app sur azure.\
Connecter le web app au repository git.

### Etape 1

git clone https://github.com/kuramentooo/TP2.git

#### Modifier app.py

nano app.py\
modifier par exemple la version.

### Etape 2

Push le nouveau app.py sur github

### Etape 3

Dans les actions un workflow doit être en cours vérifier que tous fonctionnent correctement

### Etape 4

Acceder a la page web avec le lien donner quand l'action est terminer

## Explication de la pipeline de CI/CD

Lors de la création du web app Azure on la connecte au repository Git.\
Azure push alors un workflow dans le repository, que l'on va utiliser ensuite.\
Dans ce workflow il est dit qu'a chaque fois que l'on fait un "push" dans le repository il se lance.\
Des lors que l'on modifie le fichier app.py et que l'on push, l'Azure web app se met à jour avec la modification prise en compte.

## Deroulement du workflow

Dans un premier temps on vient build app.py qui est une app flask, qui nous retourne une page web.\
Ensuite on vient tester notre app.py avec test app py, pour vérifier que tous fonctionnent.\
Pour finir si tout est correctement seter on build le web app.
