<template>
  <!-- PRELOAD -->
  ? PRELOAD ?
  - Vídeo: "vue js 3 portfolio template" (WebCodeCamp): 31:08
  - Falta arrumar todo CSS scoped
  - Falta arrumar todo Javascritp
  - Colocar logo no menu
  - Arrumar escrevendo/descrevendo e colocar apagando e escrevendo meu nome e depois a profissão
  -

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

<style></style>
