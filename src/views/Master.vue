<template>
  <!-- PRELOAD -->
  <!-- <div style="color: red">
    - ? PRELOAD ?<br />
    - Falta arrumar todo CSS scoped<br />
    - Falta arrumar todo Javascript (converter para Vue)<br />
    - Colocar logo no "navbar.vue"<br />
    - Arrumar escrevendo/descrevendo e colocar apagando e escrevendo meu nome e depois a profissão<br />
    - Organizar tamanho (responsividade) para meu monitor (monitores grandes)<br />
    - Lembrar de verificar ao final se o site todo está em inglês<br />
    - Verificar se todas as variáveis das páginas estão nos lugares das fontes e cores <br />
    - Caso queira, criar outra página (components), junto do "vue-router", para o ".load.more" na área "portfolio" do
    website, indo para uma página que irá consumir uma API em Javascript dos meus projetos no Github.<br />
    - Colocar cards dos projetos em ".projects_storage" que nem no "Portfolio João Carlos Lima e Silva"<br />
    - Revisar Javascript na "page": "Professional.vue", os botões não estão funcionando.<br />
    - Revisar Javascript na "page": "Portfolio.vue", os botões não estão funcionando. E aplicar um click na imagem e
    aparecer o layout inteiro.<br />
    -
  </div> -->

  <!-- Navegation Bar -->
  <Navbar></Navbar>

  <!-- Home | Hero -->
  <Home></Home>

  <!-- About -->
  <About></About>

  <!-- Services -->
  <Services></Services>

  <!-- Portfolio -->
  <Portfolio></Portfolio>

  <!-- Experience -->
  <Professional></Professional>

  <!-- Footer -->
  <Footer></Footer>
</template>

<script>
import Navbar from '@/views/pages/Navbar.vue'
import Home from '@/views/pages/Home.vue'
import About from '@/views/pages/About.vue'
import Services from '@/views/pages/Services.vue'
import Portfolio from '@/views/pages/Portfolio.vue'
import Professional from '@/views/pages/Professional.vue'
import Footer from '@/views/pages/Footer.vue'

export default {
  app: '',

  components: {
    Navbar,
    Home,
    About,
    Services,
    Portfolio,
    Professional,
    Footer
  },

  setup() {
    return {

    }
  }
};

</script>

<style>
/* FONTS */
@import url('https://fonts.googleapis.com/css2?family=Amatic+SC:wght@700&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Amatic+SC:wght@700&family=Berkshire+Swash&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Baloo+Da+2:wght@400;500;600;700&family=Josefin+Slab:ital,wght@0,300;0,400;0,600;0,700;1,300;1,400;1,600&family=Mulish:ital,wght@0,200;0,300;0,400;0,500;1,200;1,300;1,400&display=swap');

/* ALL WEBSITE */
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  list-style: none;
  text-decoration: none;
}

html {
  scroll-behavior: smooth;
}

body {
  background-color: var(--color-6);
  margin: 0 auto;
}

/* VARIÁVEIS */
:root {
  --font-1: "Poppins", serif;
  --font-2: "Berkshire Swash", cursive;
  --font-3: "Baloo Da 2", serif;
  --font-4: "Josefin Slab", serif;
  --font-5: "Mulish", serif;

  --color-1: #000;
  --color-2: #fff;
  --color-3: #707070;
  --color-4: #f7f7f7;
  --color-5: #B4DF9F;
  --color-6: #0f121b;
  --color-7: #111;
  --color-8: #151515;
  --color-9: #222;

  --color-gradient-1a: rgba(13, 12, 12, 0.176);
  --color-gradient-1b: rgba(46, 46, 46, 0.724);
}

/* CLASSES - SIZE WEBSITE */
.site-website {
  max-width: 1200px;
  margin: 0 auto;
}

/* CLASSES - TITLES */
.sobre_titulo {
  margin: 0;
  grid-column: 1/-1;
  text-align: center;
  color: var(--color-2);
}

