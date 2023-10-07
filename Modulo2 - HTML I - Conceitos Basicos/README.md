# **HTML I - Conceitos Básicos**

Rever algumas tags HTML. Entender como funcionam os formulários de um website e como uma informação enviada através de formulário chega até o servidor.

* **Tag `<form>`**

  Formulários são elementos essenciais na construção de páginas da web interativas, permitindo que os usuários insiram informações que podem ser enviadas para um servidor. Aqui estão alguns atributos comuns da tag `<form>`:

  `<form name="formulario_A">`: Especifica um nome para o formulário, que é usado principalmente para identificá-lo em scripts JavaScript ou CSS.

  `<form action="url">`: Define para onde o formulário será enviado após o usuário submetê-lo. A URL fornecida como valor do atributo `action` é o destino onde os dados do formulário serão processados.

  `<form target="_blank">`: Controla onde a resposta após o envio do formulário será exibida. Aqui estão os valores comuns:

  * `_blank` - Carrega em uma nova aba;
  * `_self` - Carrega na aba atual;
  * `_parent` - A resposta será exibida na janela pai, útil quando o formulário está aninhado em uma estrutura de frames ou iframes.
  * `_top` -  Isso faz com que a resposta seja exibida na janela superior, substituindo qualquer frame ou iframe existente.

  `<form method="post">`: Indica o método pelo qual o formulário será submetido. Os valores comuns são:

  * `post`: Envia os dados do formulário no corpo da solicitação HTTP, tornando-o mais apropriado para o envio de dados sensíveis, como senhas.
  * `get`: Anexa os dados do formulário à URL, o que pode ser visto na barra de endereço do navegador. Isso é menos seguro para dados sensíveis.

  `<form autocomplete="off">`: Especifica se os campos do formulário serão preenchidos automaticamente pelo navegador. Quando definido como `off`, os campos não serão auto-completados. Se essa tag não for especificada ou for definida como `on`, os campos podem ser preenchidos automaticamente pelo navegador, caso o recurso de autocompletar esteja habilitado.

