# HTML II - Ampliando o conhecimento 

### Tags estruturais &lt;section&gt;, &lt;aside&gt; e &lt;nav&gt;

#### &lt;section&gt;

O elemento HTML **`<section>`** representa uma seção autônoma genérica de um documento, que não tem um elemento semântico mais específico para representá-lo. As seções devem sempre ter um título, com pouquíssimas exceções.

```html
<section>
    <h2>Este é um título de seção</h2>
    <p>Este é um páragrafo de exemplo para esta seção</p>
</section>
```

#### &lt;aside&gt;

O elemento [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) `<aside>` representa uma parte de um documento cujo conteúdo está apenas indiretamente relacionado ao conteúdo principal do documento. Os lados são frequentemente apresentados como barras laterais ou caixas de chamada.

Desta forma o que estiver em `<aside>` não precisa necessariamente ter relação ao assunto principal da página. Exemplo: anúncios, classificados, links, etc. Menos importante que o `<section>`.

```html
<article>
  <p>
    The Disney movie <cite>The Little Mermaid</cite> was first released to
    theatres in 1989.
  </p>
  <aside>
    <p>The movie earned $87 million during its initial release.</p>
  </aside>
  <p>More info about the movie…</p>
</article>
```

&LT;**NAV&GT;**

O elemento HTML `<nav>` representa uma seção de uma página cuja finalidade é fornecer links de navegação, dentro do documento atual ou para outros documentos. Exemplos comuns de seções de navegação são menus, sumários e índices.

Um exemplo o `<nav>` foi inserido no `<header>`:

```html
<header>
    <h2>Tags estruturais - &lt;aside&gt;, &lt;section&gt; &lt;nav&gt;</h2>
    <nav>
        <ul>
            <li><a href="#">Item 1</a></li>
            <li><a href="tel: +553199999-8877">Telefone</a></li>
            <li><a href="https://wa.me/553199999-8877" target="_blank">Whatsapp</a></li>
        </ul>
    </nav>
</header>
```