.sobre_titulo h1 {
  font-size: 2.5rem;
  color: var(--color-5);
  font-family: var(--font-2);
}

.sobre_titulo p {
  color: var(--color-3);
  font-size: 1.4rem;
  margin: 1rem;
  position: relative;
  font-family: var(--font-4);
}

.sobre_titulo div {
  display: flex;
  gap: 10px;
  justify-content: center;
}

.sobre_titulo span {
  display: block;
  height: 20px;
  width: 20px;
  border-radius: 50%;
  background-color: var(--color-5);
}

/* KEYFRAMES - HOME*/
@keyframes pisca {
  from {
    opacity: 1;
  }

  to {
    opacity: 0;
  }
}

@keyframes inicializar {
  from {
    opacity: 0;
    transform: translate3d(0, -60px, 0);
  }

  to {
    opacity: 1;
    transform: translate3d(0, 0, 0);
  }
}

/* KEYFRAMES - SOBRE */
@keyframes sobeSecao {
  from {
    transition: .5s;
    transform: translate3d(60px, 0, 0);
  }

  to {
    transform: translate3d(0, 0, 0);
  }
}

@keyframes ladoSecao {
  from {
    transition: .5s;
    transform: translate3d(-60px, 0, 0);
  }

  to {
    transform: translate3d(0, 0, 0);
  }
}

/* KEYFRAMES - PORTFOLIO */
@keyframes animationImageButtom {
  0% {
    opacity: 0;
    transform: translate3d(0, -30px, 0);
  }

  100% {
    opacity: 1;
    transform: translate3d(0, 0, 0);
  }
}

/* RESPONSIVE */
@media(max-width: 992px) {

  /* HEADER | HOME */

  .section-div {
    background-image: url(../assets/me/mee2.png);
    background-repeat: no-repeat;
    background-size: 70vh !important;
    background-position: right !important;
  }

  .section-div div p {
    text-shadow: 2px 2px 2px var(--color-1);
  }

  header {
    justify-content: space-between;
    padding: 30px 70px;
  }

  header .navegacao-primaria {
    display: none !important;
  }

  header i {
    color: var(--color-4);
    font-size: 3rem;
    display: block !important;
  }

  header .navegacao-primaria.ativado {
    background: linear-gradient(var(--color-gradient-1a), var(--color-gradient-1b));
    position: absolute;
    display: grid;
    top: 80px;
    color: var(--color-2);
    z-index: 1;
    padding: 30px;
    font-size: 1.6rem;
    font-weight: bold;
    border-radius: 0 0 4px 4px;
    right: 20px;
    animation: sobeSecao .8s ease-in-out forwards;
  }
}

@media(max-width: 992px) {

  /* SOBRE */
  main {
    height: 100% !important;
  }

  main .sobre::after {
    margin: 2rem auto -1rem auto !important;
  }

  .sobre img {
    grid-column: 1/-1;
    justify-self: center;
  }

  .sobre_conteudo {
    grid-column: 1/-1 !important;
  }

  /* SERVICES */
  .services {
    height: 100% !important;
  }

  .services::after {
    margin: 0 auto -1rem auto !important;
  }

  .projects {
    height: 100% !important;
  }

  .projects::after {
    margin: 2% auto -5rem auto !important;
  }
}

@media(max-width: 1089px) {

  /* PROFESSIONAL - EXPERIENCE/EDUCATION */
  .resume_generico .experience_content,
  .education_content {
    justify-self: center;
    grid-column: 1/-1;
  }

  .resume_generico .education {
    grid-column: 1/-1;
    grid-row: 3;
    justify-self: center;
    margin: 30px 0;
  }

  .resume_generico .experience {
    grid-column: 1/-1;
    grid-row: 1;
    justify-self: center;
  }
}

@media(max-width: 1089px) {

  /* PORTFOLIO */
  .projects_storage ul {
    grid-template-columns: repeat(2, 1fr) !important;
  }
}
</style>
