<template>
  <!-- PRELOAD -->
  <div style="color: red">
    ? PRELOAD ?<br />
    - Vídeo: "vue js 3 portfolio template" (WebCodeCamp): 31:08<br />
    - Falta arrumar todo CSS scoped<br />
    - Falta arrumar todo Javascritp<br />
    - Colocar logo no menu<br />
    - Arrumar escrevendo/descrevendo e colocar apagando e escrevendo meu nome e depois a profissão<br />
    -<br />
  </div>

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

  <!-- Professional -->
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
    Portfolio,
    Professional,
    Services,
    Footer
  },

  setup() {
    return {

    }
  }
};

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Amatic+SC:wght@700&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Amatic+SC:wght@700&family=Berkshire+Swash&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

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
  background-color: #000;
  max-width: 1200px;
  margin: 0 auto;
}

/* CLASSES - TITLES */
.sobre_titulo {
  margin: 30px 0;
  grid-column: 1/-1;
  text-align: center;
  color: #fff;
}

.sobre_titulo h1 {
  font-size: 2.5rem;
  color: #ff5d56;
  font-family: 'Berkshire Swash', cursive;
}

.sobre_titulo p {
  color: #707070;
  font-size: 1.4rem;
  margin-bottom: 1rem;
  position: relative;
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
  background-color: #dc3545;
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
  .section-div img {
    display: none;
  }

  .section-div {
    background-image: url(../assets/me/mee3.jpeg);
    background-repeat: no-repeat;
    background-size: contain !important;
    background-position: center !important;
  }

  .section-div div p {
    text-shadow: 2px 2px 2px #000;
  }

  header {
    justify-content: space-between;
    padding: 30px 70px;
  }

  header .navegacao-primaria {
    display: none;
  }

  header i {
    color: #f7f7f7;
    font-size: 3rem;
  }

  header .navegacao-primaria.ativado {
    background: linear-gradient(rgba(13, 12, 12, 0.176), rgba(46, 46, 46, 0.724));
    position: absolute;
    display: grid;
    top: 80px;
    color: white;
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
  .sobre img {
    grid-column: 1/-1;
    justify-self: center;
  }

  .sobre_conteudo {
    grid-column: 1/-1;
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

  /* PROFESSIONAL - CURSOS */
  .cursos {
    grid-template-columns: 1fr;
  }

  .cursos .my_skill h2 {
    justify-self: center;
  }

  .cursos .my_skill {
    text-align: center;
    grid-template-columns: 1fr;
    justify-self: center;
    grid-column: 1/-1;
  }
}

@media(max-width: 1089px) {

  /* PORTFOLIO */
  .projects_storage ul {
    grid-template-columns: repeat(2, 1fr);
  }
}
</style>
