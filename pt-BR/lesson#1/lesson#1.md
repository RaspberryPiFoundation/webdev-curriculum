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

As tags podem ter atributos, que são pequenas informações úteis sobre o elemento.
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

1. Abra o arquivo `page.html`
2. Pergunte a um voluntário se você pode usar o Óculos de Raio X (X-Ray Googles) ou o Inspetor Web para olhar o código (desenvolvedor é alguém que faz coisas com código).

#### Se você preferir usar o Óculos de Raio X:
3. Clique no bookmark X-Ray Googles.
4. Mova seu mouse sob a página. Você pode ver as partes da página acendendo, e ver também com quais tags elas são feitas. Você também pode clicar em cada elemento para ver o seu trecho do código.

#### Se você preferir o Inspetor Web:
3. Mova o cursor sobre a página. Clique com botão direito em algum local interessante, e então escolha a opção `Inspecionar elemento`. Um painel será aberto e lhe mostrará a página e o seu código.
4. Mova o mouse por diferentes pedaçõs do código. As áreas correspondentes irão acender, então você pode ver do que ela é feita.

5. Tente inspecionar todas as partes de uma página. Voce pode descobrir o que os diferentes nomes de tags representam?

Nós já conhecemos `<p>` e `<a>`.
`<ol>` - lista ordenada 
`<ul>` - lista não ordenada
`<li>` - item da lista
`<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>` - títulos
`<hr>` - linha horizontal
`<div>` - uma caixa para agrupar as coisas
`<img>` - um elemento especial, que diferente das outras tags não possui tag de fechamento. Serve para carregar imagens na página.

Também existem algumas tags que serão sempre usadas em documentos HTML, são elas:
`<html>` - fala para o navegador onde ele vai pegar o código
`<head>` - dentro do `<head>` é onde nós colocaremos as coisas úteis para o navegador, mas não serão visíveis para na página. Como exemplo disso temos o `<title>` aqui, que será o título da aba na janela do navegador.
`<body>` - É onde nós colocaremos todas as coisas que desejaremos que apareça na página.

6. Atenção como as tags podem __aninhar__ umas com as outras. Nós temos a tag `<a>`, que está dentro de um `<p>`, que está por sua vez dentro de um `<div>`, posicionado dentro do `<body>`.

Sempre que isso acontece, nós dizemos que a tag que está sendo envolvida é a _filha_ do elemento _pai_ que está o envolvendo. É bem parecido com uma árvore geneológica!

7. Para o navegador todas as tags do mesmo tipo são a mesma, mas você pode diferenciá-las usando classes (class) e ids (pronuncia-se ai-dís)
Por exemplo, alguns dos seus parágrafos devem ser introduções, então você pode atribuir a ele a classe `introducao`. Veja se consegue identificar algumas classes dentro do arquivo `page.html`.

8. Ids são usados para marcar itens únicos em sua página. Veja se consegue identificar a tag `div` com um `id` de `gatinho` na página.

9. O que acontecerá se você trocar as coisas de lugar? Vamos voltar para o editor de código. Encontre uma tag `<ol>` no código e selecione com tudo que estiver dentro, desse modo:

```HTML
<ol>
	<li>Gatinhos</li>
	<li>Bolo</li>
	<li>Descansos</li>
	<li>Jogando</li>
</ol>
```
Agora copie e mova as coisas de lugar. Salve a página e atualize o navegador. Como a ordem do seu código afetou a ordem das coisas que estão sendo exibidas no navegador?

## Experimente

* Criar seu próprio parágrafo.
* Fazer um link que aponte para outra parte da página (dica: é algo com id - procure por um link que leve você ao gatinho).
* Adicione seus títulos onde você acha que vão ser uteis. O que acontece se você mudar o número do título, por exmeplo de um `<h3>` para um `<h4>`?
* O que teria que fazer para fazer um link para uma página diferente?
* Se você estiver usando Inspetor Web, uma vez que você abri-lo tente clicar duas vezes em um código que parece interessante. Veja se você consegue mudá-lo. Agora você tem uma prévia do que irá acontecer sem alternar entre o navegador e o editor de códigos. Maneiro, né? Agora, atualize a página. O que aconteceu? Quando você editar o código dessa maneira ele não é salvo, então você pode visualizar o que aconteceria, mas sem não atrapalhar seu arquivo, então você pode experimentar muitas e sempre voltar.





