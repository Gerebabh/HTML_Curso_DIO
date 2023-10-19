# HTML II - Ampliando o conhecimento 

Tópicos:

* [HTML - Semântica](#html-semantica)
* [Diferenças do HTML4 para o HTML5](#diferencas-do-html4-para-o-html5)
* [Introdução sobre Acessibilidade](#introducao-sobre-acessibilidade)
* [Introdução ao Web Scraping](#introducao-ao-web-scraping)

___

### [HTML - Semântica](#html-semantica)

**O que é semântica?**
Num sistema linguístico, o componente do sentido das palavras e da interpretação das sentenças e dos enunciados.

Um exemplo para identificar a semântica no caso do HTML. Antes do HTML5 eram utilizadas classes para separar partes do corpo do HTML.

```html
<body>
    <div class="header"></div>  <!--Cabeçalho-->
    <div class="main"></div>    <!--Corpo-->
    <div class="footer"></div>  <!--Rodapé-->
</body>
```

Uma desvantagem de definir classes é que pode ser utilizada qualquer palavra como nome da classe, um exemplo é trocar o `header` por `cabecalho`. 

Com o HTML5, foram introduzidas tags que melhoram a semântica do HTML. Isso significa que as tags são escolhidas de forma a descrever claramente o tipo de conteúdo que contêm. Isso é benéfico não apenas para os desenvolvedores humanos, que podem entender a estrutura do documento de forma mais intuitiva, mas também para os ‘robôs’ de ferramentas de busca e leitores de tela, que podem usar essa informação para fornecer resultados de busca mais precisos ou melhorar a acessibilidade do site. Aqui está um exemplo:

```html
<body>
    <header></header>  <!--Cabeçalho-->
    <main></main>      <!--Corpo-->
    <footer></footer>  <!--Rodapé-->
</body>
```

---

### [Diferenças do HTML4 para o HTML5](#diferencas-do-html4-para-o-html5)

Com o desenvolvimento do HTML5 foram disponibilizadas muitas mudanças / melhorias.

A **W3C** disponibiliza a documentação para consulta sobre estas diferenças. Veja [aqui](https://www.w3.org/TR/html5-diff/).

Foram criados novos atributos e tags, enquanto outros foram alterados ou ficaram obsoletos.

**Exemplos de novos elementos:**

* `<main>`: Representa o conteúdo principal único de um documento ou aplicativo.
* `<header>`: Representa um grupo de conteúdo introdutório ou de navegação.
* `<footer>`: Representa um rodapé para a seção mais próma de ancestrais ou para o corpo inteiro.
* `<nav>`: Representa uma seção de uma página que contém links de navegação.
* `<section>`: Representa uma seção genérica contida em um documento HTML, geralmente com um título.
* `<aside>`: Representa uma seção do conteúdo que é apenas indiretamente relacionada ao conteúdo principal.
* `<article>`: Representa um componente independente de um documento, página, aplicativo ou site.
* `<video>`:    Usado para incorporar conteúdo de vídeo em documentos. Ele pode conter várias fontes de vídeo representadas por elementos filho &lt;source&gt;, dentro do elemento &lt;video&gt;.

**Exemplos de elementos depreciados:**

`<basefont>`, `<big>`, `<center>`, `<font>`, `<strike>`, `<tt>`, `<frame>`, `<frameset>`...

---

### [Introdução sobre Acessibilidade](#introducao-sobre-acessibilidade)

"A acessibilidade é essencial para desenvolvedores e organizações que desejam criar sites e ferramentas da Web de alta qualidade e não excluir as pessoas de usar seus produtos e serviços.

A missão da Iniciativa de Acessibilidade da Web (WAI) é levar a Web a todo o seu potencial para ser acessível, permitindo que pessoas com deficiência participem igualmente na rede."

W3C

**Exemplo:**

```html
<img src="../img/motivacao1.jpg" width="350" alt="Confie no que a vida planejou para você!" />
```

<img src="../img/motivacao1.jpg" width="350" alt="Confie no que a vida planejou para você!" />

Foi inserida uma imagem `.jpg` na página HTML. A imagem se trata de uma mensagem motivacional com os seguintes dizeres: "Confie no que a vida planejou para você!" 

Para aplicar a acessibilidade nesta imagem devemos utilizar a tag `<alt="">`. Desta forma um usuário, por exemplo com deficiência visual ao utilizar um programa que interprete as informações do HTML fará a leitura do texto para o mesmo.

O tema acessibilidade é muito extenso e requer um estudo bem mais aprofundado. Este é apenas um exemplo.

___

### [Introdução ao Web Scraping](#introducao-ao-web-scraping)

**O que é Web Scraping?**

Web Scraping é uma técnica utilizada para extrair grandes quantidades de dados de websites onde os dados são extraídos e salvos em um formato local em seu computador ou em um banco de dados em formato de tabela (csv, xls, etc). O scraping é realizado pegando a página HTML de um site e extraindo os dados que precisamos.

Por exemplo, se quisermos extrair informações sobre produtos de um site de comércio eletrônico, primeiro precisamos entender a estrutura e o padrão do HTML da página. Em seguida, usamos essa estrutura para extrair as informações desejadas.

```html
<div class="product">
    <h2 class="product-name">Nome do Produto</h2>
    <p class="product-price">Preço do Produto</p>
</div>
```

No exemplo acima, se quisermos extrair o nome e o preço do produto, precisaríamos identificar as classes CSS `product-name` e `product-price` e usar essas classes para extrair as informações.

**Por que usar Web Scraping?**

Web Scraping é usado para coletar grandes informações da web. Esses dados podem ser usados para análise de dados, pesquisa de mercado, recuperação de informações e muitos outros propósitos.

**Nota Importante:**

Embora o web scraping seja uma ferramenta poderosa, é importante lembrar que nem todos os sites permitem web scraping. Antes de iniciar um projeto de web scraping, é importante verificar os Termos de Serviço do site para garantir que você não esteja violando nenhuma regra. Além disso, o scraping deve ser feito de maneira responsável e ética para evitar sobrecarregar os servidores do site.
