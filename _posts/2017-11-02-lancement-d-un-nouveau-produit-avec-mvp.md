---
layout: post
title: Lancement d’un nouveau produit avec MVP
description: Développer une application iOS et Android rapidement à l’aide de React Native.
image: images/mvp.jpg
categories: [Tech]
---
La semaine dernière j’ai décidé de me lancer à nouveau dans le développement d’une petite application Footstats pour iOS et Android. Sur les 6 derniers mois, 80% du trafic sur [footstats.ch](https://www.footstats.ch/) provenait de téléphone mobile. 

Actuellement j’exploite le concept de [« Progressive web app »](https://developers.google.com/web/progressive-web-apps/) avec footstats. Mais force est de constater que ce concept peine encore à se démocratiser. D’un point de vue « browser », si Chrome semble être à la pointe des dernières nouveautés, Safari n’implémente pas encore les « Service Workers » qui sont au cœur du fonctionnement des PWA’s. Puisque 50% des visites sur footstats.ch proviennent de Safari, le concept PWA est donc à remettre en question pour le moment. D’un point de vue utilisateur, je doute que beaucoup de personnes « installent » ou savent comment installer une progressive web app sur leurs smartphones. Footstats présente du contenu mis à jour quotidiennement et les visiteurs ont tendance à le visiter plusieurs fois par semaine voire plusieurs fois par jour (58% returning visitors sur les 6 derniers mois). Pour toutes ces raisons, j’ai choisi de développer une application native. 

## MVP

Les chiffres cités précédemment et mon ressentit m’ont donc poussé à développer une application native iOS/Android. J’ai choisi d’exploiter la technique [MVP (Minimum Viable Product)](https://en.wikipedia.org/wiki/Minimum_viable_product) pour le lancement de cette nouvelle application. Cette technique, comme son nom l’indique, permet de développer rapidement un produit avec le minimum de fonctionnalités à faire tester et valider rapidement par les utilisateurs. 

## React Native

Pour mettre en pratique la stratégie MVP il me fallait donc choisir des technologies qui me permettaient de développer simplement une première version de mon application. Je me suis donc tourné vers [React Native](https://facebook.github.io/react-native/) qui est un framework de développement qui permet de créer des applications hybrides. En d’autres termes, avec ce type de framework, je peux développer une application pour Android et iOS avec le même code source plutôt qu’avec un code source pour chaque plateforme.

Il y a un peu plus d’une année j’avais déjà expérimenté cela avec [une application de score en direct pour le foot amateur](/2017/05/28/2017-05-28-webapp-participative). Je ne partais donc pas de zéro.

## L’application

L’application développée ici consiste à afficher les classements équipes et buteurs pour chaque régions et ligues de Suisse. Il s’agit donc simplement d’afficher des listes de données que je récupère sur un service (API) existant que j'avais déjà développé pour le site footstats.ch

J’ai choisi d’utiliser le même type de navigation et de design sur iOS et Android car je constate que c’est une tendance actuelle. Des applications comme AirBnB sont très semblables voir similaires sur iOS et Android. React Native permet d’afficher certains éléments différemment sur iOS ou Android mais j’ai fait le choix de faire deux applications identiques pour le moment dans une logique de stratégie MVP.

En un week-end j’ai donc réussi à sortir une première version de mon application.

<img src="/images/footstats-app.jpg" alt="Footstats App" class="post-image" />

## La communication et le retour utilisateur

Le concept MVP privilégie les utilisateurs de type « early adopter ». Comme son nom l’indique se sont les utilisateurs qui ont déjà témoigné un intérêt pour vos services ou vos produits. Je dispose déjà d’une liste d’environ 80 mails d’utilisateurs qui m’écrivent régulièrement sur footstats.ch pour me communiquer des erreurs dans les classements ou simplement pour me donner leurs avis. J’ai donc choisi de faire partir une newsletter vers ceux-ci afin de les informer de la sortie de ma nouvelle application. Les premiers retours utilisateurs ont été positifs et m’ont permis de faire quelques améliorations graphiques.

Mon produit étant validé par les premiers utilisateurs, je vais pouvoir maintenant m’attaquer au « grand public ». Dans les prochaines semaines je vais tenter de faire connaître mon application de différentes manières (réseaux sociaux, blog, newsletter). Toutefois la sortie de cette application coïncide avec la fin de la saison régulière de football, le public cible sera peut-être un peu moins sensibles à mes annonces. Je donnerai les statistiques de téléchargement dans les prochaines semaines.

### Mises à jour

<img src="/images/footstats-app-2.jpg" alt="Footstats App mise à jour" class="post-image" />

#### Janvier 2018
Au mois de janvier j'ai publié à plusieurs reprises des posts (non payants) sur les réseaux sociaux via la page Facebook et le compte Instagram Footstats.ch. L'application a été téléchargée plus de 250 fois (60% iOS, 40% Android). Avec le développement de cette application native, j'ai choisi de changer mon business model et d'expérimenter les achats intégrés. Au mois de janvier, je dénombre 28 achats intégrés (20 iOS, 8 Android).

Ces chiffres sont plutôt encourageants puisqu'en moyenne [5% des utilisateurs d'applications procèdent à des achats intégrés](https://www.appsflyer.com/pr/new-report-global-app-spending-habits-finds-asian-consumers-spend-40-apps-rest-world/). Si on comptabilise chaque application comme étant un utilisateur, l'application Footstats possède une moyenne d'environ 11% d'utilisateurs payants.

#### Février 2018
On se rapproche du début du deuxième tour. Habituellement les visites sur Footstats.ch augmentent drastiquement dès la mi-mars. Pour l'instant toujours aucune promotion payante. Au mois de février, l'application a été téléchargée plus de 270 fois (55% iOS, 45% Android). Côté achats intégrés on dénombre 19 transactions. Ces chiffres sont toujours aussi prometteurs même si les chiffres Footstats collent maintenant avec [les standards](https://www.appsflyer.com/pr/new-report-global-app-spending-habits-finds-asian-consumers-spend-40-apps-rest-world/).

#### Mars 2018
Le mois de Mars est synonyme de reprise dans la plupart des championnats amateurs en Suisse. Cela signifie pour l'application Footstats le début des choses sérieuses. Les chiffres de ce mois passé sont plutôt encourageants. On recense environ 600 téléchargements sur iOS et 350 sur Android. Du côté des achats intégrés, 82 au total (75% iOS, 25% Android). Chiffre intéressant, environ 8.6% des utilisateurs sont des utilisateurs payants si on comptabilise chaque téléchargement d'application comme étant un utilisateur.

#### Avril 2018
Les chiffres pour le mois d'avril sont clairement à la hausse. Au total, 1'900 téléchargements et 170 achats intégrés. Autre statistique intéressante, les 3'200 utilisateurs actifs par mois.

#### Mai 2018
La saison 2017/2018 se termine durant le mois de mai dans la majorité des régions. Pour ce qui représente certainement le dernier gros mois de cette saison, Footstats dénombre 1'550 téléchargements et 175 achats intégrés. Le nombre d'utilisateurs actifs par mois dépasse maintenant la barre des 4'000.

#### Juin 2018 à Octobre 2018
Après un été plutôt calme dû à l'absence de compétition, la saison 2018/2019 a débuté fin août. Pour cette nouvelle saison Footstats a fait peau neuve avec un tas de nouvelles statistiques disponibles pour chaque ligue. Les achats intégrés ont évolué, l'app propose maintenant des IAP (in app products) entre 2.- CHF et 5.- CHF. A mi-octobre l'app a franchi le seuil symbolique des 5'000 utilisateurs actifs 🎉.

J'ai décidé de clore les mises à jour de cet article. Pour suivre l'évolution des chiffres de l'application, rendez-vous sur [mon profil LinkedIn](https://www.linkedin.com/in/adrien-bigler-6408a2a1/). 