---
title: Aurores - Notes pour les leaders du club
---

#Introduction:
Dans ce projet, les enfants apprendront à animer une scène simple en utilisant CSS. Ils utiliseront la règle @keyframes en CSS pour animer différentes propriétés d'images et de divisions.

#Ressources en ligne

Nous recommandons d'utiliser [trinket](https://trinket.io/) pour écrire du HTML & CSS en ligne. Ce projet contient les trinkets suivants :

+ [Point de départ 'Sunrise'](https://trinket.io/html/web-sunrise)

Des enfants peuvent aussi utiliser ce trinket vide [(jumpto.cc/html-blank)](http://jumpto.cc/html-blank) pour écrire leur propre code HTML & CSS, ou ils peuvent utiliser ce trinket modèle [(jumpto.cc/html-template)](http://jumpto.cc/html-template).

Il y a aussi un trinket contenant une solution d'exemple à tous les challenges :

+ ['Sunrise' terminé](https://trinket.io/html/abcc0284a3)

#Ressources hors ligne
Ce projet peut être [terminé hors ligne](../offline.html) si désiré. Vous pouvez accéder aux ressources du projet en cliquant sur le lien 'Télécharger matériaux du projet' pour ce projet. Ce lien contient un dossier 'Ressources du projet', laquelle inclut des ressources dont les enfants auront besoin pour terminer ce projet en mode hors ligne. Assurez-vous que chaque enfant ait accès à une copie de ces ressources. Ce dossier inclut les fichiers suivants :

+ template/index.html
+ template/prefix.js
+ template/style.css
+ sunrise/index.html
+ sunrise/style.css
+ sunrise/prefixfree.js
+ sunrise/boat.png
+ sunrise/cloud.png
+ sunrise/helicopter.png
+ sunrise/rainbow.png
+ sunrise/sun.png

Vous pouvez aussi trouver une version terminée des challenges de ce projet dans la section 'Ressources bénévoles', qui contient :

+ sunrise-finished/index.html
+ sunrise-finished/style.css
+ sunrise-finished/prefixfree.js
+ sunrise-finished/boat.png
+ sunrise-finished/sun.png
+ sunrise-finished/rainbow.png

#Objectifs d'apprentissage
+ Stylisation et animation avec CSS :
	+ Introduction de la règle `@keyframes` pour définir des étapes dans une animation.
	+ Renforcement de l'utilisation des propriétés pour définir la taille, la forme, la position et la coupe des éléments d'une page Web.

Ce projet couvre des éléments des composantes suivantes de [Raspberry Pi Digital Making Curriculum](http://rpf.io/curriculum):

+ [Conception de ressources 2D et 3D](https://www.raspberrypi.org/curriculum/design/creator).

#Challenges
+ "Animation diagonale" - modification de l'animation des propriétés `@keyframe` à utiliser à gauche :;
+ "Améliorer le ciel" - ajouter plus d'images clés et paramétrage de l'arrière-plan:.
+ "Plus d'animations" - animer plus d'images ou d'éléments en utilisant différentes propriétés CSS. 

#Questions fréquemment posées

+ Ce projet utilise la bibliothèque javascript `prefixfree.js` pour permettre une compatibilité des animations entre les navigateurs. Si cette bibliothèque n'est pas utilisée, alors les enfants utilisant des anciens navigateurs devront déclarer une animation pour leur navigateur, par exemple :

```
animation: sky 10s infinite; 		  	// pour tous les navigateurs plus récents
-webkit-animation: sky 10s infinite;  	// pour les navigateurs Webkit (Chrome, Safari...)
-moz-animation: sky 10s infinite;     	// pour les navigateurs Mozilla
-o-animation: sky 10s infinite;       	// pour les navigateurs Opera
-ms-animation: sky 10s infinite;		// pour les navigateurs Microsoft 
```
