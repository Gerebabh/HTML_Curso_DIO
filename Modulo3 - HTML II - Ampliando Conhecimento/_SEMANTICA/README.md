# HTML II - Ampliando o conhecimento 

### HTML - Semântica

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





