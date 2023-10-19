# HTML II - Ampliando o conhecimento 

### Tags estruturais &lt;article&gt;, &lt;blockquote&gt; e &lt;q&gt;

#### &lt;article&gt;

O elemento HTML **`<article>`** representa uma composição independente em um documento, página, aplicativo ou site, que se destina a ser distribuível independentemente ou reutilizável (por exemplo, em distribuição). Exemplos incluem: uma postagem no fórum, um artigo de revista ou jornal, ou uma entrada de blog, um cartão de produto, um comentário enviado pelo usuário, um widget ou gadget interativo ou qualquer outro item independente de conteúdo.

**Código:**

```html
...
<article class="previsao">
	<h1>Previsão do tempo para Belo Horizonte</h1>
    <article class="day-forecast">
        <h2 class="day-forecast">03 junho 2023</h2>
		<p>Chuva.</p>
    </article>
    <article class="day-forecast">
	    <h2 class="day-forecast">05 junho 2023</h2>
    	<p>Períodos de Chuva.</p>
    </article>
    <article class="day-forecast">
    	<h2 class="day-forecast">06 junho 2023</h2>
    	<p>Chuva forte.</p>
    </article>
</article>
...
```

**Resultado:**

<article class="previsao">
	<h1>Previsão do tempo para Belo Horizonte</h1>
    <article class="day-forecast">
        <h2 class="day-forecast">04 junho 2023</h2>
		<p>Chuva.</p>
    </article>
    <article class="day-forecast">
	    <h2 class="day-forecast">05 junho 2023</h2>
    	<p>Períodos de Chuva.</p>
    </article>
    <article class="day-forecast">
    	<h2 class="day-forecast">06 junho 2023</h2>
    	<p>Chuva forte.</p>
    </article>
</article>

___

#### &lt;blockquote&gt;

O elemento HTML `<blockquote>` indica que o texto incluído é uma citação estendida. Normalmente, isso é renderizado visualmente por recuo. Uma URL para a fonte da citação pode ser dada usando o atributo, enquanto uma representação de texto da fonte pode ser dada usando o elemento `<cite>`.

Vale ressaltar que na tela da sua pagina esse link do `<c>` não será apresentado. Servirá somente como forma semântica para os mecanismos de busca.

**Código:**

```html
<blockquote cite="https://www.pensador.com/frases_stephen_hawking/">
	<p>Eu não tenho nenhuma idéia (de qual seja o meu QI). Pessoas que se vangloriam dos seus QI são perdedores.</p>
    <footer>
        -Stephen, Hawking, <cite>Momento desconhecido</cite>
    </footer>
</blockquote>
```

**Resultado:**

<blockquote cite="https://www.pensador.com/frases_stephen_hawking/">
	<p>Eu não tenho nenhuma idéia (de qual seja o meu QI). Pessoas que se vangloriam dos seus QI são perdedores.</p>
    <footer>
        -Stephen, Hawking, <cite>Momento desconhecido</cite>
    </footer>
</blockquote>

___

&LT;**q&GT;**

Diferente do `<blockquote>` que suporta diversos parágrafos o `<q>`  também é utilizado para citações, porém em pequenos textos.

**Código:**

```html
<q>Este é uma pequena citação. As aspas já são inseridas automáticamente. Também suporta o &lt;cite&gt;</q>
```

**Resultado:**

<q>Este é uma pequena citação. As aspas já são inseridas automáticamente. Também suporta o &lt;cite&gt;</q>
