# p-gina-web-html-css
@import url("styles/header.css");
@import url("styles/banner.css");
@import url("styles/carrossel.css");
@import url("styles/topicos.css");
@import url("styles/contato.css");
@import url("styles/rodapé.css");


:root {
    --cor-de-fundo: #EBECEE;
    --branco: #FFFFFF;
    --laranja: #EB9B00;
    --azul-degrade: linear-gradient(97.54deg, #002f52 35.49%, #326589 165.37%);
    --fonte-principal: "Poppins";
    --azul: #002F52;
    --fonte-secundario: "Josefin Sans";
    --preto: #000000;
    --cinza: #474646;
    --cinza-claro: #858585;
}

body {
    background-color: var(--cor-de-fundo);
    font-family: var(--fonte-principal);
    font-size: 16px;
    font-weight: 400;
}
/* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
*/

html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
}

/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
    display: block;
}

body {
    line-height: 1;
}

ol,
ul {
    list-style: none;
}

blockquote,
q {
    quotes: none;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
    content: '';
    content: none;
}

table {
    border-collapse: collapse;
    border-spacing: 0;
}
<!DOCTYPE html>
<html>

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AluraBooks</title>
  <link rel="stylesheet" href="reset.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css?family=Josefin+Sans:wght@400;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <header class="cabeçalho">
    <div class="container">
      <input type="checkbox" id="menu" class="container__botao">
      <label for="menu" class="container__rotulo">
        <span class="cabeçalho__menu-hamburguer container__imagem"></span>
      </label>
      <ul class="lista-menu">
        <li class="lista-menu__titulo">Categorias</li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Programação</a>
        </li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Front-end</a>
        </li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Infraestrutura</a>
        </li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Business</a>
        </li>
        <li class="lista-menu__item">
          <a href="#" class="lista-menu__link">Design & UX</a>
        </li>
      </ul>
      <img src="img/Logo.svg" alt="Logo da Alurabooks" class="container__imagem">
      <h1 class="container__titulo"><b class="container__titulo--negrito">Alura</b>Books</h1>

      <ul class="opções">
        <input type="checkbox" id="opções-menu" class="opções__botão" />
        <label for="opções-menu" class="opções__rotulo">
          <li class="opções__item">Categorias</li>
        </label>

        <ul class="lista-menu">
          <li class="lista-menu__item">
            <a href="#" class="lista-menu__link">Programação</a>
          </li>
          <li class="lista-menu__item">
            <a href="#" class="lista-menu__link">Front-end</a>
          </li>
          <li class="lista-menu__item">
            <a href="#" class="lista-menu__link">Infraestrutura</a>
          </li>
          <li class="lista-menu__item">
            <a href="#" class="lista-menu__link">Business</a>
          </li>
          <li class="lista-menu__item">
            <a href="#" class="lista-menu__link">Design & UX</a>
          </li>
        </ul>
        <li class="opções__item"><a href="#" class="opções__link">Favoritos</a></li>
        <li class="opções__item"><a href="#" class="opções__link">Minha estante</a></li>
      </ul>

    </div>
    <div class="container">
      <a href="#"><img src="img/Favoritos.svg" alt="Meus favoritos"
          class="container__imagem container__imagem-transparente"></a>
      <a href="#" class="container__link">
        <img src="img/Compras.svg" alt="Carrinhos de compras" class="container__imagem">
        <p class="container__texto">Minha sacola</p>
      </a>
      <a href="#" class="container__link">
        <img src="img/Usuario.svg" alt="Meu perfil" class="container__imagem">
        <p class="container__texto">Meu perfil</p>
      </a>
    </div>
  </header>

  <section class="banner">
    <h2 class="banner__titulo">Já sabe por onde começar?</h2>
    <p class="banner__texto">Encontre em nossa estante o que precisa para seu desenvolvimento!</p>
    <input type="search" class="banner__pesquisa" placeholder="Qual será sua próxima leitura?">
  </section>

  <section class="carrossel">
    <h2 class="carrossel__titulo">Novos lançamentos</h2>

    <div class="carrossel__container">
      <!-- Slider main container -->
      <div class="swiper">

        <div class="swiper-pagination"></div>
        <!-- Additional required wrapper -->
        <div class="swiper-wrapper">
          <!-- Slides -->
          <div class="swiper-slide"><img src="img/ApacheKafka.svg"
              alt="Livro sobre apache kafka e spring boot da alura books"></div>
          <div class="swiper-slide"><img src="img/Liderança.svg"
              alt="Livro sobre liderança em design design da alura books"></div>
          <div class="swiper-slide"><img src="img/Javascript.svg" alt="Livro sobre javascript assertivo da alura books">
          </div>
          <div class="swiper-slide">
            <img src="img/Guia Front-end.svg" alt="Livro Guia front end" />
          </div>
          <div class="swiper-slide">
            <img src="img/Portugol.svg" alt="Livro sobre portugol" />
          </div>
          <div class="swiper-slide">
            <img src="img/Acessibilidade.svg" alt="Livro sobre acessibilidade" />
          </div>
        </div>

        <!-- If we need navigation buttons -->
        <div class="swiper-button-prev"></div>
        <div class="swiper-button-next"></div>

      </div>

      <div class="card">
        <div class="card__descrição">
          <div class="descrição">
            <h3 class="descrição__titulo">Talvez você também se interesse por...</h3>
            <h2 class="descrição__titulo-livro">Angular 11 e Firebase</h2>
            <p class="descrição__texto">
              Construindo uma aplicação integrada com a plataforma do Google.
            </p>
          </div>
          <img src="img/Angular.svg" class="descrição__imagem" />
        </div>
        <div class="card__botões">
          <ul class="botões">
            <li class="botões__item">
              <img src="img/Favoritos.svg" alt="Favoritar livro" />
            </li>
            <li class="botões__item">
              <img src="img/Compras.svg" alt="Adicionar no carrinho de compras" />
            </li>
          </ul>
          <a href="#" class="botões__ancora">Saiba mais</a>
        </div>
      </div>
    </div>

  </section>

  <section class=”carrossel”>
    <h2 class="carrossel__titulo">Mais vendidos</h2>

    <div class="carrossel__container">
      <div class="swiper">
        <!-- Additional required wrapper -->
        <!-- If we need pagination -->
        <div class="swiper-pagination"></div>

        <div class="swiper-wrapper">
          <!-- Slides -->
          <div class="swiper-slide"><img src="img/ApacheKafka.svg"
              alt="Livro sobre apache kafka e spring boot da alura books"></div>
          <div class="swiper-slide"><img src="img/Liderança.svg" alt="Livro sobre liderança em design da alura books">
          </div>
          <div class="swiper-slide"><img src="img/Javascript.svg" alt="Livro sobre javascript assertivo da alurabooks">
          </div>
          <div class="swiper-slide"><img src="img/Guia Front-end.svg" alt="Livro Guia front end"></div>
          <div class="swiper-slide"><img src="img/Portugol.svg" alt="Livro sobre portugol"></div>
          <div class="swiper-slide"><img src="img/Acessibilidade.svg" alt="livro sobre acessibilidade"></div>
        </div>

        <!-- If we need navigation buttons -->
        <div class="swiper-button-prev"></div>
        <div class="swiper-button-next"></div>
      </div>

      <div class="card">
        <!-- 1º linha -->
        <div class="card__descrição">
          <!-- 1º coluna -->
          <div class="descrição">
            <img src="img/Estrelinhas.svg" alt="Avaliação 5 estrelas">
            <h3 class="descrição__titulo">Autora do Mês</h3>
            <h2 class="descrição__titulo-livro">Juliana Agarikov</h2>
            <p class="descrição__texto">Analista de sistemas e escritora, Juliana é especialista em
              Front-End.
            </p>
          </div>
          <!-- 2º coluna -->
          <img src="img/Escritora.svg" class="descrição__imagem">
        </div>

        <!-- 2º linha -->
        <div class="card__botões">
          <!-- 1º coluna -->
          <ul class="botões">
            <li class="botões__item"><img src="img/Favoritos.svg" alt="Favoritar livro"></li>
            <li class="botões__item"><img src="img/Compras.svg" alt="Adicionar no carrinho de compras"></li>
          </ul>
          <!-- 2º coluna -->
          <a href="#" class="botões__ancora">Saiba mais</a>
        </div>
      </div>
    </div>


  </section>

  <section class="tópicos">
    <h2 class="tópicos__titulo">TÓPICOS VISITADOS RECENTEMENTE</h2>
    <ul class="tópicos__lista">
      <li class="tópicos__item"><a href="#" class="tópicos__link">Android</a></li>
      <li class="tópicos__item">
        <a href="#" class="tópicos__link">Marketing Digital</a>
      </li>
      <li class="tópicos__item">
        <a href="#" class="tópicos__link">Agile</a>
      </li>
      <li class="tópicos__item">
        <a href="#" class="tópicos__link">Startups</a>
      </li>
      <li class="tópicos__item">
        <a href="#" class="tópicos__link">HTML & CSS</a>
      </li>
      <li class="tópicos__item">
        <a href="#" class="tópicos__link">Python</a>
      </li>
      <li class="tópicos__item">
        <a href="#" class="tópicos__link">OO</a>
      </li>
      <li class="tópicos__item">
        <a href="#" class="tópicos__link">Java</a>
      </li>
    </ul>
  </section>

  <section class="contato">
    <div class="contato__descrição">
      <h2 class="contato__titulo">Fique por dentro das novidades!</h2>
      <p class="contato__texto">
        Atualizações de e-books, novos livros, promoções e outros.
      </p>
    </div>
    <input type="email" placeholder="        Cadastre seu e-mail" class="contato__email">
  </section>

  <hr />

  <footer class="rodapé">
    <h2 class="rodapé__titulo">Grupo Alura</h2>
    <ul class="lista-rodapé">
      <li class="lista-rodapé__titulo">Educação</li>
      <li class="lista-rodapé__item">
        <img src="img/Caelum.svg" alt="Logo da Caelum" />
        <a href="#" class="lista-rodapé__link">Caelum</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/CasaDoCodigo.svg" alt="Logo da Casa do Código" />
        <a href="#" class="lista-rodapé__link">Casa do Código</a>
      </li>
    </ul>

    <ul class="lista-rodapé">
      <li class="lista-rodapé__titulo">Educação online</li>
      <li class="lista-rodapé__item">
        <img src="img/Alura.svg" alt="Logo da Alura" />
        <a href="#" class="lista-rodapé__link">Alura</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraEmpresas.svg" alt="Logo da AluraParaEmpresas" />
        <a href="#" class="lista-rodapé__link">Alura para Empresas</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraLATAM.svg" alt="Logo da Alura Latam" />
        <a href="#" class="lista-rodapé__link">Alura LATAM</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraStart.svg" alt="Logo da Alura START" />
        <a href="#" class="lista-rodapé__link">Alura Start</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/MusicDot.svg" alt="Logo da Music Dot" />
        <a href="#" class="lista-rodapé__link">Music Dot</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraLingua.svg" alt="Logo da Alura Lingua" />
        <a href="#" class="lista-rodapé__link">Alura Língua</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/PM3.svg" alt="Logo da PM3" />
        <a href="#" class="lista-rodapé__link">PM3</a>
      </li>
    </ul>

    <ul class="lista-rodapé">
      <li class="lista-rodapé__titulo">Comunidade</li>
      <li class="lista-rodapé__item">
        <img src="img/HipstersTech.svg" alt="Logo do Hipsters ponto Tech" />
        <a href="#" class="lista-rodapé__link">Hipsters ponto Tech</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/ScubaDev.svg" alt="Logo do Scuba Dev" />
        <a href="#" class="lista-rodapé__link">Scuba Dev</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/LayersTech.svg" alt="Logo do Layers ponto Tech" />
        <a href="#" class="lista-rodapé__link">Layers ponto Tech</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/LikeABoss.svg" alt="Logo do Like a Boss" />
        <a href="#" class="lista-rodapé__link">Like a Boss</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/CarreiraSemFronteira.svg" alt="Logo do Carreira sem fronteiras" />
        <a href="#" class="lista-rodapé__link">Carreira sem fronteiras</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/HipstersJobs.svg" alt="Logo do Hipsters ponto jobs" />
        <a href="#" class="lista-rodapé__link">Hipsters ponto jobs</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/GUJ.svg" alt="Logo do GUJ" />
        <a href="#" class="lista-rodapé__link">GUJ</a>
      </li>
    </ul>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
  <script>
    const swiper = new Swiper(".swiper", {
      spaceBetween: 10,
      slidesPerView: 3,
      pagination: {
        el: '.swiper-pagination',
        type: 'bullets',
      },
    });
  </script>
