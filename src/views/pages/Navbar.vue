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

<style scoped>
/* HEADER */
header {
  background-color: #000;
  padding: 10px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

header h1 {
  color: #fff;
  font-size: 2.5rem;
}

header span {
  color: #B4DF9F;
}

header nav {
  display: flex;
  justify-content: center;
}

header .navegacao-primaria {
  display: flex;
  gap: 30px;
  align-items: center;
}

header .navegacao-primaria li a {
  color: #fff;
  width: 0px;
  height: 0px;
  font-size: 1.3rem;
}

header .navegacao-primaria li a::after {
  content: '';
  width: 0px;
  height: 0px;
  display: block;
  border-bottom: 4px solid transparent;
  transition: .9s;
}

header .navegacao-primaria li a:hover::after {
  width: 100%;
  height: 0px;
  padding: 0px;
  border-bottom: 4px solid #B4DF9F;
}
</style>