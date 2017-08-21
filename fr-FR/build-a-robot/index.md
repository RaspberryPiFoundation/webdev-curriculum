---
title: Construire un Robot
description: Apprenez à positionner des images pour fabriquer votre propre robot.
layout: project
notes: "Build a Robot - notes.md"
---

# Introduction { .intro}

Dans ce projet, vous apprendrez à positionner des images pour créer votre propre robot !

![screenshot](images/robot-final.png)

# Étape 1 : Donner des yeux à votre robot { .activity}

Donnons des yeux à votre robot !

## Liste de contrôle de l'activité { .check}

+ Ouvrez ce trinket : <a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a>.

    Le projet doit ressembler à ça :

	![screenshot](images/robot-starter.png)

+ Chaque image de ce projet possède son propre nom (ou __id__). Par exemple, le lien HTML pour les images des yeux et du visage (â€˜faceâ€™, â€˜eyes1â€™ et â€˜eyes2â€™ commençant à la ligne 8 de votre code) ressemblent à ça :

```
<img id="face" ...>
<img id="eyes1" ...>
<img id="eyes2" ...>
```

+ Vous pouvez utiliser l'id d'une image pour lui donne son propre style, en utilisant le symbole `#`. Cela vous permet de styliser chaque image séparément.

Cliquez sur le fichier `style.css`. Vous voyez comme la taille du visage du robot et celle des autres images sont différentes ?

![screenshot](images/robot-id.png)

+ Ajoutez ce code CSS pour donner un style aux yeux du robot :

```
#eyes1 {
    width: 200px;
}
```

Remarquez que vous stylisez uniquement l'image `eyes1`, en utilisant `#eyes1` dans votre CSS. Si vous préférez, vous pouvez utiliser `#eyes2` ou `#eyes3` à la place !

![screenshot](images/robot-eyes-width.png)

+ Vous remarquez comme chaque image est affichée l'une après l'autre ? Il s'agit d'un positionnement __relatif__. Si vous voulez dire au navigateur exactement où placer les yeux de votre robot, il vous faudra utiliser un positionnement __absolu__ à la place.

Ajoutez ces 3 lignes de code au CSS pour votre image `eyes1` :

```
position: absolute;
top: 200px;
left: 100px;
```

Vous devriez voir les yeux de votre robot se déplacer au bon endroit sur votre robot.

![screenshot](images/robot-eyes-position.png)

Ce code CSS dit au navigateur à quelle distance afficher l'image du sommet/de la gauche de la page Web.

![screenshot](images/robot-eyes-position2.png)

Vous pouvez utiliser `bottom` au lieu de `top` pour dire au navigateur à quelle distance du bas de l'écran afficher l'image, et utiliser `right` au lieu de `left`.

# Étape 2 : Donner une bouche à votre robot { .activity}

Donnons une bouche à votre robot !

## Liste de contrôle de l'activité { .check}

+ Ajoutez le code CSS suivant pour styliser votre image `mouth1` :

```
#mouth1 {
    width: 50px;
    position: absolute;
    top: 200px;
    left: 200px;
}
```

+ La bouche de votre robot a l'air très petite, et elle ne se trouve pas au bon endroit.

![screenshot](images/robot-mouth.png)

Pouvez-vous modifier cela en effectuant des changements dans votre CSS ?

## Enregistrez votre projet {.save}

##Challenge: Concevez votre propre robot {.challenge}
Utilisez ce que vous avez appris pour finir la conception de votre propre robot. Voici quelques exemples de ce à quoi votre robot pourrait ressembler :

![screenshot](images/robot-examples.png)

## Enregistrez votre projet {.save}

##Challenge: Ajoutez vos propres images {.challenge}
Pouvez-vous trouver des images supplémentaires à ajouter à votre robot, et les positionner sur votre page Web ? Vous pouvez même remplacer le visage de votre robot par le vôtre !

```
<img id="face" src="myFace.png">
```

## Enregistrez votre projet {.save} 
