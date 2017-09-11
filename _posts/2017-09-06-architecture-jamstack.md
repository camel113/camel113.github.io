---
layout: post
title: L’architecture JAMstack
description: Pourquoi et comment exploiter l'architecture JAMstack
image: images/jamstack.jpg
---
Le concept JAMstack semble prendre de plus en plus d’importance depuis quelques mois. L’architecture JAMstack permet de se débarrasser des liens souvent trop contraignants entre une base de données et un site web. Le principe de cette nouvelle architecture consiste à développer des sites/application web plus performants, mieux sécurisés et plus simple à faire évoluer. 

## Qu'est-ce que le JAM de JAMstack signifie :

* JavaScript: La partie dynamique du site est gérée avec du Javascript côté client (browser).
* API’s: les bases de données deviennent des API’s réutilisables.
* Markup: le contenant et le contenu statique du site web est généré et déployé au préalable (Jekyll, React,…)

## Un peu plus en détail

Si vous ne comprenez rien à ce que je viens d’écrire je vais tenter de vous l’expliquer un peu mieux ici.

Mon précédent [article](/2017/07/21/generateurs-site-web-statique.html) entrait en détail dans la partie M de JAMstack. Avec Jekyll on génère un site web avec des informations statiques. Si l’on souhaite rendre le contenu dynamique, il nous faut alors ajouter du code Javascript. Ce code va nous permettre de nous connecter à des bases de données distantes via des services que l’on appelle API’s. Ces API’s sont accessibles depuis n’importe où sur internet mais peuvent être protégée par différents moyens. Elles permettent par exemple de gérer les commentaires d’un article, d’autoriser les gens à se connecter à une partie admin ou encore d’intégrer un e-commerce.

## Un exemple concret (très simplifié)

Vous possédez un site web statique développé avec Jekyll et vous souhaitez y ajouter une boutique en ligne pour y vendre des livres. Pour mettre en place votre boutique, [Snipcart](https://snipcart.com/) propose un système e-commerce qui s’intègre directement sur votre site statique. 
Pour commencer, vous devez décrire chacun de vos de livres à l’aide de fichiers markdown comme celui-ci.

```
titre: How Google Works
prix: 19.90
slug: how-google-works
sku: HGW
image: http://d.gr-assets.com/books/1422538855l/23158207.jpg
```

Il vous reste ensuite à ajouter quelques lignes de Javascript et d’HTML dans votre code sources pour vous connecter à l’API Snipcart. Toutes la gestion du stock, des ventes et des fichiers se fera alors directement depuis l’interface en ligne (dans le cloud) de Snipcart.

## Mon avis
J’ai personnellement exploité ce concept pour le site [Footstats](http://www.foostats.ch) avec lequel j’ai développé une boutique en ligne pour vendre des maillots. Mon exemple concret est très simplifié, mais la mise en place de Snipcart est extrêmement rapide et la gestion des stocks et l’administration est simplifiée au maximum. En une journée votre site peut se transformer en boutique en ligne pour autant que vous soyez prêt d’un point de vue logistique. Reste à savoir que Snipcart prend 2% sur chacune des transactions. Sur le court terme la solution Snipcart semble imbattable financièrement parlant. Sur le long terme par contre, l’utilisation d’autres solutions comme Magento ou Prestashop s’avèreront peut être plus rentable.