</body>

</html>
.banner {
    background: var(--azul-degrade);
    color: var(--branco);
    text-align: center;
    padding: 2.5em 2em;
}

.banner__titulo {
    font-size: 18px;
    font-weight: 700;
}

.banner__texto {
    font-weight: 500;
    margin: 1em 0;
}

.banner__pesquisa {
    background-color: transparent;
    border: 1px solid var(--branco);
    color: var(--branco);
    border-radius: 24px;
    padding: 1em;
    width: 100%;
}

.banner__pesquisa::placeholder {
    font-family: var(--fonte-principal);
    font-size: 14px;
    font-weight: 400;
    text-align: center;
    color: var(--branco);
    background: url("../img/Lupa.svg") no-repeat;
    background-position: 1em;
}

@media screen and (min-width: 1024px) {
    .banner__titulo {
        font-size: 36px;
    }

    .banner__pesquisa {
        width: 50%;
    }

    .banner__pesquisa::placeholder {
        background-position: 7em;
    }
}



@media screen and (min-width: 1728px) {
    .banner__pesquisa {
        width: 35%;
    }

    .banner {
        padding: 6em 0;
    }

    .banner__pesquisa::placeholder {
        background-position: 12em;
    }


}
.carrossel__titulo {
    color: var(--laranja);
    background-color: var(--branco);
    text-align: center;
    text-transform: uppercase;
    font-size: 18px;
    font-weight: 700;
    padding: 1em 0 0.5em 0;
}

