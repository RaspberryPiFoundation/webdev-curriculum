---
title: Nascer do Sol — Notas para instrutores
language: pt-BR
embeds: "*.png"
materials: [""]
...

#Introdução:
Neste projeto, as crianças vão aprender a animar uma cena simples usando CSS. Elas vão usar a regra CSS @keyframes para animar várias propriedades de imagens e divs.

#Recursos on-line

Recomendamos o uso do [trinket](https://trinket.io/) para escrever HTML e CSS on-line. Este projeto contém os links para os seguintes trinkets:

+ ['Nascer do sol' - ponto de partida](https://trinket.io/html/web-sunrise)

Há ainda um link para trinket que contém uma solução de exemplo para os desafios:

+ ['Nascer do sol' completo](https://trinket.io/html/abcc0284a3)

#Recursos off-line
Este projeto pode ser [feito off-line](../offline.html) se você quiser. Também é possível acessar os recursos do projeto clicando no link 'Download Project Materials' deste projeto. Este link contém uma pasta 'Project Resources', que inclui recursos que as crianças precisam para completar o projeto off-line. Lembre-se de que cada criança precisa ter acesso a uma cópia desses recursos. Esta seção inclui os seguintes arquivos:

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

Você também pode encontrar uma versão finalizada dos desafios do projeto na pasta 'Volunteer Resources', que contém:

+ index.html
+ style.css
+ prefixfree.js
+ boat.png
+ sun.png
+ rainbow.png

#Objetivos de aprendizado
+ Estilização e animação com CSS:
	+ Introdução da regra `@keyframes` para definir as etapas de uma animação.
	+ Reforçar o uso de propriedades para definir o tamanho, a forma, a posição e a cor de elementos em uma página web.

#Desafios
+ "Animação diagonal" - edite as propriedades de animação de`@keyframe` para usar a esquerda left:;
+ "Melhore o céu" - adicione mais quadros-chave e defina o fundo background:.
+ "Mais animação" - anime mais imagens e elementos usando várias propriedades CSS. 

#Perguntas frequentes

+ Este projeto usa a biblioteca `prefixfree.js` do javascript, para permitir a compatibilidade da animação entre navegadores. Se essa biblioteca não for usada, as crianças que usam navegadores mais antigos vão precisar declarar uma animação para o navegador, por exemplo:

```
animation: sky 10s infinite; 		  	//para todos os navegadores mais novos
-webkit-animation: sky 10s infinite;  	// Para navegadores Webkit (Chrome, Safari...)
-moz-animation: sky 10s infinite;     	// Para navegadores Mozilla
-o-animation: sky 10s infinite;       	// Para navegadores Opera
-ms-animation: sky 10s infinite;		// Para navegadores Microsoft 
```