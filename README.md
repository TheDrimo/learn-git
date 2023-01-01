# learn-git
les notes de la formation git et github : de débutant à confirmé

## Introduction

+ bienvenue dans cette formation
+ versionner son code
+ pourquoi git et github
+ quiz1 : un petit quiz

## Installation de Git

+ sur Windows
+ sur Linux
+ sur osX
taper dans le terminal :
```
$ git version #si pas installé une pop up apparait pour installer git
```
ou alors télécharger le binaire d'installation depuis le site officiel
+ utiliser un terminal
toujours préferer utiliser git depuis le terminal et donc utiliser des commandes comme ls, cd, mkdir, pwd ... pour naviguer dans les dossiers depuis le terminal.
+ configurer git
```
$ git config --global user.name "mon_nom_d'utilisateur"
$ git config --global user.email mon_adresse_email@gmail.com
$ git config --global --list #pour vérifier qu'on a bien enregistré son compte

$ git #pour avoir l'aide/manuel de git
```

## Mon premier commit

+ Comprendre processus d'enregistrement
L'enregistrement des modifications se fait en plusieurs phases. Déjà on enregistre les modif dans la zone d'index (qui est une zone tampon) et ensuite on "commit" ces modifs dans le dépot local de git.
+ Initialiser un dépôt git
```
$ git init #initialise le dépôt (créé un dossier caché ".git")
$ ls -la #pour afficher les dossiers cachés, noteamment le ".git"
```
+ Mettre en place son projet
```
$ git status #pour savoir quels sont les dossiers dans le répertoire et s'ils sont ajoutés dans le dépôt
```
