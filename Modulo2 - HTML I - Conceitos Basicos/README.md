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

  É um campo onde valores serão inseridos sejam texto ou números entre outros.

  `<input type="text">`: Campo para inserção de texto.

  `<input type="number">`: Permite valores e símbolos matemáticos.

  