---
title: Lettre Mystère
level: HTML & CSS 1
language: fr-FR
embeds: "*.png"
materials: ["Club Leader Resources/mystery-letter-finished/*.*", "Project Resources/mystery-letter/*.*", "Project Resources/template/*.*"]
stylesheet: web
...

# Introduction {.intro}

Dans ce projet, tu va créer une lettre mystère avec chaque mots découpé de différents morceaux de journal, magazine, bande-desinnée ou encore autre chose.

![screenshot](letter-final.png)

# Step 1: Choisi ton message {.activity}

Les lettres mystère sont utilisé dans les films et les livres pour envoyer des messages secrets.

## Liste d'activité { .check}

+ Réflechi a ton message mystère, 12 mots est à peu pres la bonne longueur. Si tu ne trouves pas de message, utilise celui ci: 'Ton prochain indice est dans le coffre. Le code est 65536'.

+ Écrit le quelque part pour que tu puisses t'en rappeler.

# Step 2: Édite ton message {.activity}

C'est parti, écrit ton message dans ta page web.

## Liste d'activités { .check}

+ Ouvre ce trinket: <a href="http://jumpto.cc/web-letter" target="_blank">jumpto.cc/web-letter</a>. Si tu lis ce projet en ligne, tu peux aussi utiliser la version embarquée de ce trinket ci-dessous.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/b5fbcf112e" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ l'Élément paragraphe `<p>` a été introduit dans le projet 'Joyeux Anniversaire'. l'Élement `<span>` peut être utiliser pour rassembler plusieurs élément de texte a l'intérieur d'un paragraphe pour qu'on puisse le stylé. 

![screenshot](letter-placeholder.png)

## Liste d'activités { .check}

+ Change les mots de ton message en ajoutant un mot par element `<span>`. Tu devras ajouter ou enlever des élements `<span>` si ton message a une longueur différente.

![screenshot](letter-message.png)

## Liste d'activités { .check}

+ Appuie sur le bouton 'Run' pour tester ton trinket.

	Si tu regardes les mots de plus pres, tu peux voir que les mots on été stylé et qu'on dirais qu'ils sont collés a la page.

# Step 3: Utilisation des classes CSS {.activity}

## Liste d'activités { .check}

+ As-tu remarqué la propriété `class=""` dans les éléments `<span>` ? Tu peux utiliser ceci pour stylé plusieurs choses d'une seule facon.

+ Ajoute la classe `magazine1` à quelques elements `<span>` et test ta page web.

![screenshot](letter-magazine1.png)

## Liste d'activités { .check}

+ Tu peux ajouter plus d'une classe un élément. Laisse juste un espace entre chaque classes. Ajoute la class `big` à un de tes éléments`<span>`. Test ta page.

![screenshot](letter-big.png)

## Enregistre ton projet {.save}

## Défi: Style ton message {.challenge}

Utilise les styles deja présent pour tourner ton message en lettre mystère.

Ajoute ces classes à tes élements `<span>`:

+ `newspaper`, `magazine1`, `magazine2`

+ `medium`, `big`, `reallybig`

+ `rotateleft`, `rotateright`

+ `skewleft`, `skewright`

N'ajoute pas plus d'une classe par ligne à un élément `<span>` en particulier.

Voici à quoi ta lettre devrais ressembler:

![screenshot](letter-challenge1.png)

## Enregistre ton projet {.save}

# Step 4: Édite tes classes  {.activity}

## Liste d'activités { .check}

+ Clique sur l'onglet __'style.css'__. Trouve le style pour la classe `newspaper` que tu viens d'utiliser.

![screenshot](letter-newspaper.png)

+ Remarque qu'il y a un point '.' avant chaque nom de tes classes dans ton fichier CSS mais pas sur tes éléments `<span>` dans ton document HTML.

+ Maintenant regarde les autres classes CSS que tu as utiliser pour stylé ta lettre mystère. Peut tu trouver:

	+ Comment la classe `magazine1` change le texte en le rendant tout en majuscules.

	+ Comment la classe `magazine2` ajoute une image derrière le texte.

![screenshot](letter-magazines.png)

+ Que se passe-t-il si tu change la propriété `background-image` de la classe `magazine2` en `canvas.png`? Si tu préferes l'image `pink-pattern.png` tu peux toujours la remettre.

