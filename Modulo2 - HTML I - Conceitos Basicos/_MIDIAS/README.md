# HTML I - Conceitos Básicos

#### Trabalhando com Mídias

Neste capítulo vamos conhecer as tags de mídia. 

Uma boa utilização de mídias no HTML poderão enriquecer a experiência do usuário no site.

* `<img>` - Esta tag é usada para incorporar imagens em uma página HTML. Ela permite que você exiba imagens em seu site, especificando o atributo `src` (source) para o URL da imagem. Exemplo:

  ```html
  <img src="imagem.jpg" alt="Descrição da imagem">
  ```

  Atributos úteis de serem utilizados:

  `title="referência da imagem"` - Utilizando ao atributo `title` quando o usuário passar o cursor sobre a imagem aparecerá um balão com a informação descrita neste atributo.

  `alt="descrição da imagem"` - Adicionar uma descrição a imagem possibilita que programas de acessibilidade leiam a descrição da imagem. Exemplo: `alt="Criança jogando futebol em um campo gramado"`.

* `<audio>` - A tag `<audio>` é usada para incorporar áudio em uma página HTML. Você pode especificar a origem do áudio usando o atributo `src` e adicionar controles de reprodução usando o atributo `controls`. Exemplo:

  ```html
  <audio src="musica.mp3" controls></audio>
  ```

* `<video>` -  A tag `<video>` é semelhante à tag `<audio>`, mas é usada para incorporar vídeos. Você pode especificar o vídeo usando o atributo `src` e adicionar controles de reprodução usando o atributo `controls`. Exemplo:

  ```html
  <video src="video.mp4" controls></video>
  ```

* `<track>` - A tag `<track>` é usada para adicionar legendas a um vídeo HTML. Você pode especificar o arquivo de legenda usando o atributo `src` e definir o idioma usando o atributo `srclang`. Exemplo:

  ```html
  <video controls>
      <source src="video.mp4" type="video/mp4">
      <track src="legendas.vtt" kind="subtitles" srclang="pt" label="Português">
  </video>
  ```

  * **Obs.:** O arquivo `.vtt` é um arquivo de texto comum, porém na primeira linha deve conter a informação `WEBVTT`. Exemplo padrão:

  ```vtt
  WEBVTT
  00:00:08.009 --> 00:00:09.640
  Pessoal, nesse primeiro dia não precisa correr, ok!
  ```

* `<iframe>` - A tag `<iframe>` permite incorporar outro documento HTML em sua página, geralmente usado para incorporar conteúdo de outras páginas da web. Você pode especificar a origem usando o 

* atributo `src`. Exemplo:

  ```html
  <iframe src="https://www.exemplo.com"></iframe>
  ```

  

