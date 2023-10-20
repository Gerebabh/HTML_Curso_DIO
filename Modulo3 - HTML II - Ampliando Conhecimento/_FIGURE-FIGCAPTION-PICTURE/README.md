# HTML II - Ampliando o conhecimento

### Tags estruturais &lt;figure&gt;, &lt;figcaption&gt; e &lt;picture&gt;

#### &lt;figure&gt; e &lt;figcaption&gt;

O elemento HTML `figure` representa conteúdo independente, potencialmente com uma legenda opcional, que é especificada usando o elemento `<figcaption>` elementos. A figura, sua legenda e seu conteúdo são referenciados como uma única unidade.

O elemento HTML `<figcaption>` representa uma legenda ou legenda que descreve o restante do conteúdo de seu elemento pai `<figure>`.

**Código:**

```html
...
<figure>
    <img src="https://i.ytimg.com/vi/2SDc_6aMX6Q/maxresdefault.jpg" width="400" />
    <figcaption>Troca de tiro, frontal</figcaption>
</figure>
...
```

**Resultado:**

<figure>
    <img src="https://i.ytimg.com/vi/2SDc_6aMX6Q/maxresdefault.jpg" width="400" />
    <figcaption>Troca de tiro, frontal</figcaption>
</figure>

___

#### &lt;**picture**&gt;

O elemento HTML `<picture>` contém zero ou mais elementos &lt;source&gt; e um elemento `<img>` para oferecer versões alternativas de uma imagem para diferentes cenários de exibição/dispositivo. O navegador considerará cada elemento filho e escolherá a melhor correspondência entre eles. Se nenhuma correspondência for encontrada — ou se o navegador não oferecer suporte ao elemento — a URL do atributo src do elemento será selecionada. A imagem selecionada é então apresentada no espaço ocupado pelo elemento.`<source>` `<picture>` `<img>` `<img>`.

```html
<picture>
    <source srcset="../img/foto1_small.jpg" media="(max-width:700px)">
    <img src="../img/foto1_hd.jpg" />
</picture>
```