# learn-git
les notes de la formation git et github : de débutant à confirmé

## Introduction

#### bienvenue dans cette formation
#### versionner son code
#### pourquoi git et github
#### quiz1 : un petit quiz

## Installation de Git

#### sur Windows
#### sur Linux
#### sur osX
taper dans le terminal :
```
$ git version #si pas installé une pop up apparait pour installer git
```
ou alors télécharger le binaire d'installation depuis le site officiel
#### utiliser un terminal
toujours préferer utiliser git depuis le terminal et donc utiliser des commandes comme ls, cd, mkdir, pwd ... pour naviguer dans les dossiers depuis le terminal.
#### configurer git
```
$ git config --global user.name "mon_nom_d'utilisateur"
$ git config --global user.email mon_adresse_email@gmail.com
$ git config --global --list #pour vérifier qu'on a bien enregistré son compte

$ git #pour avoir l'aide/manuel de git
```

## Mon premier commit

#### Comprendre processus d'enregistrement
L'enregistrement des modifications se fait en plusieurs phases. Déjà on enregistre les modif dans la zone d'index (qui est une zone tampon) et ensuite on "commit" ces modifs dans le dépot local de git.
#### Initialiser un dépôt git
```
$ git init #initialise le dépôt (créé un dossier caché ".git")
$ ls -la #pour afficher les dossiers cachés, noteamment le ".git"
```
#### Mettre en place son projet
```
$ git status #pour savoir quels sont les dossiers dans le répertoire et s'ils sont ajoutés dans le dépôt
```
#### Indexer ses modifications
```
$ git add fichier1 fichier2 #pour déposer les fichiers nommés dans la zone d'index
$ git add . #pour déposer tous les fichiers de la zone de travail
$ git reset fichier1 #pour retirer le fichier1 de la zone d'index
```
#### Faire son premier commit
```
$ git commit -m "message de commit" #pour enregistrer dans git les fichiers de la zone d'index
```
#### Afficher les modifications en cours
```
$ git diff fichier1 #pour voir les modifs apportées au fichier1
$ git diff #pour voir toutes les modifs
$ git diff --cached #pour voir les modifs des fichiers indexés (qui sont déjà dans la zone d'index)
```
#### Quiz3 : Les commits
#### Exercice et bilan de la section

## Voyager dans l'historique

#### Comprendre l'archivage des commits
chaque commits s'inscrit dans une branche, la branch principale est la branch master.
chaque commits va être décrit par :
- un identifiant unique de 40 caractères (le SHA-1)
- un ensemble de modificaiton
- un commentaire décrivant le commit
- les informations sur l'auteur (nom et mail)
- une date
- liste de SHA-1 de son (ou ses) parents

#### Voir l'historique des commits
Pour afficher les commits :
```
$ git log
$ git show
```

#### Naviguer dans l'historique des commits
```
$ git log #pour afficher les commit
$ git checkout Sha1duCommit #pour déplacer le curseur sur ce commit là
$ git log #affichera seulement les commits précédent au commit sur lequel on est
$ git checkout master #pour revenir sur le master
```

#### Utiliser des tags
Les tags permettent de naviguer plus facilement qu'avec les sha1 et de personnaliser les versions de developpement
```
$ git checkout sha1ducommit
$ git tag versionBeta #associe le tag "versionBeta" au commit sur lequel on est
$ git --delete versionBeta #supprime le tag
$ git tag #pour afficher les tags présents
```

#### Quiz4 : Voyager dans l'historique d'un dépôt Git
#### Exercice et bilan de la section

## Présentation de Github

#### Découvrir Github
#### Utiliser les gists
