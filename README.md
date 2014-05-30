Micro Workshop Online do Tableless
===================
#### Assunto: Responsive Web Design
[O vídeo do Workshop Online do Tableless pode ser visto aqui](https://www.eventials.com/tableless/live-coding-implementando-um-site-responsivo/).

#Anotações do treinamento:

### METATAG VIEWPORT:
- Resolução é diferente de tamanho de tela.
- Um iphone, com tela pequena, tem uma resolução bem grande.
- Você não trabalha com resoluções, você trabalha com tamanhos de tela.
- A Metatag Viewport, faz a resolução ficar do mesmo tamanho que a tela do aparelho. Ou quase isso.
- Essa é a metatag padrão que uso nos meus projetos.
[code]
	<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
[/code]

Ref: [Manipulando a Metatag Viewport](http://tableless.com.br/manipulando-metatag-viewport/)

### MEDIA QUERIES
- Antes existiam as Media Types. As media types serviam para formatar a informação para outros tipos de media.
- Uma media muito usada é a print, que formata o layout para quando o site for impresso.
- O problema é que as media types não trabalham para vários tipos de dispositivos. O valor SCREEN é muito genérico.
- Daí surgiram as media queries. As media queries formatam o layout para vários tipos de tamanho de tela, densidade de pixels, orientação e etc.
- Em projetos Mobile First, você coloca a versão desktop dentro da media querei e a versão mobile fora dessa media querie.

Ref: [Introdução sobre Media Queries](http://tableless.com.br/introducao-sobre-media-queries/)

### IMAGENS FLUIDAS
- Não perca a cabeça com as imagens. Isto é, não fique louco tentando servir várias imagens para vários tipos de dispositivos.
- Não há solução decente hoje. Usar scripts ou plugins que façam um trabalho obscuro por trás é ruim.
- A tag picture é uma solução importante, mas ainda falta suporte e não pode ser usada.
- Em um site responsivo as imagens precisa ser flexíveis. O truque simples é:
img {
  max-width: 100%;
}

### GRIDS FLEXIVEIS
- Grids são facilitadores. Eles te ajudam a prever o comportamento do layout.
- Os grids podem ser totalmente flexíveis ou fluídos.
Mostrar exemplo de grid fluído e fixo
- Você pode usar frameworks para ajudar. Eu sugiro o grid do Bootstrap e em segundo lugar o Foundation.

### FONTS em REM
- Quando diminuimos a tela, precisamos diminuir as fonts. Usar fonts com tamanho relativo é prático.
- Use REM hoje em dia. Se tiver que dar suporte para o IE 8, use EM.
- A diferença de REM e EM é que o REM pega como referência o tamanho de font do root, nesse caso o HTML.
- A conta para fazer a conversão de PX para REM/EM é simples: valor da font em pixels, dividido por 16 = valor em REM.
- No HTML, recomenda-se usar 100% como font-size. Logo, no mobile você consegue diminuir para 90% 85% de maneira com que as fonts diminuam ou aumentem proporcionalmente.



