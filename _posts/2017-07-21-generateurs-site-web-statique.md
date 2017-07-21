---
layout: post
title: Les générateurs de sites statiques
description: Comment et pourquoi utiliser les générateurs de sites statiques
image: images/staticgen.jpg
---
Comme à mon habitude, il ne s’agit pas ici d’entrer dans les détails techniques mais simplement de développer mon point de vue sur une technologie, une idée ou un concept.

Depuis quelques mois voir quelques années maintenant, les générateurs de sites statiques deviennent de plus en plus populaire. J’en veux pour preuve des sociétés comme Vox Media, Mailchimp, Sequoia Capital ou encore [Footstats](http://www.foostats.ch) ;-) qui ont toutes choisi de se tourner vers cette technologie. Au MEI, nous avons développé le site web des [Jeux Olympiques de la Jeunesse 2020](www.lausanne2020.com/fr/) avec [Jekyll](www.jekyllrb.com) qui est certainement [le générateur de sites statiques le plus populaire](https://www.staticgen.com/). Pour en savoir un peu plus sur ce projet, rendez-vous sur [cet excellent article](http://blog.comem.ch/2017/05/04/les-jeux-olympiques-du-code/) rédigé par le Professeur Daniel Rappo auquel j’ai contribué.

##Comment ça fonctionne.
Sur le web, une grande partie des sites que vous visitez fonctionnent de manière dynamique. Lorsque vous appelez une page depuis votre navigateur, le site appelle une base de données, récupère les informations utiles, produit la page, puis la livre.

Un générateur de site web statique permet de réaliser le travail décrit ci-dessus au préalable. Comme son nom l’indique, il va générer un site web statique. De cette manière, lorsque que vous visitez une page sur un tel site, celui-ci n’a plus de travail à faire puisque toutes les pages sont déjà prêtes.

##Pourquoi faire ?
Mon site fonctionne grâce à Jekyll, vous êtes donc en train de consulter un site web statique. De mon point de vue, si vous souhaitez créer un site web vitrine ou un blog pour votre entreprise, c’est vers un générateur de sites web statiques plutôt que vers un CMS comme Wordpress ou Drupal qu’il faudra vous tourner. Ces derniers sont basés sur le concept de web dynamique décrit précédemment (bien qu’il existe des moyens de contourner cela). Ils permettent de mettre en place rapidement un site internet mais sont sur le long terme plus coûteux. Les CMS doivent être maintenu à jour afin d’éviter les attaques. Ils nécessitent une infrastructure serveur plus complexe avec notamment une base de données. Un site web généré dynamiquement avec Jekyll prendra certainement un peu plus de temps à être mis en place, mais une fois déployé, il sera imbattable en terme de rapidité. Fini aussi les mises à jour à faire régulièrement pour éviter d’être attaqué.

##Conclusion
Il y a évidemment des cas où un CMS classique ou l'utilisation d'un framemork web seront plus appropriés. Les services offerts par des plateformes comme [Contentful](https://www.contentful.com) ou des outils comme [Prose.io](http://prose.io/) permettent aujourd’hui aux éditeurs de maintenir le contenu de site web statique facilement. La montée en puissance du concept JAMStack et les services d’hébergement comme [Netlify](https://www.netlify.com) laisse penser que les générateurs de sites statiques ont encore de beaux jours devant eux.

Lise non exhausite de mes projets intégrant un générateur de sites statiques:
* [Immocars](www.immocars.ch)
* [Footstats](www.footstats.ch)
* [adrienbigler](www.adrienbigler.ch)
* [Carrosserie Alpina](www.carrosserie-alpina.ch)

 
