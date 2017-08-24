---
title: Lever de Soleil
description: Créer un lever de soleil animé 
layout: project
notes: Lever de soleil - matériaux
...

# Introduction { .intro}

Dans ce projet, vous apprendrez à utiliser le CSS pour créer un lever de soleil animé.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/abcc0284a3?outputOnly=true&start=result" width="600" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="images/sunrise-final.png">
</div>

# Étape 1 : Créer le soleil { .activity}

Commençons en ajoutant une image pour le soleil et en le positionnant avec un peu de CSS.

## Liste de contrôle de l'activité { .check}

+ Ouvrez ce trinket : <a href="http://jumpto.cc/web-sunrise" target="_blank">jumpto.cc/web-sunrise</a>. 

    Le projet doit ressembler à ça :

	![screenshot](images/sunrise-starter.png)

+ Regardez à l'intérieur du `body` de votre fichier `index.html` et vous trouverez les éléments de `div` pour le ciel et la mer.

    ```
    <div id="sky">
    </div>
    
    <div id="sea">
    </div>
    ```

+ Une image pour le soleil est déjà incluse dans votre projet. 

    Ajoutez l'image à l'intérieur de la `div` soleil en incluant un id pour pouvoir y appliquer un style :

    ![screenshot](images/sunrise-sun-image.png)

+ Whoa, l'image est grande. Allez dans `style.css` et ajoutez le CSS pour régler la hauteur de l'image :

    ![screenshot](images/sunrise-sun-height.png)

    Notez que la largeur est mise à jour automatiquement pour garder les mêmes proportions. 

+ Enfin, ajoutons un peu de code pour positionner le soleil :

    ![screenshot](images/sunrise-sun-position.png)


## Enregistrez votre projet {.save}

# Étape 2 : Animer le lever de soleil { .activity}

Pour animer votre lever de soleil, vous devez définir comment le soleil bouge et combien il met de temps à se lever.

Pour ce faire, vous devez définir une liste __images clés__. Chaque image clé définit les propriétés CSS d'un élément à un point spécifique de l'animation. 

## Liste de contrôle de l'activité { .check}

+ D'abord, vous devez utiliser `@keyframes` pour créer une nouvelle animation appelée lever de soleil. 

    Ajoutez ce code CSS à la fin de votre fichier `style.css` :

    ```
    @keyframes sunrise {
        0% {top: 90%;}
        100% {top: 0;}
    }
    ```

    Ce code indique au soleil où se positionner au début (`0%`) et à la fin (`100%`)de l'animation.

    Puisque le soleil est à l'intérieur de la `div` ciel, les positions `top` et `left` que vous donnez sont comprises dans le ciel, avec `top : 100%` étant le bas du ciel, et non le bas de la page Web.


+ Maintenant que vous avez créé une animation `sunrise`, vous devez simplement dire à votre soleil de l'utiliser ! 

    Ajoutez le code en surbrillance au CSS de votre soleil :

    ![screenshot](images/sunrise-sunrise.png)

    Il indique à votre soleil de passer 10 secondes à animer un lever de soleil.

+ Pour lancer l'animation à nouveau dans Trinket, cliquez simplement sur **Autorun**. 

## Enregistrez votre projet {.save}

##Challenge: Animation diagonale {.challenge}
Pouvez-vous ajouter du code à votre animation `sunrise` pour que votre soleil commence en bas à gauche du ciel et se déplace en diagonale par rapport à sa position pour se retrouver centré au sommet ?

Vous pouvez utiliser la propriété `left` pour le faire, par exemple :

```
left: 40%;
```

![screenshot](images/sunrise-left.png)

## Enregistrez votre projet {.save}


# Étape 3 : Animation infinie { .activity}

Faisons en sorte que l'animation se répète à l'infini.

## Liste de contrôle de l'activité { .check}

+ Si vous voulez que le soleil se lève puis se couche, ajoutez plus d'images clés à votre animation :

    ```
    @keyframes sunrise {
        0%   {top:90%; left:0;}
        33%  {top:0; left:40%; }
        66%  {top:0; left:40%; }
        100% {top:90%; left:80%; }
    }
    ```

    Cela signifie que l'animation commence et se termine avec le soleil au bas du ciel, et qu'il reste au sommet de 33 % à 66 % de l'animation.

+ Maintenant, vous devez simplement ajouter le mot `infinite` à l'animation `#sun` pour qu'elle tourne en boucle à l'infini :

    ![screenshot](images/sunrise-infinite.png)

+ Testez votre animation. Le soleil se lève-t-il et se couche-t-il en boucle ? 


## Enregistrez votre projet {.save}

# Étape 4 : Animer le ciel { .activity}

L'animation n'est pas que pour les mouvements. Animons le ciel pour qu'il soit sombre la nuit.

## Liste de contrôle de l'activité { .check}

+ Ajoutez une animation appelée  `sky` à votre CSS :

    ```
    @keyframes sky {
        0% {background: black}
        100% {background: lightblue}
    }
    ```

    Remarquez que cette fois vous animez la couleur du ciel, et non pas une position.

+ Ajoutez du code à votre ciel pour lui dire d'utiliser votre nouvelle animation :

    ```
    animation: sky 10s;
    ```

    ![screenshot](images/sunrise-sky.png)

+ Cliquez sur **Autorun** pour tester votre animation. 

## Enregistrez votre projet {.save}

##Challenge: Améliorer le ciel {.challenge}

Pouvez-vous changer l'animation du ciel pour qu'il soit en phase avec le soleil, qu'il reste bleu durant la journée et qu'il devienne sombre lorsque le soleil se couche ? Faites en sorte qu'il s'agisse d'une boucle. 

![screenshot](images/sunrise-sky-challenge.png)

##Challenge: Plus d'animations {.challenge}

Pouvez-vous animer une autre image ? Vous pouvez animer la position, la couleur, la forme, la taille, l'opacité (seethroughness) ou tout ce à quoi vous pouvez penser. Essayez également de changer la durée de vos animations. 

Pour chaque objet que vous souhaitez animer, il vous faudra :

+ L'inclure dans votre HTML avec un id
+ Ajouter un style pour l'id
+ Créer une règle @keyframes
+ Utiliser `animation:` dans le style pour utiliser l'animation que vous avez définie avec @keyframes 

Cliquez sur l'icône image pour voir les images qui sont incluses dans le projet :

![screenshot](images/sunrise-images.png)

Vous pouvez aussi mettre en ligne vos propres images si vous le souhaitez. 

N'oubliez pas de placer les objets dans la mer ainsi que dans le ciel :

![screenshot](images/sunrise-boat.png)

Dans l'exemple, l'arc-en-ciel utilise l'opacité pour obtenir un effet d'atténuation :

```
@keyframes fade {
  0%   {opacity: 0;}
  50%  {opacity: 100;}
  66%  {opacity: 0;}
  100%   {opacity: 0;}
}
```

Le bateau utilise une position de départ négative pour que vous ne puissiez pas le voir pendant une partie de l'animation :

```
 @keyframes left-right {
  0%    {left:-50%;}
  100%  {left:200%;}
}
```

## Enregistrez votre projet {.save}
