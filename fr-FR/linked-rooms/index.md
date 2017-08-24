---
title: Salons Liés
description: Créer un projet Web avec plusieurs 'salons' liés entre eux 
layout: project
notes: "Linked Rooms - notes.md"
---

# Introduction { .intro}

Dans ce projet, vous allez créer un réseau de salons liés, dans lequel chaque salon est une page Web différente que vous pouvez décorer avec HTML. 

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ba5d27ec68?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="images/rooms-hall-finished.png">
</div>

__Instructions__: Cliquez sur les portes pour vous déplacer entre les salons.

# Étape 1 : Établir un lien avec une autre page Web du même projet {.activity}

Les projets Web peuvent être constitués d'un grand nombre de fichiers HTML liés entre eux. 

## Liste de contrôle de l'activité { .check}

+ Ouvrez ce trinket : <a href="http://jumpto.cc/web-rooms" target="_blank">jumpto.cc/web-rooms</a>. 

	Le projet doit ressembler à ça :

	![screenshot](images/rooms-starter.png)

+ Le trinket devrait se lancer automatiquement et vous amener dans le Hall

	![screenshot](images/rooms-hall-start.png)

+ Observez la liste d'onglets de fichier pour ce trinket. Pouvez-vous voir `tvroom.html` ? Cliquez dessus.

	![screenshot](images/rooms-tvroom-html.png)

	Il s'agit d'un autre fichier html dans le même projet. 


+ Pour aller vers `tvroom.html` vous devez ajouter un lien dans `index.html`. 

	Ajoutez le code surligné à l'intérieur de la balise `<div>` avec la classe `room`: 

	![screenshot](images/rooms-link-tvroom.png)

+ Testez votre trinket en cliquant sur le lien __Salon TV__ pour voir la page Web `tvroom.html`.

	Notez que `tvroom.html` possède aussi son propre fichier de style `tvroom.css` qui définit l'agencement de cette page. 

	![screenshot](images/rooms-tvroom-unstyled.png)

	
##Challenge: Ajouter un autre lien {.challenge}

Ajouter un lien `<a>` sur la page Web `tvroom.html` pour revenir à la page Web Hall qui est appelée `index.html`. Le texte du lien doit être 'Hall'.

La page Web Salon TV doit avoir un lien cliquable comme suit :

![screenshot](images/rooms-hall-link.png)

Assurez-vous de tester votre code. Vous devriez pouvoir vous déplacer du Hall à Salon TV et revenir en cliquant sur les liens.  


## Enregistrez votre projet {.save}

# Étape 2 : Ajouter un autre salon {.activity}

Maintenant ajoutons un autre salon, un __Salon de jeux__. 

+ Cliquez sur le bouton ajouter une page __+__ :

	![screenshot](images/rooms-add-page.png)

	Inscrivez `gamesroom.html` comme nom de page :

  	![screenshot](images/rooms-games-html.png)

+ Le HTML pour le __Salon de jeux__ est très similaire à `tvroom.html` donc __copiez_ ceci et__collez-le__ dans `gamesroom.html`.
	
	Modifiez les objets mis en relief pour qu'ils indiquent Jeux et non TV :

	![screenshot](images/rooms-games-html2.png)	

+ Votre `gamesroom.html` utilise maintenant `gamesroom.css` qui n'existe pas encore. 

	Créez `gamesroom.css` en cliquant sur le bouton ajouter une page __+__. 


+ Le CSS pour le __Salon de jeux__ est très similaire à `tvroom.css` donc __copiez_ ceci et__collez-le__ dans `gamesroom.css`.

	![screenshot](images/rooms-add-games-css.png)

+ Ajoutez un lien du Hall vers le Salon de jeux :

	![screenshot](images/rooms-hall-games.png)

+ Testez votre projet en cliquant sur le lien du Salon de jeux

	Le __Salon de jeux__ doit ressembler à ceci :

	![screenshot](images/rooms-games-before.png)

	Pas très excitant, mais vous pouvez corriger cela dans le prochain challenge. 

## Enregistrez votre projet {.save}

##Challenge: Styliser et lier le Salon de jeux {.challenge}

Modifiez le HTML et le CSS pour le __Salon de jeux__ de manière à ce que la page Web ressemble à ceci : 

![screenshot](images/rooms-games-challenge.png)

Indice : Il vous faudra modifier la couleur de l'arrière-plan, la couleur de la police et la couleur de la bordure dans `gamesroom.css`. La couleur vert clair est appelée `chartreuse`.  

