# Conteúdo das aulas

**Requisitos**: Node.js, VSCode

**Plugins do VSCode**: editorconfig, gitlens, open in browser, SVG preview

## Aula 1

- HTML serve para estruturar a informação em uma página web
- HTML é composto por tags e elementos
- atributos fornecem informações de conteúdo e funcionamento das 
tags e elementos
- existem tags/elementos abertos e vazios
- essencialmente temos duas categorias de elementos: inline e block

## Aula 2

- ul, ol e dt são elementos para criação de listas
- svg é um formato de imagem para imagens vetoriais
- temos 3 formas de escrever CSS: inline(peso 3), internal(peso 2), external(peso1)
- é boa prática sempre utilizar CSS em um arquivo externo para evitar colisões de estilo
- padding é para dar espaçamento interno em um elemento
- margin é para dar espaçamento externo em um elemento
- é possível aplicar margin negativa, porém padding não
- box-model é uma caixa que envolve todo elemento e consiste de `margin`, `border`, 
`padding`, `height` e `width`
- a propriedade `box-sizing: border-box` faz com que o padding e a borda não 
sejam somados com a largura e altura do elemento
- `*` é o seletor global

## Aula 3

- utilizamos `%` como unidade de medida para trabalhar com layout fluido
- para centralizar um elemento horizontalmente utilizamos a 'margin' com o 
valor `auto` e o `width` definido
- a propriedade `background` nos permite manusear o background de um elemento
- um elemento pode conter múltiplos backgrounds
- por padrão o `background-repeat` vem com o valor `repeat`
- a propriedade `background-size: cover` faz com que a imagem se ajuste ao 
elemento a fim de evitar distorções
- para criar um efeito de overlay podemos utilizar o 
`background-image: linear-gradient(rgba(119, 98, 178, 0.6), rgba(119, 98, 178, 0.6)), url(caminho da imagem)`
- podemos importar `fonts` através da tag `<link>`, `@import` ou `@font-face`
- várias propriedades do CSS são passadas de elemento pai para o filho, por exemplo `font-family`
- `letter-spacing`aplica espaçamento entre as letras de um texto
- utilize `text-transform: uppercase` para deixar o texto em maiúsculo
- só utilize letras maiúsculas no HTML caso realmente necessário, por exemplo em siglas

## Aula 4

- classes no CSS possibilitam o reaproveitamento e isolamento de estilos
- a propriedade `list-style: none` remove os pontos da lista
- o `display: inline-block` permite que elementos sejam arranjados lado a lado
- o atributo `target="_blank"` no element `<a>` faz com que o link seja aberto
em uma aba nova
- ao remover o `outline` é boa prática prover alguma forma de enfatizar a interação
do usuário com dado elemento
- pseudo-classes nos permite aplicar um estilo a um elemento sobre um estado
especial, por exemplo: `:hover`, `:focus`, `:first-child`, `:visited`, `:checked` ...
- `transition` nos permite criar animações de alterações de valores das propriedades
- o flex-box layout provê um modo eficiente de dispor, alinhar e distribuir espaçamento
entre elementos que estão contidos em um container flex, indepentente das suas dimensões
- o flex-box é unidirecional, ou seja só conseguimos trabalhar em um dos eixos (x ou y)
por container
- a propriedade `flex-direction` possibilita declarar qual a direção dos
itens de um container flex
- os itens de um container flex são flexíveis e adaptam as suas dimensões para se
encaixarem no container
- para realizar a quebra de linha utilizamos a propriedade `flex-wrap: wrap` e
definimos a largura de cada elemento que estiver contido em um container flex

## Aula 5

- a unidade de medida `vh` é equivalente ao valor relativo à altura do viewport
- `align-items` permite trabalhar com alinhamento dos items na vertical contando
que o `flex-direction` seja `row`
- `justify-content` permite trabalhar com alinhamento e disposição da horizontal contando
que o `flex-direction` seja `row`
- `align-content` permite o alinhamento dos items em um container flex com `flex-wrap`
- o .editorconfig é um arquivo com configurações para o nosso code editor

## Aula 6

-  a tag `main` só é permitida ter 1 por página HTML
- a tag `section` nos permite dividir o conteúdo em seções em nível mais geral
- a tag `article` serve para separar blocos de informações em um nível mais específico
- é uma boa prática nomear as imagens e links com nomes mais descritíveis possível
- um component agrupa conteúdo e comportamento que façam sentido em estarem juntos
- `overflow: hidden` faz com que o conteúdo que ultrapassar as dimensões do elemento 
seja cortado
- utilizamos imagens como `background-image` para imagens que não se remetem ao conteúdo, ou
seja, meramente ilustrativas
- utilizamos imagens com a tag `img`, imagens que se remetem ao conteúdo
- um elemento `position: absolute` se posiciona relativamente ao elemento 
ancestral mais próximo com `position: relative` declarado
- utilizamos as propriedades `top`, `right`, `bottom`, `left` para posicionar um 
elemento absoluto
- a propriedade `z-index` nos permite alteral o nível de profundidade de um elemento,
ou seja, altera o eixo z
- só conseguimos alterar o `z-index` se ao menos nosso elemento tiver o `position` relative
ou absolute
- `object-fit: cover` tem o mesmo efeito que `background-size: cover`, porém em
um elemento `img`