Tu peux aussi changer les couleurs dans tes styles de magazine si tu veux.

+ Trouve le code CSS utilisé pour tourner (`rotate` en anglais) ou incliner (`skew` en anglais) tes mots:

![screenshot](letter-rotate-skew.png)

Essaye de changer les nombres pour créer differents effets et ensuite les tester sur ta page.

# Step 5: Créer une nouvelle classe  {.activity}

On va maintenant créer un nouveau style qui ressemble à une page de bande-dessinnée. <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> te donneras plein d'exemples que tu peux utiliser gratuitement.

## Liste d'activités { .check}

+ Ajoute la classe `comic` dans ton fichier __style.css__. A la suite de `magazine2` est une bonne idée. N'oublie pas le point au debut de ta classe.

![screenshot](letter-comic1.png)

Ne t'inquiètes pas si tu vois une erreur comme 'The Rule is empty' (la règle est vide), on va fixer cela plutard.

+ Maintenant, ajouter plus de CSS à ta nouvelle classe. Tu peux utiliser différentes couleurs si tu veux. Il y a plein de couleurs derrière ce lien <a href="http://jumpto.cc/web-colours" target="_blank">jumpto.cc/web-colours</a>

![screenshot](letter-comic2.png)

+ Utilise les styles de la classe comic sur quelques éléments `<span>` dans ton document HTML et teste ta page:

![screenshot](letter-comic-output.png)

+ Maintenant tu peux ajouter une police un peu plus rigolote. Ouvre un nouvel onglet dans ton navigateur. Va sur la page <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> et recherche le mot __'bangers'__:

![screenshot](letter-fonts1.png)

+ Clique sur le bouton 'Quick-use' (demande l'aide de ton professeur si tu as besoin):

![screenshot](letter-fonts2.png)

+ Une nouvelle page va se charger. Fait défiler ta page jusqu'a ce que tu vois:

![screenshot](letter-fonts-link.png)

Et copie le texte souligné.

+ Copie le code `<link>` que tu viens de copier depuis Google fonts dans ton élément `<head>` de ta page.

![screenshot](letter-fonts-head.png)

Ceci va te permettre d'utiliser la police Bangers dans ta page.

+ Retourne sur ta page Google fonts et fait défiler ta liste encore plus et copie le code `font-family`:

![screenshot](letter-fonts-bangers.png)

+ Maintenant, retourne sur ton fichier __'style.css'__ dans trinket et colle le code `font-family` dans ta classe comic:

![screenshot](letter-fonts-comic.png)

+ Test ta page web. Le resultat devrais ressembler à ceci:

![screenshot](letter-fonts-output.png)

## Enregistre ton projet {.save}

## Défi:  Créer un style écran d'ordinateur {.challenge}

Créer un style écran d'ordinateur à l'ancienne et applique ce style sur quelques-uns de tes mots:

![screenshot](letter-fonts-printout.png)

Tu auras besoin de :

+ La police `VT323` que tu peux trouver ici <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a>. Retourne à l'étape 5 si tu as besoin de revoir comment ajouter une police Google.

+ De l'image de fond `computer-printout-paper.png`. Retourne à l'étape 4 si tu as besoin de revoir comment utiliser les images de fonds.

## Défi: Créer ton prore style {.challenge}

Maintenant crée ta propre classes et rend ta lettre mystère encore plus mysterieuse. Utilise le CSS que tu as appris dans tes projets précédents et regarde les exemples dans ton fichier __style.css__ pour avoir plus d'idées.

Voila un exemple:

![screenshot](letter-fonts-challenge3.png)

Tu peux voir les images qui sont disponible en cliquant sur l'onglet Images dans trinket.
Essaie de mettre une image de fond en utilisant une de ces images:

+ `rough-paper.png`

+ `canvas.png`

Si tu as un compte trinket, tu peux télécharger des images de ton ordinateur comme tu l'as fait dans le projet 'Raconte une histoire'.

Cherche une police que tu aimes sur la page on <a href="http://jumpto.cc/web-fonts" target="_blank">jumpto.cc/web-fonts</a> et copie le lien `<link>` et ajoute le code CSS a ton trinket pour les utiliser.

## Enregistre ton projet {.save}
