---
title: Pixel Art
description: Créer un éditeur de pixel art. 
layout: project
notes: "Pixel Art - notes.md"
---

# Introduction { .intro}

Dans ce projet, vous allez créer un éditeur de pixel art. En plus d'utiliser le HTML et le CSS, vous allez apprendre à utiliser le JavaScript pour ajouter de l'interactivité à votre projet.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/0e102a306b?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="images/pixel-art-final.png">
</div>

__Comment utiliser l'éditeur__: Cliquez sur une couleur de la palette pour choisir la couleur de votre feutre puis cliquez sur les pixels pour changer leur couleur.

# Étape 1 : Créer une grille de pixels {.activity}

Créons une grille de pixels que vous pouvez utiliser pour créer du pixel art. Le CSS fournit des styles de tableau pour les grilles et des agencements de tableau. 

Les tableaux contiennent des lignes qui contiennent des cellules. Vous allez créer un tableau avec un arrière-plan noir, puis placer des pixels blancs à l'intérieur. 

## Liste de contrôle de l'activité { .check}

+ Ouvrez ce trinket : <a href="http://jumpto.cc/web-pixel" target="_blank">jumpto.cc/web-pixel</a>. 

	Le projet doit ressembler à ça :

	![screenshot](images/pixel-starter.png)

+ Ajouter le html suivant dans le `<body>` de votre fichier `index.html` pour créer une `<div>` comme conteneur de votre pixel art et donnez-lui un id `art` pour pouvoir y appliquer un style :

	![screenshot](images/pixel-art-art.png)

+ Maintenant, allez dans votre fichier `style.css` et ajoutez la stylisation de tableau pour l'art `<div>`.

	![screenshot](images/pixel-art-style.png)

	Cela crée un tableau avec une bordure et définit l'espacement à l'intérieur de la grille. 

	Il n'a pas l'air très intéressant pour l'instant, vous devez placer des lignes de pixels à l'intérieur. 

 + Maintenant, retournez à ton fichier `index.html` et ajoutez une ligne de 3 pixels à l'intérieur de l'art `<div>` :

	![screenshot](images/pixel-art-row.png)
	
	 Remarquez que les lignes de trois pixels sont les mêmes. Saisissez la première, puis faites un copier/coller pour créer les autres. 

 	Cette fois vous utilisez des classes pour styliser les divisions car il y en aura beaucoup. 

 + Ajoutez le style suivant pour les lignes et les cellules ;

	![screenshot](images/pixel-art-row-style.png)

 	Maintenant, vos pixels s'aligneront dans une grille avec des lignes noires autour. 

 + Ajoutez maintenant deux autres lignes de pixels pour créer une grille 3 x 3. Souvenez-vous d'utiliser la fonction copier/coller pour gagner du temps. 

	![screenshot](images/pixel-art-grid-3.png)
	
    
##Challenge: Redimensionner votre grille {.challenge}

3 x 3 est une grille plutôt petite pour du pixel art. Pouvez-vous la rendre plus grande ? 8 x 8 est une bonne taille pour du pixel art. 

Essayez d'utiliser la fonction couper/coller plutôt que de tout saisir. 

![screenshot](images/pixel-art-grid-8.png)

## Enregistrez votre projet {.save}

# Étape 2 : Colorer les pixels {.activity}

Le HTML est utilisé pour organiser votre contenu et le CSS pour le styliser. Le JavaScript est un langage de programmation qui peut être utilisé pour modifier une page Web et la façon d'interagir avec. 

Vous pouvez utiliser le HTML et le CSS pour définir la couleur de l'arrière-plan des pixels individuels, mais ce sera très long ! Au lieu de ça, vous allez ajouter un peu de code en JavaScript pour colorer les pixels automatiquement lorsque vous cliquez dessus. 

