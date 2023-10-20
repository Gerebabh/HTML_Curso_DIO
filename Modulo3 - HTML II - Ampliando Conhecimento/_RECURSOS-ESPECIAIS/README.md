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

