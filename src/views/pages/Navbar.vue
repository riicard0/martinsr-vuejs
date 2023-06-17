<template>
  <!-- MENU -->
  <header class="site-website">
    <h1>Ricardo <span>Martins</span></h1>
    <nav>
      <ul aria-label="navegação primária" class="navegacao-primaria">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#portfolio">Portfolio</a></li>
        <li><a href="#professional">Experience</a></li>
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
  background-color: var(--color-6);
  padding: 30px 70px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

header h1 {
  color: var(--color-2);
  font-size: 2rem;
}

header span {
  color: var(--color-5);
}

header nav {
  display: flex;
  justify-content: center;
}

header nav i {
  display: none;
}

header .navegacao-primaria {
  display: flex;
  gap: 30px;
  align-items: center;
}

header .navegacao-primaria li a {
  color: var(--color-2);
  width: 0px;
  height: 0px;
  font-family: var(--font-1);
  font-size: 1.1rem;
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
  border-bottom: 4px solid var(--color-5);
}
</style>