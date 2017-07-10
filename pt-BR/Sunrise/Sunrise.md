---
title: Nascer do Sol
level: HTML e CSS 2
language: pt-BR
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
...

# Introdução { .intro}

Neste projeto, você vai aprender a usar CSS para criar um nascer do sol animado.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/abcc0284a3?outputOnly=true&start=result" width="600" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="sunrise-final.png">
</div>

# Etapa 1: Criando o sol { .activity}

Vamos começar adicionando uma imagem para o sol e posicionando-a com CSS.

## Lista de atividades { .check}

+ Abra este link de trinket: <a href="http://jumpto.cc/web-sunrise" target="_blank">jumpto.cc/web-sunrise</a>. Se você está lendo isso on-line, você também pode usar o link embutido abaixo.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/5085f92143" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
</div>

+ Olhe dentro do corpo `body` do seu arquivo `index.html` e você vai encontrar os elementos da `div` para o céu (sky) e para o mar (sea).

    ```
    <div id="sky">
    </div>
    
    <div id="sea">
    </div>
    ```

+ Uma imagem para o sol já está inclusa em seu projeto. 

    Adicione a imagem dentro da sua `div` que representa o sol incluindo um `id` para estilizá-la:

    ![screenshot](sunrise-sun-image.png)

+ Uau, a imagem é grande. Vá para o arquivo `style.css` e adicione o código CSS para definir a altura da imagem:

    ![screenshot](sunrise-sun-height.png)

    Observe que a largura é atualizada automaticamente para manter as proporções. 

+ Por fim, vamos adicionar um código para posicionar o sol:

    ![screenshot](sunrise-sun-position.png)


## Salve seu projeto {.save}

# Etapa 2: Animando o nascer do sol { .activity}

Para animar seu nascer do sol, você precisa definir como o sol se move e quanto tempo ele leva para nascer.

Para fazer isso, você deve definir uma lista de __quadros-chave__. Cada quadro-chave define as propriedades CSS de um elemento em um ponto específico em uma animação. 

## Lista de atividades  { .check}

+ Primeiro, você precisa usar `@keyframes` (quadros-chave) para criar uma nova animação chamada sunrise (nascer do sol). 

    Adicione este código CSS ao final do seu arquivo `style.css`:

    ```
    @keyframes sunrise {
        0% {top: 90%;}
        100% {top: 0;}
    }
    ```

    Este código diz ao sol onde ele deve se posicionar no início (`0%`) e no final (`100%`) da animação.

    Como o sol está dentro da `div` do céu, as posições acima `top` e esquerda `left` que você passa são referentes ao céu, sendo `top: 100%` a parte inferior do céu, e não a parte inferior da página.


+ Agora que você criou uma animação do nascer do sol `sunrise`, você só precisa dizer ao seu sol para usá-la! 

    Adicione o código em destaque ao CSS do seu sol:

    ![screenshot](sunrise-sunrise.png)

    Isso faz com que o sol gaste 10 segundos com a animação do nascer do sol.

+ Para executar a animação novamente no Trinket, clique em **Autorun**. 

## Salve seu projeto {.save}

##Desafio: Animação diagonal {.challenge}
Você consegue adicionar um código à animação do nascer do sol `sunrise`, para fazer com que o seu sol inicie no canto inferior esquerdo do céu e se mova na diagonal até chegar a sua posição no centro da parte superior?

Você pode usar a propriedade esquerda `left` para fazer isso, por exemplo:

```
left: 40%;
```

![screenshot](sunrise-left.png)

## Salve seu projeto {.save}


# Etapa 3: Animação infinita { .activity}

Vamos fazer com que a animação se repita para sempre.

## Lista de atividades { .check}

+ Se você quer que o sol nasça e se ponha, basta adicionar mais quadros-chave à animação:

    ```
    @keyframes sunrise {
        0%   {top:90%; left:0;}
        33%  {top:0; left:40%; }
        66%  {top:0; left:40%; }
        100% {top:90%; left:80%; }
    }
    ```

    Isso significa que a animação começa e termina com o sol na parte inferior do céu, e permanece na parte superior de 33% até 66% da animação.

+ Agora, você só precisa adicionar a palavra `infinite` (infinito) à animação `#sun` para que ela se repita para sempre:

    ![screenshot](sunrise-infinite.png)

+ Teste sua animação. O sol continua nascendo e se pondo? 


## Salve seu projeto {.save}

# Etapa 4: Animação do céu { .activity}

A animação não serve apenas para movimento. Vamos animar o céu para que fique noite.

## Lista de atividades { .check}

+ Adicione uma animação chamada `sky` (céu) ao seu CSS:

    ```
    @keyframes sky {
        0% {background: black}
        100% {background: lightblue}
    }
    ```

    Observe que dessa vez você está animando a cor do céu, e não a posição.

+ Adicione um código ao seu céu para que ele use sua nova animação:

    ```
    animation: sky 10s;
    ```

    ![screenshot](sunrise-sky.png)

+ Clique em **Autorun** para testar sua animação. 

## Salve seu projeto {.save}

##Desafio: Melhore o céu {.challenge}

Você consegue alterar a animação do céu para que ele acompanhe o sol e fique azul durante o dia e volte a ser escuro quando o sol se puser? Faça com que isso se repita para sempre. 

![screenshot](sunrise-sky-challenge.png)

##Desafio: Mais animação {.challenge}

Você consegue animar outra imagem? Você pode animar a posição, a cor, a forma, o tamanho, a opacidade, ou qualquer outra coisa que você quiser. Experimente também alterar a duração de suas animações. 

Para cada item que você queira animar, você vai precisar:

+ Incluí-lo em seu HTML com um id
+ Adicionar um estilo para o id
+ Criar uma regra @keyframes
+ Usar `animation:` no estilo para usar a animação definida com @keyframes 

Clique no ícone da imagem para ver as imagens que estão inclusas no projeto:

![screenshot](sunrise-images.png)

Você também pode fazer upload de suas próprias imagens se quiser. 

Não se esqueça de que você também pode colocar itens no mar, assim como no céu:

![screenshot](sunrise-boat.png)

No exemplo, o arco-íris usa opacidade para dissolver a imagem:

```
@keyframes fade {
  0%   {opacity: 0;}
  50%  {opacity: 100;}
  66%  {opacity: 0;}
  100%   {opacity: 0;}
}
```

O barco usa uma posição inicial negativa e uma posição positiva acima dos 100% para que você não possa vê-lo em parte da animação:

```
 @keyframes left-right {
  0%    {left:-50%;}
  100%  {left:200%;}
}
```

## Salve seu projeto {.save}
