# HTML - CURSOS DIO ![html5](https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white)

Repositório para Cursos HTML DIO.

1. **Formação HTML Web Developer** - Curso teórico.

* História da Web
* O que são Clients
* O que são Servers
* Linguagens de programação

2. **Introdução do HTML na Prática**

* Ferramentas utilizadas  

![Visual Studio Code](https://img.shields.io/badge/Visual Studio Code-007ACC?style=plastic&logo=Visual Studio Code&logoColor=white) Extensões: `Live Server (Ritwick Dey)` - `Emmet (Pré instalado no VSC)`

3. **Inspetor de elementos**

   O Inspetor de Elementos é uma ferramenta do desenvolvedor e é disponibilizada pelo navegador. Para acessar por exemplo no ![googlechrome](https://img.shields.io/badge/googlechrome-4285F4?style=plastic&logo=googlechrome&logoColor=white) ou no ![microsoftedge](https://img.shields.io/badge/microsoftedge-0078D7?style=plastic&logo=microsoftedge&logoColor=white) basta pressionar `F12`.

4. **Estrutura básica do HTML**

   Crie uma pasta e aponte o caminho no VSCode e crie o primeiro arquivo como `index.html`.

   Por convenção a página inicial do site tem como nome `index.html`. 

   Dentro deste arquivo a estrutura base é:

   ```html
   <html>
       <head>
           <title>Meu primeiro HTML</title> 
       </head>
       <body>
           
       </body>
   </html>
   ```

5. **Atributos das TAGS**

   Os atributos das tags HTML são informações extras que você pode adicionar a uma tag para controlar ou definir suas propriedades. Eles fornecem instruções adicionais sobre como a tag deve funcionar ou aparecer. Por exemplo, em uma tag de imagem `<img>`, o atributo `src` é usado para especificar a origem da imagem que deve ser exibida na página. Em resumo, os atributos das tags HTML são como configurações ou instruções que você pode ajustar para personalizar o comportamento ou a aparência dos elementos HTML em sua página da web.

   ```html
   <body>
       <!-- Rótulo para o campo "nome" -->
       <label for="nome">Informe seu nome:</label>
       <!-- Campo de entrada de texto para o nome -->
       <input type="text" name="nome" /><br />
   
       <!-- Rótulo para o campo "idade" -->
       <label for="idade">Informe sua idade:</label>
       <!-- Campo de entrada de número para a idade -->
       <input type="number" name="idade" /><br />
   </body>
   ```

6. **Textos - Tipografia HTML**

   Neste guia, exploraremos algumas tags HTML relacionadas à tipografia:

   ## `<h1>` - Cabeçalho Principal

   A tag `<h1>` é usada para criar o cabeçalho principal da página, como o título. Existem vários níveis de cabeçalhos, de `<h1>` a `<h6>`.

   ## `<p>` - Parágrafo

   A tag `<p>` é usada para criar parágrafos em seu texto.

   ## `<blockquote>` - Citação

   A tag `<blockquote>` é usada para destacar citações ou observações em seu conteúdo.

   ## `<u>` - Sublinhado

   A tag `<u>` é usada para adicionar sublinhado ao texto.

   ## `<i>` - Itálico

   A tag `<i>` é usada para aplicar estilo itálico ao texto.

   ## `<strong>` - Negrito

   A tag `<strong>` é usada para aplicar estilo negrito ao texto.

   Para ver uma lista completa de tags HTML, você pode consultar a [W3Schools](https://www.w3schools.com/tags/default.asp).

   Aqui está um exemplo de código HTML usando essas tags:

   ```html
   <body>
       <h1>Este é um título</h1>
       <h2>Este é um sub-título</h2>
       <p>
           Este é um parágrafo. "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
           tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
           exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
       </p>
       <blockquote>
           <i>“Inteligência é a capacidade de se adaptar à mudança.”</i>
           <u>— Stephen Hawking</u>
       </blockquote>
   </body>

7. **Listas ordenadas e Não ordenadas**

   Listas ordenadas são apresentadas por números sequenciais e as não ordenadas por asteriscos (*).

   ```html
   <body>
          Lista ordenada
          <ol>
              <li>Item 1</li>
              <li>Item 2</li>
              <li>Item 3</li>
          </ol>
   
          Lista Não ordenada
          <ul>
              <li>Item 1</li>
              <li>Item 2</li>
              <li>Item 3</li>
          </ul>
   </body>
   ```

   ### Lista Ordenada

   1. Item 1
   2. Item 2
   3. Item 3

   ### Lista Não Ordenada

   * Item 1
   * Item 2
   * Item 3

8. **Links**

   Os links no HTML servem tanto para navegação interna como externa conforme a referência informada.

   `<a href="link / url">` - Informa o link para onde o usuário será direcionado.

   `<title>` - Opcional, quando o usuário passar o mouse por cima, será exibido um balão com o texto especificado.

   `<target="_blank">` - Define onde o link será aberto, neste caso em uma nova aba. Caso não seja especificado ou definido como `<target="_self">`  o funcionamento será o padrão, ou seja, abrirá na mesma aba.

   ```html
   <body>
       <a href="https://www.instagram.com/raptorspaintballteam" title="Equipe Mineira de Paintball Speed - INSTAGRAM" target="_blank">Raptors Paintball</a>
       <a href="https://www.facebook.com/rota57ea" title="facebook" target="_blank">Rota 57 Estética Automotiva</a>
   </body>
   ```

   