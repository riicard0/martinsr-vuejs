<template>
  <!-- MENU -->
  <header>
    <h1>Ricardo <span>Martins</span></h1>
    <nav>
      <ul aria-label="navegação primária" class="navegacao-primaria">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">Sobre</a></li>
        <li><a href="#services">Serviços</a></li>
        <li><a href="#portfolio">Portfólio</a></li>
        <li><a href="#professional">Experiência</a></li>
      </ul>
      <i class="fa-solid fa-bars"></i>
    </nav>
  </header>
</template>

<script>

export default {
  name: 'Navbar',

  setup() {
    return {

    }
  }
};
</script>

<style scoped></style>