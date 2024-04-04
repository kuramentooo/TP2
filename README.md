#  pipeline de CI/CD

## Objectif



## Mise en place

### Requirement

Creer web app sur azure.\
Connecter la web app au repository git.

### Etape 1

git clone https://github.com/kuramentooo/TP2.git

#### Modifier app.py

nano app.py\
modifier par exemple la version.

### Etape 2

push le nouveau app.py sur github

### Etape 3

dans les actions un workflow doit etre en cours verifier que tous fonctionne correctement

### Etape 4

Acceder a la page web avec le lien donner quand l'action est terminer

## Explication de la pipeline de CI/CD

Lors de la creation de la web app Azure on la conncete au repository Git.\
Azure push alors un workflow dans le repository, que l'on va utiliser ensuite.\
Dans ce workflow il est dit qu'a chaque fois que l'on fait un "push" dans le repository il ce lance.\
Dans quand on moifie le fichier app.py et que l'on push sa nouvelle version l'Azure web app ce met a jour avec le modification prise en compte.\

## Deroulement du workflow

Dans un premier temps on vient build app.py qui est une app flask, qui nous retourne une page web.\
Ensuite on vient tester notre app.py avec test_app.py, pour verifier que tous fonctionne.\
pour finir si tous est correctment seter on build la web app.\

