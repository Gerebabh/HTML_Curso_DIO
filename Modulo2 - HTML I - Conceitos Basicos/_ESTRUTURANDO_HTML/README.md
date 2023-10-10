# **HTML I - Conceitos Básicos**

#### Estruturando HTML + Formatações

* **Formatando Textos - Parte 1**

  Serão apresentadas formatações básicas de texto.
  <p align="center">Programe o seu futuro global agora!</p>

  **`<i>` - Itálico**.

  <p><i>Programe o seu futuro global agora!</i></p>

  **`<b>` - Negrito**.

  <p><b>Programe o seu futuro global agora!</b></p>

  **`<strong>` - Negrito com ênfase** - Semelhante ao negrito porém aplica ênfase no texto, ou seja, motores de busca e tecnologias assistivas (como leitor de tela para usuários com  deficiência visual) que reconhecem e diferenciam o texto dentro desta tag. Maiores informações em semântica.

  **`<u>` - Sublinhado**.

  <p><strong>Programe o seu futuro global agora!</strong></p>

  <p><u>Programe o seu futuro global agora!</u></p>

  **`<mark>` - Marca-texto**.

  <p><mark>Programe o seu futuro global agora!</mark></p>

  **`<sup>` -** Reduz um pouco o tamanho da fonte e desloca um pouco mais para cima no alinhamento horizontal.

  <p>10<sup>2</sup></p>

  **`<sub>` **- Reduz um pouco o tamanho tamanho da fonte e desloca um pouco mais para cima no alinhamento horizontal.

  <p>10<sub>2</sub></p>

  **`<blockquote>`** - Exibe como citação.

   <p><blockquote>Programe o seu futuro global agora!</blockquote></p>

