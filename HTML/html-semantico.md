# HTML Semântico

- HTML semântico é a prática de utilizar a construção do arquvio HTML de forma que os elementos passem mais informação para o usuário e para os dispositivos que vão interagir com essa página, do que apenas uma estrutura de exibição visual.


## O que são Elementos semânticos?

- Elementos semânticos significam elementos com significado.

- Um elemento semântico claramente descreve o seu significado, tanto para o navegador quanto para o desenvolvedor.

- Exemplos de elementos não semânticos (não dizem nada sobre o seu conteúdo):
  - div
  - span

- Exemplos de elementos semânticos (claramente informam o seu conteúdo):
  - form
  - table
  - article


## Porque usar elementos semânticos?

De acordo com a W3C: *"Uma Web semântica permite que os dados sejam compartilhados e reutilizados através das aplicações, empresas e comunidades."*


## Elementos semânticos em HTML

Muitos website apresentam código HTMl como: `<div id="nav">` `<div class="header">` `<div id="footer">` para indicar *navigation*, *header* e *footer*, respectivamente.

Existem alguns elementos semânticos em HTML que podem ser usado para diferentes partes de uma página web:

- `<article>` - Defines independent, self-contained content
- `<aside>` - Defines content aside from the page content
- `<details>` - Defines additional details that the user can view or hide
- `<figcaption>` - Defines a caption for a `<figure>` element
- `<figure>` - Specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.
- `<footer>` - Defines a footer for a document or section
- `<header>` - Specifies a header for a document or section
- `<main>` - Specifies the main content of a document
- `<mark>` - Defines marked/highlighted text
- `<nav>` - Defines navigation links
- `<section>` - Defines a section in a document
- `<summary>` - Defines a visible heading for a `<details>` element
- `<time>` - Defines a date/time


### Elemento HTML `<section>`

O elemento `<section>` define uma seção no documento.

De acordo com a documentação de HTML W3C's: *"Uma **section** é um agrupamento temático de conteúdo, tipicamente com um cabeçalho (tipically with a heading).*

Uma página web pode normalmente ser dividida em seções para intrução, conteúdo e informação de contato.

#### Exemplo de duas seções em um documento:

`<section>`
`<h1>`WWF`</h1>`
`<p>`The World Wide Fund for Nature (WWF) is an international organization working on issues regarding the conservation, research and restoration of the environment, formerly named the World Wildlife Fund. WWF was founded in 1961.`</p>`
`</section>`

`<section>`
`<h1>`WWF's Panda symbol`</h1>`
`<p>`The Panda has become the symbol of WWF. The well-known panda logo of WWF originated from a panda named Chi Chi that was transferred from the Beijing Zoo to the London Zoo in the same year of the establishment of WWF.`</p>`
`</section>`


### Elemento HTML `<article>`

O elemento `<article>` especifica um conteúdo independente e autocontido(*que está enquadrado ou imerso dentro de algo e não ultrapassa seus limites, exemplo: **a água está contida na garrafa.***).

Um *article* deve fazer sentido por si próprio, e deve ser possível distribuí-lo de forma independente do resto do website.

Exemplos onde um elemento `<article>` pode ser usado:

- Post de Forúm
- Post de Blog
- Artigo de jornal

#### Exemplo de 3 artigos com conteúdo independente e autocontido:

`<article>`
`<h2>`Google Chrome`</h2>`
`<p>`Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!`</p>`
`</article>`

`<article>`
`<h2>`Mozilla Firefox`</h2>`
`<p>`Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.`</p>`
`</article>`

`<article>`
`<h2>`Microsoft Edge`</h2>`
`<p>`Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.`</p>`
`</article>`


### Aninhando `<article>` numa `<section>` ou vice-versa?

O elemento `<article>` especifica um conteúdo independente e autocontido.

O elemento `<section>` define uma seção em um documento.

Podemos utilizar as definições deles para decidir como aninhá-los? Não podemos!

Por esse motivo, é possível encontrar páginas HTML com elementos `<section>` contendo elementos `<article>`, e elementos `<article>` contendo elementos `<section>`.