Indice : Il vous faudra ajouter un lien `<a>` dans `gamesroom.html` qui dirigera vers `hall.html`.

## Enregistrez votre projet {.save}

# Étape 3 : Faire en sorte que les liens ressemblent à des portes {.activity}

Les liens ne doivent pas être simplement du texte. Faites une porte cliquable en utilisant une balise `<div>`.

## Liste de contrôle de l'activité { .check}

+ Ouvrez `index.html` et ajoutez une balise `<div>` autour du lien textuel __Salon TV__. Cela doit être fait à l'intérieur de la balise `<a>` pour qu'il soit cliquable.

  Ajoutez `id="hall2tv"` pour l'étiqueter comme la porte depuis le Hall vers le Salon TV pour pouvoir appliquer un style à la porte. 

  ![screenshot](images/rooms-tvroom-div.png)  

+ Cliquez sur l'onglet `style.css`, allez au bas de la page et ajoutez le CSS suivant pour modifier la taille et la couleur de la porte :

	![screenshot](images/rooms-door-css1.png)

+ Testez votre page Web en cliquant n'importe où sur la porte, pas seulement sur le texte.

+ Maintenons, essayons d'améliorer l'apparence de porte en ajoutant une bordure autour de trois côtés :

	![screenshot](images/rooms-door-css2.png)

+ Puis ajoutons du CSS pour que le texte sur la porte ait un meilleur rendu :

	![screenshot](images/rooms-door-css3.png)

+ Vous avez probablement remarqué que la porte flotte dans les airs. Corrigeons cela en positionnant la porte à l'intérieur du salon.

	![screenshot](images/rooms-door-position.png)	

+ Testez votre page Web en cliquant sur la porte pour aller dans le __Salon TV__.

## Enregistrez votre projet {.save}

##Challenge: Ajouter plus de portes ! {.challenge}

Transformez les autres liens de votre projet en portes de la même manière. 

Pour chaque porte :

+ Modifiez le lien de la porte pour utiliser une balise `<div>` avec un id comme `hall2games` pour pouvoir y appliquer un style. 

	Par exemple : 

	`<a href="gamesroom.html"><div id="hall2games">Games Room</div></a>`

+ Ajoutez du CSS pour l'id de la porte au fichier `.css` pour son salon. Utilisez _copier_ et _coller_ pour gagner du temps. Vous pouvez faire en sorte que chaque porte ait l'air différente si vous le souhaitez. 

+ Positionnez la porte en utilisant `bottom:` et `left:` ou `right:`.

Le Hall peut ressembler à ça :

![screenshot](images/rooms-hall-doors.png)

Le Salon TV devrait ressembler à quelque chose comme ça :

![screenshot](images/rooms-tvroom-door.png)	


# Étape 4 : Ajouter une image d'arrière-plan {.activity}

Décorons le hall avec une image d'arrière-plan.

## Liste de contrôle de l'activité { .check}


+  Modifiez le `style.css` pour ajouter une image d'arrière-plan au Hall :

	![screenshot](images/rooms-hall-decorated.png)	

	L'image sera répétée pour remplir tout le salon. 


## Enregistrez votre projet {.save}

##Challenge: Ajouter un fond d'écran au Salon de jeux {.challenge}

Pouvez-vous décorer le salon de jeux avec une image d'arrière-plan ?

Vous pouvez utiliser l'image d'arrière-plan `space-invader.png` qui est incluse dans votre projet. 

Pour ce faire :

+ Ajoutez une `background-image:` au CSS `.room` pour le Salon de jeux. 

Le salon décoré devrait ressembler à ça :

![screenshot](images/rooms-games-finished.png)	

## Enregistrez votre projet {.save}

##Challenge: Personnalisez-le ! {.challenge}

Ajoutez plus de salons à votre projet. Souvenez-vous que vous pouvez utiliser __copier__ et __coller__ pour économiser du temps, puis seulement modifier les choses qui doivent être différentes. 

Pour chaque salon :

+ Créez un fichier `.html`
+ Ajoutez plus de liens vers et à partir du nouveau 'salon'.
+ Créez un fichier `.css` avec les styles pour votre nouveau salon et ses portes

Vous pouvez modifier la `background-color:` pour chaque salon. Cliquez sur l'icône images pour voir les images d'arrière-plan que vous pouvez choisir :

![screenshot](images/rooms-images.png)	

## Enregistrez votre projet {.save}

