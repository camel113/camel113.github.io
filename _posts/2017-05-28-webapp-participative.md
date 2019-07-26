---
layout: post
title: La première application participative de score en direct
description: La webapp qui permet à tous les passionés du football amateur de partager le score en direct de leurs équipes favorites
image: images/app-participative.jpg
categories: [Tech]
---
En dehors de mes activités professionnelles je développe plusieurs projets personnels avec lesquels j'essaie d'expérimenter de nouveaux concepts et de nouvelles technologies.

Depuis plusieurs années déjà je tiens un site/blog sur [les statistiques du football amateur en Suisse romande](http://www.footstats.ch). Début 2017 mon site recensait plus de 5'000 visiteurs uniques par mois pour environs 20'000 pages vues. L’été passé m’est venu l’idée élaborer un concept de plateforme participative de score en direct susceptible d’intéresser les visiteurs de mon site. Cette plateforme a pris la forme d’une [app iOS](https://itunes.apple.com/ch/app/footstats-live-score-en-direct-football-amateur/id1116387146?l=en&mt=8) et a été téléchargée plus de 1’000 fois. Le principe de fonctionnement est simple. Soit vous êtes un reporter et dans ce cas vous vous créez un compte pour avoir accès aux différents matchs et donner les scores en direct. Soit vous êtes un simple utilisateur et accédez directement à tous les matchs en direct sans avoir besoin de créer de compte. Durant les six premiers mois de vie de l’application plus d’une cinquantaine de matchs ont été reportés et environ 200 personnes se sont inscrites comme reporter.

Après ces premiers mois d’utilisation plusieurs utilisateurs m’ont fait part de leurs besoins de fonctionnalités supplémentaires. Parallèlement à cela les adeptes d’Android souhaitaient avoir une application similaire sur leur store. 
Pour répondre à tous ces besoins j’ai choisi de changer complètement de stratégie et opté pour le développement d’une PWA (Progressive Web App). Pour faire court, une PWA permet d’avoir un comportement presque similaire à celui d’une application native (iOS/Android) directement depuis le navigateur internet de votre smartphone. J’écrirai prochainement sur les avantages et inconvénients des PWA et pourquoi j’ai fait ce choix.

Aujourd’hui plus de 350 utilisateurs sont inscrits sur la plateforme et une centaine de matchs ont pu être suivis en direct sur [live.footstats.ch](http://live.footstats.ch/). Ce concept innovant peut s’adapter à toutes sortes de sports. Le code source de mon application est open source et [disponible sur Github](https://github.com/camel113/livescore-client) et peut donc être repris et développé par n’importe qui.