.swiper-slide img {
    width: 100%;
}

.swiper-button-prev,
.swiper-button-next {
    display: none;
}

.swiper-pagination {
    position: initial;
    margin: .5em 0;
}

.card__descrição {
    display: flex;
    justify-content: space-between;
    margin-bottom: 0.5em;
}

.card__botões {
    display: flex;
    justify-content: space-between;
}

.botões {
    display: flex;
}

.card {
    background: var(--branco);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    border-radius: 10px;
    margin: 1em;
    padding: 1em;
}

.descrição__titulo {
    color: var(--laranja);
    font-weight: 700;
}

.descrição__titulo-livro {
    color: var(--azul);
    font-size: 18px;
    font-weight: 700;
    margin: 0.5em 0;
}

.descrição__texto {
    font-size: 14px;
}

.botões__item {
    margin: 0 0.5em;
}

.botões__ancora {
    background-color: var(--laranja);
    padding: 1em 2.2em;
    color: var(--branco);
    font-weight: 700;
    text-decoration: none;
}

@media screen and (min-width: 1024px) {
    .carrossel__titulo {
        font-size: 26px;
    }

    .swiper-pagination {
        margin: 2em 0 3em 0;
    }

    .swiper {
        width: 60%;
    }

    .swiper-button-prev,
    .swiper-button-next {
        display: block;
        top: 60%;
    }
}

