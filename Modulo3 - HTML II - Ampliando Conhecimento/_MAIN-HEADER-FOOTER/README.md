# HTML II - Ampliando o conhecimento 

### Tags estruturais &lt;header&gt;, &lt;main&gt; e &lt;footer&gt;

A tag `<main>` deve ser filha direta de `<body>` e nenhuma outra. Ela é projetada para desenvolver o conteúdo principal de uma página web. Portanto deve haver apenas uma tag `<main>` por página.  

```html
...
<body>
    <main>
        <!--Conteúdo principal da página.-->
    </main>
</body>
...
```

Entretanto as tags estruturais como exemplo `<header>`, `<footer>`, `<article>`, `<nav>` entre outras podem ser filhas da tag `<main>`. Mesmo as tags `<header>` e `<footer>`  podendo serem utilizadas dentro da tag `<main>` é recomendado que elas sejam filhas diretas da tag `<body>`. Portanto, alinhado com as melhores práticas, uma vez que estas tags geralmente representam elementos globais da página, como cabeçalho e rodapés, que não estão diretamente relacionados ao conteúdo principal da página a melhor forma de construir o HTML é esta:

```html
...
<body>
    <header>
        <!--Conteúdo do cabeçalho.-->
    </header>
    <main>
        <!--Conteúdo principal da página.-->
    </main>
    <footer>
         <!--Conteúdo do rodapé.-->
    </footer>
</body>
...
```

