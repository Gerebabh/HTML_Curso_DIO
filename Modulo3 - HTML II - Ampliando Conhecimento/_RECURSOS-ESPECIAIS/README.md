# HTML II - Ampliando o conhecimento

### Recursos Especiais

#### Datalist

O elemento HTML `<datalist>` contém um conjunto de elementos `<option>` que representam as opções permitidas ou recomendadas disponíveis para escolha em outros controles.

Diferente do select que permite exclusivamente os valores determinados o `<datalist>` pemite que o usuário insira informações que não constem na lista. Uma vantagem em relação ao select é que ele oferece o "autocomplete".

 ```html
 ...
 <label for="browsers-datalist">Datalist: </label>
     <input list="browsers" type="search" name="search" />
     <datalist id="browsers">
         <option>Selecione um Navegador</option>
         <option>Google Chrome</option>
         <option>Firefox</option>
         <option>Edge</option>
         <option>Safari</option>
         <option>Opera</option>
     </datalist>
 ...
 ```

____

#### CODE, KBD e PRE

* **`<code>`**

Será exibido o conteúdo estilizado deixando a entender que é um fragmento de código alterando inclusive a fonte para monospace.

* **`<pre>`**

Representa o texto pré formatado que deve ser apresentado exatamente como escrito no arquivo HTML.

* **`<kbd>`**

Esta tag "keyboard" é utilizada para apresentar ao usuário que a informação é um comando no teclado. Ela diferencia a fonte escrita e permite aplicação de estilos CSS.

Veja abaixo a combinação destas três tags:

**Código:**

```html
<P>Para copiar este texto, pressione: <kbd>CTRL</kbd>+<kbd>C</kbd>.</P>
```

```css
/*CSS do kbd*/
kbd {
    border: solid 1px ;
}
```

**Resultado:**

<P>Para copiar este texto, pressione: <kbd>CTRL</kbd>+<kbd>C</kbd>.</P>

___

#### DETAILS e SUMMARY

O elemento HTML cria um widget de divulgação no qual as informações ficam visíveis somente quando o widget é alternado para um estado "aberto". Um resumo ou rótulo deve ser fornecido usando o elemento `<details>` `<summary>`. Um widget de divulgação normalmente é apresentado na tela usando um pequeno triângulo que gira (ou gira) para indicar o status aberto/fechado, com um rótulo próximo ao triângulo. O conteúdo do `<summary>`elemento é usado como rótulo para o widget de divulgação.

**Código:**

```html
<details>
    <summary>Como troco a cor de fundo de um elemento no HTML?</summary>
    <p>Para executar esta ação utilize o comanando <code>background-color</code> no CSS.</p>
</details>
```

**Resultado:**

<details>
    <summary>Como troco a cor de fundo de um elemento no HTML?</summary>
    <p>Para executar esta ação utilize o comanando <code>background-color</code> no CSS.</p>
</details>

___

#### METER e PROGRESS

O elemento `<meter>` representa um valor escalar dentro de um intervalo conhecido ou um valor fracionário. É comumente usado para exibir quantidades como a quantidade de combustível em um tanque ou o espaço disponível em um disco rígido.

**Código:**

```html
<meter min="0" max="100" value="30"></meter>
```

**Resultado:**

<meter min="0" max="100" value="30"></meter>

O elemento `<progress>` exibe um indicador que mostra o progresso da conclusão de uma tarefa, normalmente exibido como uma barra de progresso.

**Código:**

```hmtl
<progress min="0" max="100" value="80"></progress>
```

**Resultado:**

<progress min="0" max="100" value="80"></progress>

___

#### Mark e Java Script

O elemento `mark` representa o texto marcado ou destacado para fins de referência ou notação devido à relevância da passagem marcada no contexto envolvente.

<mark>Este texto foi destacado</mark>

Aqui está um exemplo de como você pode combinar HTML e JavaScript. No campo abaixo, ele buscará letras ou palavras no texto e aplicará o destaque usando o elemento `<mark>`.

```js
<input type="text" id="busca"> <br />
<p id="descricao">Os nossos programas de formação são criados em conjunto com especialistas das empresas mais inovadoras do mundo, aplicando uma metodologia para que você domine as tecnologias utilizadas no mercado e também mergulhe nas novas e mais atuais tecnologias que impactarão o futuro dos negócios digitais.</p>

<script>
    var searchField = document.getElementById('busca');
    var descriptionObject = document.getElementById('descricao');
    var textToSearch = descriptionObject.innerHTML;
    function realizaBusca(busca){
        const regex = new RegExp(`(${busca})(?!(.(?!<mark))*</mark)+`, 'ig');
        const ocurrences = textToSearch.match(regex);
        descriptionObject.innerHTML = textToSearch.replace(regex, `<mark>${busca}</mark>`)
    }

    searchField.addEventListener('keyup', (e) => realizaBusca(e.target.value));
</script>
```

___

#### HTML 5 - Novos Atributos

Algumas tag ainda pouco utilizadas no HTML

- `<autofocus>` - Ao carregar apresenta o campo do formulário destacado e selecionado.
- `<placeholder>` - Preenche com uma espécie de marca d'água um input com uma sugestão.
- `<required>` - Torna o preenchimento do campo obrigatório.
- `<fieldset - disable>` - Usado para desabilitar todos os campos dentro do elemento `<fieldset>`.
- `<textarea - minleght - maxlenght>` -  Permite definir um número mínimo e máximo de caracteres para um campo de texto `<textarea>`.