### Elemento HTML `<header>`

O elemento `<header>` representa um container para um conteúdo introdutório ou para definir links de navegação.

Um típico elemento `<header>` contém:

- um ou mais elementos de cabeçalho (`<h1>`-`<h6>`)
- logo ou ícone
- informação de autoria

**Nota**: Você pode ter diversos elementos `<header>` em apenas um documento HTML. No entanto, `<header>` não pode ser inserido dentro de um elemento `<footer>`, `<address>` ou outro elemento `<header>`.

#### Exemplo de utilização de um `<header>` dentro de um `<article>`:

`<article>`
  `<header>`
    `<h1>`What Does WWF Do?`</h1>`
    `<p>`WWF's mission:`</p>`
  `</header>`
  `<p>`WWF's mission is to stop the degradation of our planet's natural environment,
  and build a future in which humans live in harmony with nature.`</p>`
`</article>`


### Elemento HTML `<footer>`

O elemento `<footer>` determina o rodapé para um documento ou uma seção.

Um elemento `<footer>` normalmente apresenta:

- Informação de autoria
- Informação de direito autoral
- Informação de contato
- Um Mapa do site
- Links para retornar para os outros conteúdos da página
- Informação de documentos relacionados

É possível ter diversos elementos `<footer>` in um documento.

#### Exemplo de utilização de um footer em um documento:

`<footer>`
  `<p>`Author: Newton Lomar`</p>`
  `<p>``<a href="mailto:newton@example.com">`newton@example.com`</a>``</p>`
`</footer>`


### Elemento HTML `<nav>`

O elemento `<nav>` determina um conjunto de links de navegação

**É importante destacar que nem todos links de um documento devem estar dentro de um elemento `<nav>`. O Elemento `<nav>` destina-se apenas ao bloco principal de links de navegação.**

**Browsers, como leitores de tela para usuários com deficiência, podem utilizar dessa elemento para determinar se deve-se omitir a renderização inicial deste conteúdo.**

#### Exemplo de um conjunto de links de navegação:

`<nav>`
  `<a href="/html/">`HTML`</a>` |
  `<a href="/css/">`CSS`</a>` |
  `<a href="/js/">`JavaScript`</a>` |
  `<a href="/jquery/">`jQuery`</a>`
`</nav>`


### Elemento HTML `<aside>`

O elemento `<aside>` determina um conteúdo lateral além do conteúdo cujo o qual esse elemento está inserido (*funcionando como uma barra lateral*).

O conteúdo dentro de `<aside>` deve ser indiretamente relacionado ao conteúdo cujo o qual ele está inserido.

#### Exemplo de utilização do elemento `<aside>`, onde é exibido um conteúdo além do conteúdo em que a tag é inserida:

`<p>`My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!`</p>`

`<aside>`
`<h4>`Epcot Center`</h4>`
`<p>`Epcot is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
`</aside>`


### Elementos HTML `<figure>` e `<figcaption>`

A tag `<figure>` especifica um conteúdo autocontido, como ilustrações, diagramas, fotos, lista de códigos, etc...

A tag `<figcaption>` determina a assinatura (ou título/subtítulo, dependendo do contexto) para um elemento `<figure>`. O elemento `<figcaption>` pode ser inserido como o primeiro ou último elemento filho de um elemento `<figure>`.

O elemento `<img>` determina a real imagem/ilustração.

#### Exemplo de utilização dos elementos `<figure>` e `<figcaption>`

`<figure>`
  `<img src="pic_trulli.jpg" alt="Trulli">`
  `<figcaption>`Fig1. - Trulli, Puglia, Italy.`</figcaption>`
`</figure>`


#### Fonte

Esse rascunho teve como base o estudo e a tradução da página: &copy; https://www.w3schools.com/html/html5_semantic_elements.asp

Ele não é uma tradução direta e tem comentários e adições de conteúdos e conclusões de minha autoria: &copy; *Newton Lomar*

##### Links adicionais e úteis:

HTML Tag Reference - w3schoools: https://www.w3schools.com/tags/default.asp