* **Tag `<input type="">`**  

  É uma tag onde deve ser completada com o seu tipo conforme alguns exemplos abaixo. Além disso podem ser consultadas em [w3Scholls/tags]([HTML input tag (w3schools.com)](https://www.w3schools.com/tags/tag_input.asp)).

  É importante notar que, para os campos `<input>`, o atributo `value` desempenha um papel crucial. O valor que o usuário insere ou seleciona em um campo `<input>` é o que será enviado quando o formulário for submetido. Por exemplo, se tivermos um campo `<input type="text">` e o usuário digitar ‘Olá, mundo!’, esse texto será o valor enviado quando o formulário for submetido. Da mesma forma, para campos `<input type="radio">` ou `<input type="checkbox">`, o atributo `value` especificado na tag é o que será enviado. Portanto, é essencial garantir que os atributos `value` sejam definidos corretamente para capturar as informações desejadas

  `<input type="text">`: Campo para inserção de texto.

  `<input type="number">`: Permite apenas números. Útil para entradas que exigem valores.

  `<input type="range">`: Cria uma barra de deslizamento que permite o usuário escolher um valor específico entre o que foi definido como mínimo e máximo e passos caso tenham sido configurados.

  `<input type="color">`: Exibe seletor de cores.

  `<input type="email">`: Campo para preenchimento de email com formatação correta utilizando o "@".

  `<input type="url">`: Campo parra preenchimento de URL com formatação correta exigindo http:// ou https://.

  `<input type="date">`: Exibe seletor de datas.

  `<input type="week">`: Exibe seletor de semana. (Podem não funcionar em todos os navegadores)

  `<input type="month">`: Exibe seletor de mês. (Podem não funcionar em todos os navegadores)

  `<input type="checkbox">`: Exibe checkbox.

  `<input type="radio">`: Exibe radio-button.

  `<input type="hidden">`: Oculta o campo que guardam informações, porém não são exibidas para o usuário.

  `<input type="file">`: Exibe campo para seleção de arquivos.

  `<input type="search">`: Exibe campo para pesquisa.

  `<input type="submit">`: Exibe botão para "Enviar".

* **Checkbox e Radio**

  * **Checkbox**

  Estes campos são caixas de seleção, porém com uma diferença muito importante entre elas.

  `<input type="checkbox">`: Estes campos são caixas de seleção, porém com uma diferença muito importante entre elas.
  
  ```html
  <input type="checkbox" name="complemento[]" value="Alface" /><label>Alface</label>
  <input type="checkbox" name="complemento[]" value="Bacon"/><label>Bacon</label>
  <input type="checkbox" name="complemento[]" value="Ovo"/><label>Ovo</label>
  <input type="checkbox" name="complemento[]" value="Queijo"/><label>Queijo</label>
  ```

  > Dessa forma, temos um campo de `entrada` do tipo `checkbox` com o nome `complemento` que possui uma lista de elementos devido ao uso de `[]` após o nome. Isso significa que, ao enviar essas informações para um banco de dados usando o método `post`, elas não serão um único item, mas sim tudo o que foi selecionado. *O valor dentro do atributo* `value` *é o que será enviado quando o formulário for submetido.*

  *Complementos*:

  [] - Alface

  [x] - Bacon

  [] - Ovo

  [x] - Queijo
  
  * **Radio**
  
  `<input type="radio">`- Ao utilizar o radio é importante ter em mente que ele é para seleção única entre, ou seja, a seleção de um grupo de opções em um radio-button é exclusiva. Utilizando o mesmo exemplo do fast-food o cliente poderá escolher uma bebida incluída  em seu pedido.
  
  ```html
  <!--Observe que todas as opções são do tipo radio e fazem parte do grupo "bebidas". Portanto, apenas uma opção de bebida pode ser selecionada.-->
  <input type="radio" name="bebidas" value="Suco"/><label>Suco</label>
  <input type="radio" name="bebidas" value="Refrigerante Lata"/><label>Refrigerante lata</label>
  <input type="radio" name="bebidas" value="Cerveja"/><label>Cerveja</label>
  ```

  *O valor dentro do atributo* `value` *é o que será enviado quando o formulário for submetido.*
  
  *Bebidas:*
  
  [] - Suco
  
  [x] - Refrigerante lata
  
  [] - Cerveja
  

* **Button e seus tipos**

  Utilizando a tag `<button>`, podemos criar três tipos de botões que se comportam de forma semelhante, mas têm funcionalidades diferentes.

  * Tipo 1 - Clicável

    `<button type="button"> Clicável </button>` - Ele é apenas clicável, porém pode ser associado ao uso de JavaScript.

    ```html
    <button type="button">Clicável</button> <!--Botão apenas clicável-->
    <button type="button" onclick="alert('Cliquei aqui!')">Associado ao JS</button> <!--Associado ao JS e, ao ser clicado, gera um alerta na tela-->
    ```

  * Tipo 2 - Reset

    `<button type="reset"> Reset </button>` - Este é o botão do tipo Reset. Ele limpa todos os campos do formulário.

    ```html
    <form name="teste_reset">
        Nome: <input type="text" name="nome" /><br />
        Idade: <input type="number" name="idade" /><br />
        Senha <input type="password" name="senha" /><br />
        <button type="reset">Limpar</button>
    </form>
    ```

    

  * Tipo 3 - Submit

    `<button type="submit"> Enviar </button>` - O botão do tipo Submit é usado para enviar o formulário. Uma observação importante é que o botão `submit` permite que o usuário pressione a tecla ENTER em qualquer momento para enviar o formulário. Portanto, é recomendável usar o evento "onsubmit" do JavaScript para validar os campos obrigatórios.

    ```html
    <form name="submit">
        Nome: <input type="text" name="nome" /><br /><br />
        Idade: <input type="number" name="idade" /><br /><br />
    	Senha <input type="password" name="senha" /><br /><br />
    <button type="submit">Enviar</button>
    </form>
    ```

* **Select e seus tipos**

  São campos com respostas predefinidas ao qual o usuário apenas fará a seleção entre as opções apresentadas.

  O `select` pode ser utilizado com alguns parâmetros extras que podem ser úteis. Exemplos:

  * `selected` - O programador determina que alguma das opções já seja pré-selecionada.
  * `placeholder` - O atributo `placeholder` não é suportado na tag `select` em HTML. Ele é comumente usado com as tags `input` e `textarea` para fornecer uma dica sobre o que o usuário deve digitar no campo.
  * `disabled` - Desabilita o campo `select` para que o usuário não possa seleciona-lo.
  * `multiple` - Permite que o usuário selecione mais de uma opção. Caso seja configurado o modo de exibição não será individual como no padrão.

  ```html
  <form name="test_select">
      <label>Nome: </label><input type="text" name="nome"><br /><br />
      <label>Curso: </label>
      <select name="curso" multiple>
          <option selected value="">Selecione o Curso</option>
          <option value="ciencia da computacao">Ciência da computação</option>
          <option value="administracao">Administração</option>
          <option value="desenvolvimento full stack">Desenvolvimento Full Stack</option>
      </select><br /><br />
      <label>Conclusão: </label><input type="date" /><br /><br />
      <button type="submit">Enviar</button>
  </form>
  ```

* **Textarea**

  A tag `<textarea>` é usada para criar uma área de texto que permite ao usuário digitar texto livremente, como comentários, revisões ou qualquer outro tipo de texto de várias linhas. Aqui estão alguns atributos comuns da tag `<textarea>`:

  - `name`: Especifica um nome para a área de texto.
  - `rows` e `cols`: Define a altura e a largura da área de texto, respectivamente.
  - `disabled`: Desativa a área de texto para que o usuário não possa interagir com ela.
  - `readonly`: Faz com que a área de texto seja somente leitura. O usuário pode ver o conteúdo, mas não pode modificá-lo.
  - `maxlength`: Define o número máximo de caracteres que o usuário pode inserir na área de texto.
  - `placeholder`: Fornece uma dica sobre o que o usuário deve digitar na área de texto.

  ```html
  <form name="textarea">
      <p>&lt;textarea name="mensagem"&gt;&lt;/textarea&gt;</p>
      <label>Mensagem: </label><textarea name="mensagem" placeholder="Digite sua mesagem"></textarea><br /><br />
      <button type="submit">Enviar</button>
  </form>
  ```
