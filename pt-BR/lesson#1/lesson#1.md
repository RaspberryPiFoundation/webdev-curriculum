# The web

## Introdução

Você já imaginou como a Internet funciona? Claro que sim! Hoje você irá aprender como fazer sites então você poderá ajudar a construir a Internet. Sites são escritos usando __HTML__, é uma sigla em inglês que significa __Linguagem de Marcação Hipertexto__. Você irá encontrar mais como irá construir sua página.

## Passo 1: O que são páginas web?

1. Abra um __text editor__. 
2. Crie um novo documento.
3. Escreva alguma coisa! Por exemplo:
`Olá! Meu nome é... …`
4. Salve o arquivo. Nomei-o de `ola.txt`.
5. Agora encontre o arquivo e o abra novamente. Essa ação abrirá o editor de texto, o que não é muito divertido.
6. Mude a extensão (são as letrinhas que ficam depois do ponto) para `.html`, então agora o arquivo terá o nome de `ola.html`.
7. Abra o arquivo novamente.

Qual programa foi usado para abrir o arquivo dessa vez? O navegador é um programa especial que sabe interpretar arquivos textos escritos usando __Linguagem HTML__. Nós ainda não colocamos nenhum __HTML__, nós simplesmente colocamos algum texto, mas o Navegador não se incomoda! Assim que você deu ao arquivo a extensão `.html`, ele fará o melhor para exibir-lo de modo que você possa compreender.

Isso é algo muito útil: toda vez quando um site contém erros, o Navegador irá tentar achar como exibí-lo de qualquer maneira.

__Como podemos ver esses arquivos?__

Quando você escreve um endereço em seu navegador, você solicita a um outro computador que está sempre ligado para permitir você ver páginas que estão armazenadas nele. Este computador é chamado de servidor. Quando ele recebe uma solicitação de um outro computador, ele checa tudo que for necessário para que os arquivos `.html` e envia junto todas outras coisas que a página necessida, como imagens e vídeos.

// diagrama de como a internet funciona - deve dizer no topo: Eu posso ter esta página for favor? E na parte debaixo: Aqui vamos nós!

## Passo 2: O que é HTML?

HTML é uma linguagem de __marcação__ - que significa que irá ser usada para descrever o que cada coisa é.

Mesmo que o navegador irá tentar exibir as coisas da melhor forma que puder, isso irá o ajudar saber o que são essas coisas.

Para dizer ao navegador o que, nós usamos `tags`.

Tags se parecem com isso:
<p>Alguma coisa escrita.</p>

`<p>` é abreviação de __parágrafo__.

Aqui tem um abertura de uma tag:
`<p>`
e ela termina quando ao final a escrevemos com uma barra:
`</p>`
Dessa forma o navegador sabe que qualquer coisa entre duas tags é um parágrafo de texto.

As tagas podem ter atributos, que são pequenas informações úteis sobre o elemento.
Vamos dar uma olhada na tag de link:
<a href="http://codeclubbrasil.org">Visite o site do Code Club</a>
`<a>` significa __âncora__, o que é como os links são chamados.

Eles também tem uma tag para abrir:
`<a>`
e uma tag para fechar:
`</a>`
mas nós adicionamos um atributo na tag de abertura:
`<a href="http://codeclubbrasil.org">`
`href` é o atributo, e `http://codeclubbrasil.org` é o seu valor.
`href` significa _referência de hipertexto_. Quando um text tem links (ligações) com outro texto dizemos que ele é _hipertexto_, por causa disso ele pode conter imagens, sons e podem estarem linkados com outros textos. O que são feitos de modo um pouco diferente que um texto comum.
`href` diz ao navegador para onde os links devem levar você, e o texto entre as tags será a parte visível do link.

1. Open the `page.html` file.
2. Ask the volunteer whether you can use X-Ray Goggles or developer tools to look at the code (developer is someone who makes things with code).


#### If you can use X-Ray Goggles:
3. Click on the X-Ray Goggles bookmarklet. 
4. Move your mouse around the page. You can see the parts of the page light up, and see what tags they are made of. You can click on each box to see the snippet of code the box is made of.

#### If you are using developer tools:
3. Move around the page. Right click anything interesting, and then click `Inspect element`. A panel will open up which will show you the page's code as the same time as the page.
4. Move your mouse over different pieces of code. The corresponding things on the page will be highlighted, so you can see which bit does what.

 
5. Try to inspect all parts of the page. Can you figure out what the different tag names stand for?

We already know `<p>` and `<a>`.
`<ol>` - ordered list 
`<ul>` - unordered list
`<li>` - list item
`<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>` - headings
`<hr>` - horizontal rule
`<div>` - a box for grouping things
`<img>` - a special element, which unlike others doesn't have a closing tag. We use it for putting the images in.

There are also some tags that we will always use in HTML documents, and they are:
`<html>` - tells the browser where we put out code
`<head>` - inside `<head>` we put things which may be useful to the browser, but which don't appear as text on the page. In this example we put a `<title>` there, which then shows up at the top of the browser window.
`<body>` - that's where we put the things we want to appear on the page

6. Notice how tags can __nest__ within one another. We have the `<a>` tag, which is inside a `<p>` tag, which in turn is inside `<div>`, which is placed inside `<body>`.

Whenever this happens, we say that the tag that is being wrapped is the _child_ and the tag that does the wrapping is the __parent__ element. It's a little bit like a family tree!

7. To the browser all tags of the same kind are the same, but you can mark them out using classes and ids (pronounced aye-dees). 
For example, some of your paragraphs might be introductions, so you could give them a class `introduction`. See if you can spot some classes inside `page.html` .

8. Ids are used to mark unique items on your page. See if you can spot the `div` tag with an `id` of `kitten` in the page.

9. What will happen if you move things around? Let's go back to the code editor. Find an `<ol>` tag in the code and select it with all its got inside, like so:

```HTML
<ol>
	<li>Kittens</li>
	<li>Cake</li>
	<li>Lie-ins</li>
	<li>Playing games</li>
</ol>
```

Now copy it and move it somewhere else. Save the page and refresh it in the browser. How does the order of your code affect the order in which things are displayed in the browser?

## Things to try

* Create your own paragraph of text.
* Make a link that points to another part of page (hint: it is something to do with id - look out for a link that takes you to the kitten).
* Add your own headings where you think they might be useful. What happens if you change the heading numbers, for example from `<h3>` to `<h4>`?
* What would you have to do to link to a different page?
* If you are using developer tools, once you bring up the panel with the code try double-clicking on the code that looks interesting. See if you can change it. Now you get a live preview without having to move between the browser and the code editor. Cool, huh? Now refresh the page. What happened? When you edit code like this it doesn't get saved, so you can preview what would happen if you did, but don't mess up your file, so you can experiment lots and always go back.