@media screen and (min-width: 1728px) {
    .carrossel__container {
        display: flex;
        margin: 0 20vw 3em 20vw;
    }

    .swiper-pagination {
        margin: 1em 0;
    }

    .swiper {
        width: 50%;
    }

    .descrição__titulo {
        font-size: 32px;
    }

    .descrição__texto {
        font-size: 16px;
    }

    .card {
        width: 60%;
        margin-left: 3em;
    }

}
.contato {
    background-color: var(--branco);
    padding: 1em;
}

.contato__titulo,
.contato__texto {
    background: var(--azul-degrade);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.contato__titulo {
    font-size: 18px;
    font-weight: 500;
}

.contato__texto {
    font-weight: 300;
    margin: 1em 0;
}

.contato__email {
    padding: 1em;
    border: 1px solid var(--azul);
    border-radius: 24px;
    width: 90%;
    color: var(--azul);
}

.contato__email::placeholder {
    font-family: var(--fonte-principal);
    color: var(--azul);
    background: url("../img/Email.svg") no-repeat 5%;
    padding-left: 2em;
}

@media screen and (min-width: 1024px) {
    .contato {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .contato__titulo {
        font-size: 24px;
    }

    .contato__descrição {
        margin-right: 1em;
        width: 30%;
    }

    .contato__email {
        width: 30%;
    }
}

@media screen and (min-width: 1728px) {
    .contato {
        padding: 3em 20vw;
    }
}
.cabeçalho__menu-hamburguer {
    width: 24px;
    height: 24px;
    display: inline-block;
    background-image: url("../img/Menu.svg");
    background-repeat: no-repeat;
    background-position: center;
}

.container__botao:checked~.container__rotulo>.cabeçalho__menu-hamburguer {
    background-image: url("../img/MenuAberto.svg");
}

.container__botao:checked~.container__rotulo {
    background: var(--azul-degrade);
}

.cabeçalho {
    background-color: var(--branco);
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
}

.container {
    display: flex;
    align-items: center;
}

.container__imagem {
    padding: 1em;
}


.lista-menu {
    display: none;
    position: absolute;
    top: 100%;
    width: 60vw;
}

.container__botao:checked~.lista-menu {
    display: block;
}

.lista-menu__titulo,
.lista-menu__item {
    padding: 1em;
    background-color: var(--branco);
}

.lista-menu__titulo {
    color: var(--laranja);
    font-weight: 700;
}

.lista-menu__link {
    background: var(--azul-degrade);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-transform: uppercase;
}

.container__botao {
    display: none;
}

.container__titulo {
    display: none;
}

.container__texto {
    display: none;
}

.opções {
    display: none
}

@media screen and (min-width: 1024px) {

    .container__titulo,
    .container__titulo--negrito {
        font-family: var(--fonte-secundario);
        font-size: 30px;
    }

    .container__titulo {
        font-weight: 400;
        display: block;
    }

    .container__titulo--negrito {
        font-weight: 700;
    }

    .opções {
        display: flex;
    }

    .opções__item {
        padding: 0 1em;
        text-transform: uppercase;
    }

    .opções__link {
        text-decoration: none;
        color: var(--preto);
    }

    .container__imagem-transparente {
        display: none;
    }

    .cabeçalho__menu-hamburguer {
        display: none;
    }

    .opções__botão:checked~.lista-menu {
        display: block;
        width: auto;
    }

    .opções__botão {
        display: none;
    }

    .opções__botão:checked~.opções__rotulo>.opções__item {
        background: var(--azul-degrade);
        color: var(--branco);
    }

    .opções__item {
        padding: 2em 1em;
    }

    .lista-menu__item:hover {
        background: var(--azul-degrade);
    }

    .lista-menu__item:hover>.lista-menu__link {
        -webkit-text-fill-color: var(--branco);
        text-decoration: none;
    }

}

@media screen and (min-width: 1728px) {
    .container__link {
        display: flex;
        align-items: center;
        text-decoration: none;
        color: var(--preto);
        padding-right: 30px;
    }

    .opções {
        margin-right: auto;
    }

    .container__texto {
        display: block;
    }

}
hr {
    margin: 0;
}

.rodapé {
    background-color: var(--branco);
    padding: 1em;
}

.lista-rodapé {
    display: none;
}


@media screen and (min-width: 1024px) {
    .rodapé {
        display: flex;
        justify-content: space-around;
    }

    .lista-rodapé {
        display: block;
    }

    .lista-rodapé__item {
        display: flex;
        align-items: center;
        margin: 0.6em 0;
    }

    .lista-rodapé__link {
        color: var(--cinza);
        text-decoration: none;
        margin-left: 0.6em;
    }

    .lista-rodapé__titulo {
        font-size: 14px;
        color: var(--cinza-claro);
    }

    .rodapé__titulo {
        font-size: 24px;
    }
}

@media screen and (min-width: 1728px) {
    .lista-rodapé {
        border-left: 1px solid var(--cinza-claro);
        padding-left: 1em;
    }
}
.tópicos {
    background: var(--azul-degrade);
    text-align: center;
    padding: 1em 0;
}

.tópicos__titulo {
    color: var(--branco);
    font-weight: 300;
    margin-bottom: 1em;
}

.tópicos__lista {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.tópicos__item {
    margin: 2em 0.5em;
}

.tópicos__link {
    color: var(--branco);
    padding: 1em;
    background-color: var(--laranja);
    text-decoration: none;
    font-size: 14px;
    font-weight: 700;
}

@media screen and (min-width: 1024px) {
    .tópicos__titulo {
        font-size: 24px;
    }

    .tópicos__link {
        font-size: 24px;
    }
}


@media screen and (min-width: 1728px) {
    .tópicos {
        padding: 3em 30vw;
    }
}
