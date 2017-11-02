---
layout: post
title: Publier une app NodeJS sur infomaniak avec Git
description: 
image: images/jamstack.jpg
---
Une fois n'est pas coutume, j'ai décidé de publier ici un article purement technique. Pour ma nouvelle app Footstats (bientôt disponible), j'ai besoin d'un serveur Node.js afin d'y déployer une serveur Express JS. Il y a quelques années je déployais mes apps Node.JS sur Openshift car il proposait un mode "Free" plutôt intéressant pour faire tourner de petites applications. Mais depuis peu Openshift à changer son pricing et son infrastructure. Heroku propose lui aussi un mode "Free" mais la mise en veille des applications après 30 minutes d'inactivité pose quelques problèmes d'éfficacité. En cherchant d'autres alternatives à ces deux services bien connu je me suis rappelé qu'il était possible d'installer Node.JS sur les serveurs cloud d'Infomaniak. Etant détenteur d'un tel serveur chez Infomaniak je me suis donc lancé dans le déploiement de mon serveur Express JS sur ce dernier. Voici les quelques étapes qui m'ont permis de déployer un tel serveur.

## Etape 1
Préparer un hébégement sur Infomaniak. Ici j'ai ajouté l'hébérgement _footstats-api_ sur lequel sera installé Node.JS.

## Etape 2 
Demander à Infomaniak d'installer Node.JS sur l'hébérgement créé à l'étape 1. (Il est possible aussi d'installer MongoDB)

## Etape 3
Je souhaite déployer mon serveur avec Git (installé par défaut sur les serveurs cloud Infomaniak), la première chose à faire consiste donc à préparer un dépôt (remote) sur mon serveur cloud. 

Pour cela j'ai d'abord créé un repository

`mkdir MonProjet.git`

J'ai ensuite initialisé