## Aula 7

- a função `rgba(red, green, blue, alpha)` permite declarar uma cor com transparência
- utilize `aria-hidden="true"` em elementos abertos sem conteúdo para que o leitor de tela
não interprete o elemento
- ARIA é a API de acessibilidade do HTML
- os pseudo-elementos nos permitem aplicar estilo em um conteúdo interno de um elemento,
por exemplo: `::firs-letter` primeira letra, `::first-line` primeira linha, `::selection` 
que é o conteúdo selecionado pelo cursor
- com os pseudo-elementos `::before` e `::after` devemos declarar a propriedade `content`
- `::before` e `::after` por padrão tem o `display: inline`

## Aula 8

- o grid layout provê um modo eficiente de dispor, alinhar e distribuir espaçamento 
entre linhas e colunas contidas em um elemento com `display-grid`
- o grid layout é bidirecional, ou seja só conseguimos trabalhar com os dois eixos 
(x para linhas e y para colunas) ao mesmo tempo
- através da função `repeat` conseguimos repetir dimensões das linhas e colunas
- a propriedade `gap` permite declarar a distância entre linhas e colunas
- idealmente criamos classe com estilos desacoplados para reutilização de 
código, exemplo: classe `.grid` sabe estilizar um grid, classe `.grid-col-2`
diz quantas colunas tem o grid

## Aula 9

- o valor `inherit` é utilizado para herdar o valor de alguma propriedade de um 
elemento ancestral que tenha declarado tal propriedade
- utilize as pseudo-classes `:hover` e `:focus` preferivelmente em elementos
focáveis, ou seja, que sejam navegáveis através do teclado: `<a>`, `<button>`
- é possível utilizar features experimentais no CSS utilizando vendor preffix,
exemplo `display: -webkit-box`
- quando uma feature se torna especificação, o vendor preffix não é mais obrigatório
- podemos utilizar features experimentais em orodução contanto que não haja quebra
de layout

## Aula 10

- a sigla BEM vem de: block, element e modifier
- o BEM é uma metodologia que estabelece uma convenção de nomes para classes CSS:
`.block`, `.block__element`, `.block--modifier`, `.block__element--modifier`
- block é o elemento pai, que dá significado ao component, por exemplo `.header`
- element é uma parte que compõe um bloco, por exemplo `.header__title`
- um block pode ser composto por outros blocks
- não crie muita dependência entre elementos, exemplo 
`.social-media__list__item__link`
- os estilos de um bloco devem ser autocontidos e não devem depender de estilos de
blocos ou elementos externos
- um modifier aplica um estilo que modifica alguma propriedade de um bloco ou elemento
- o BEM não estabelece um padrão de nomenclatura para modifiers globais, exemplo `.text-center`
- o BEM traz como benefício a modularidade, reusabilidade e estruturação dos nossos 
components
- blocos bem escritos são como peças de Lego, qua vão se encaixando e compondo outros blocos 
e assim formam o layout
- a metodologia BEM fornece ao nosso código CSS uma estrutura sólida que se mantém simples
e fácil de entender

## Aula 11

- as unidades de medida `em` e `rem` são relativas e se baseiam no tamanho da letra M
da font utilizada na página
- elementos que utilizam `em` irão sempre se basear no `font-size` declarado em algum
elemento ancestral
- caso nenhum elemento ancestral e nem o `body` esteja com o `font-size` declarado,
o elemento irá se basear no `font-size` default do browser
- os elementos que utilizam `rem` irão sempre se basear no `font-size` declarado no elemento
raiz, ou seja o `<html>`
- o `font-size` default dos browsers é `font-size: 100%` que é equivalente à 16px
- se quisermos saber em % qual seria o `font-size` de 10px, basta aplicar uma regra de 3

```
16 -> 100%
10 -> x = 65.2%
```

- o cálculo para conversão de `px` para `em` ou `rem` é bem simples, basta pegar o número
que deseja converter, e dividir pelo font-size base

```
valor / base
20px / 16px = 1.25em ou 1.25rem
```

- e para fazer o inverso, `em` ou `rem` para `px`, basta multiplicar

```
valor * base
2em ou 2rem * 16px = 20px
```

- utilize a base 10px para simplificar o cálculo `20px / 10px = 2em ou 2rem`
- `em` e `rem` são escaláveis, o que possibilita com poucas linhas de código aumentar
ou diminuir as dimensões, espaçamentos e tamanhos de font
- media queries possibilitam aplicar um CSS específico para um tipo de mídia,
seja um tamaho de tela específico, impressão, TV, orientação do device
(portrait ou landscape) ...
- há diversos tipos de media queries: `screen`, `print`, `tv`, `monochrome` ...
- é possível utilizar os operadores lógicos: `not`, `and` e `only`
- podemos inserir diversar regras em uma media querie
`@media (min-width: 769px) and (orientation: landscape)`
- media queries são fundamentais no desenvolvimento de aplicações mobile first,
ou seja, que são desenvolvidas com foco no mobile e, através das media queries
vamos alterando os estilos para telas maiores

