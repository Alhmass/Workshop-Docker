# Exercice 1

L'objectif de cet exercice est de créer une image docker d'un serveur Minecraft spigot en version 1.14.2.

Pour se faire l'exercice est composé de deux étapes.

## Première étape

Spigot nous fournit un applicatif Build Tools.jar, qui permet de pouvoir compiler l'applicatif de notre serveur selon la version de minecraft choisis. 
Votre mission crée une image qui sera utilisé en tant que builder afin de compiler et sortir un fichier spigot-1.14.2.jar.

### Documentation

```https
https://www.spigotmc.org/wiki/buildtools/
```

## Deuxième étape

Dans cette dernière partie vous allez devoir, créez une image d'un serveur minecraft fonctionnel, en récupérant l'applicatif du serveur qui a été compiler par le builder au préalable.

### Obligatoire
Le serveur doit être accèssible depuis le port 25565

### Optionnel
Le serveur doit tourner depuis un utilisateur Linux avec le moins de droits possibles.