* **Formatando Textos - Parte 2**

  **`<font>`** 

  Neste caso será utilizado a  tag `<font>` ela aplicada sozinha não produz nenhum efeito e precisa de atributo especificado. 

  Como exemplo a tag `<font>` foi aplicado o atributo `<color="red">`, ou seja, cor vermelha, a fonte alterada para `face="Trebouchet MS, calibri, arial" e essa sequencia de fontes significa que na ausência da primeira definição, seguirá para a próxima e assim em diante.

  Essa tag `<font>` foi descontinuada para o HTML5 e não é mais recomendada para uso ao invés disso é recomendada a utilização do CSS para estilização de texto. Foi citada apenas como exemplo acadêmico de codificação.

  ```html
  <font color="red" face="Trebuchet MS, calibri, arial">Programe o seu futuro global agora!</font>
  ```

  <p><font color="red" face="Trebuchet MS, calibri, arial">Programe o seu futuro global agora!</font></p>

  **`<div>` e `<span>`** 

  A tag `<div>` em HTML é uma tag de nível de bloco que é usada para agrupar elementos e aplicar estilos CSS. Ela não tem nenhum significado semântico por si só, mas é útil para agrupar elementos para fins de estilo ou porque eles compartilham atributos comuns. A tag `<div>` cria uma quebra de linha após o conteúdo, pois é uma tag de nível de bloco.

  Por exemplo:

  ```html
  <div style="color:blue;background-color:rgb(211,243,243);">
    <p>Este é um parágrafo.</p>
    <p>Este é outro parágrafo.</p>
  </div>
  ```

  <div style="color:blue;background-color:rgb(211,243,243);">
      <p>Este é um parágrafo.</p>
      <p>Este é outro parágrafo.</p>    
  </div>

  Neste exemplo, ambos os parágrafos dentro da tag `<div>` terão o texto colorido de azul. Ao utilizar uma DIV ela ocupa a linha inteira, veja a cor de fundo "aqua" que representa o espaço da DIV (display:block).

  Por outro lado, a tag `<span>` em HTML é uma tag de nível de linha que é usada para agrupar elementos em linha ou para aplicar estilos a partes do texto. Ela também não tem nenhum significado semântico por si só. A tag `<span>` não cria uma quebra de linha após o conteúdo, pois é uma tag de nível de linha.

  Por exemplo:

  ```html
  <p>Este é um <span style="color:blue;">texto</span> com uma palavra em azul.</p>
  ```

  <p>Este é um <span style="color:blue;">texto</span> com uma palavra em azul.</p>

  <p>Este é um <span style="color:blue; background-color:rgb(211,243,243);">texto</span> com uma palavra em azul.<p>

  Neste exemplo, a palavra “texto” será exibida em azul, enquanto o restante do texto será exibido na cor padrão.

  **Fieldset**

  O elemento `<fieldset>` em HTML é usado para agrupar elementos relacionados em um formulário. Ele pode ser muito útil para ajudar os usuários a entenderem a estrutura de um formulário, especialmente se ele for longo e complexo.

  A exemplo um formulário de cadastro ao qual temos dados pessoais e endereço.

  Podemos fazer dois fieldset's um que engloba "Dados pessoais" como Nome, E-mail, CPF , etc e  outro com "Endereço" contendo logradouro, número, bairro, cidade, estado.

  Utilizando a tag `<legend></legend>` damos ao fieldset um nome.

  ```html
  <form>
      <fieldset>
          <legend>Dados Pessoais</legend> 
          <div class="row">
              <label>Nome:</label><input type="text" />
              <label>E-mail:</label><input type="text" />
          </div>
  
          <div class="row">
              <label>Profissão:</label><input type="text" />
              <label>Empresa:</label><input type="text" />
          </div>
      </fieldset>
  
      <fieldset>
              <legend>Endereço</legend>
          <div class="row">
              <label>Logradouro:</label><input type="text" />
              <label>Número:</label><input style="width: 30px" type="text" width="10" />
          </div>
  
          <div class="row">
              <label>Bairro:</label><input type="text" />
          </div>
  
          <div class="row">
              <label>Cidade/UF:</label><input type="text" />
          </div>
      </fieldset>
  </form>
  ```

  **Embed**

  A tag `<embed>` em HTML é usada para incorporar conteúdo como arquivos multimídia em uma página da web. Ela foi introduzida no HTML 5 e substituiu a necessidade de usar plugins de terceiros, como o Flash, para incorporar conteúdo multimídia. A tag `<embed>` é uma tag vazia, o que significa que não tem uma tag de fechamento.

  Por exemplo:

  ```html
  <embed src="filme.mp4" width="300" height="200">
  ```

  Neste exemplo, um arquivo de vídeo chamado “filme.mp4” está sendo incorporado na página da web.

  **Frameset**

  A tag `<frameset>` em HTML era usada para dividir a janela do navegador em várias seções, cada uma capaz de carregar um documento HTML separado. No entanto, ela foi descontinuada no HTML5 em favor do uso de iframes e CSS para alcançar layouts semelhantes. Portanto, o uso da tag `<frameset>` não é mais recomendado.

  **Iframe**

  A tag `<iframe>` em HTML é usada para incorporar outro documento HTML dentro do documento atual. Ela substituiu a necessidade de usar a tag `<frameset>`. A tag `<iframe>` é útil para incorporar conteúdo como mapas do Google Maps ou vídeos do YouTube em uma página da web.

  Por exemplo:

  ```html
  <iframe src="https://www.example.com" width="300" height="200"></iframe>
  ```

  Neste exemplo, uma página da web de “www.example.com” está sendo incorporada na página da web atual.

  **Cores**

  Como base para cores podemos consultar o site w3schools [HTML Color Names](https://www.w3schools.com/tags/ref_colornames.asp) e [HTML Color Picker](https://www.w3schools.com/colors/colors_picker.asp).

  As cores podem ser determinadas em seu HTML de várias formas:

  * **Pelo nome** - No código você pode escrever o nome da cor.

  * **RGB** - Combinação de vermelho, verde e azul (Red, Green e Blue).
  * **HEX** - Combinação de vermelho, verde e azul, mas escrito em hexadecimal.
  * **HSL** - Matiz (HUE), Saturação(Saturation) e Iluminação(Lighten). A matiz tem os valores onde 0 é vermelho, 120 verde, 240 azul.
  * **RGBA** - Mesmo que RGB, porém adicionado canal Alpha (Transparência).
  * **HSLA** - Mesmo que HSL, porém adicionado canal Alpha (Transparência).

  

  

  

  