+ En JavaScript, le code est placé dans une `function` qui peut être appelée quand nous souhaitons faire appel à ce code. 

	Vous allez créer une fonction appelée `setPixelColour`

	La fonction `setPixelColour` doit savoir de quel pixel il faut modifier la couleur, c'est un `input`.

	Ajoutez le code suivant au fichier `script.js` pour définir la couleur d'arrière-plan d'un pixel :

	![screenshot](images/pixel-art-set-pixel-colour.png)

	Remarquez que `backgroundColor` utilise les dénominations de couleur américaines. 

+ Nous devons maintenant faire appel à cette fonction pour qu'elle intervienne lorsqu'on clique sur un pixel.

	Le HTML utilise `onclick` pour appeler une fonction lorsqu'un élément est cliqué. Vous allez devoir faire de 'this' l'entrée pour que votre fonction sache de quel pixel il faut modifier la couleur. 

	Allez dans `index.html` et ajoutez le code suivant au premier pixel :

	![screenshot](images/pixel-art-onclick.png)

+ Testez votre code en cliquant sur le premier pixel. Il devrait devenir noir :

	![screenshot](images/pixel-art-black.png)

	Vous n'avez ajouté que le code `onclick` au premier pixel, donc ça ne fonctionnera pas encore pour les autres pixels. 


##Challenge: Rendre tous les pixels cliquable {.challenge}

Pouvez-vous rendre tous les pixels cliquables ? Utilisez la fonction couper/coller pour aller plus vite. 

Créez un petit morceau de pixel art. 

![screenshot](images/pixel-art-black-example.png)

Astuce : Vous pouvez cliquer sur __Autorun__ pour supprimer tous les pixels. 

# Étape 3 : Ajouter une palette de couleur {.activity}

Avez-vous trouvé ennuyeux de ne pas pouvoir modifier la couleur d'un pixel pour la rendre blanche à nouveau en cas d'erreur ? Corrigeons cela en créant une palette de couleurs, pour que vous puissiez cliquer sur une couleur et changer le feutre. 

+ D'abord, créez un style de feutre. 

	Ajoutez le code suivant au bas de votre fichier `style.css` :

	![screenshot](images/pixel-art-pen.png)

+ Maintenant, créez des couleurs de feutre noire et blanche qui utilisent ce style. 

	Ajoutez le code suivant à votre fichier `index.html` après le `<body>` :

	![screenshot](images/pixel-art-palette.png)

	`style=` vous permet d'ajouter du CSS à l'intérieur de votre HTML, ce qui est pratique ici. 

+ Vous voulez pouvoir modifier la couleur du feutre lorsqu'une couleur de la palette est cliquée. 

	Des variables sont utilisées pour stocker les informations. Créons une variable penColour dans `script.js`.

	Ajoutez le code suivant au sommet du fichier :

	![screenshot](images/pixel-art-pencolour.png)

	Puis ajoutez une fonction pour modifier la penColour :

	![screenshot](images/pixel-art-set-pen.png)

+ Il vous faudra aussi utiliser la couleur du feutre lorsque vous modifiez la couleur d'un pixel. 

	Modifiez la fonction `setPixelColour` pour utiliser la variable `penColour` au lieu de `black` :

	 ![screenshot](images/pixel-art-use-pen.png)

+ Vous devez maintenant faire appel à la fonction `setPenColour` lorsqu'un feutre de couleur est cliqué. 

	Ajoutez le code `onclick` en surbrillance à vos couleurs de feutre :

	![screenshot](images/pixel-art-palette-onclick.png)

+ Maintenant, voyez si vous pouvez faire basculer la couleur du feutre du noir au blanc pour remplir ou supprimer des pixels.


## Enregistrez votre projet {.save}

##Challenge: Ajouter plus de couleurs à la palette {.challenge}

Pouvez-vous ajouter plus de couleurs à la palette ? Choisissez les couleurs avec lesquelles vous voulez créer un pixel art. 

Puis créez quelques pixels art.

Indice : La couleur vert clair est appelée `chartreuse`.

![screenshot](images/pixel-art-final.png)

Demandez au leader de votre club si vous pouvez utiliser l'outil de capture d'écran de Windows ou une alternative pour enregistrer une copie de votre pixel art sous forme d'image. 

## Enregistrez votre projet {.save}

