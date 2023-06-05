<template>
  <!-- PROJECTS -->
  <section id="portfolio" class="projects">
    <div class="sobre_titulo">
      <h1>Portfólio</h1>
      <p>Projetos Profissionais - Aqui estão alguns projetos meus</p>
      <div aria-label="seção de botões">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>

    <div class="projects_models">
      <ul aria-label="navagação entre modelos de projetos">
        <li class="all">Tudo</li>
        <li class="design">Design</li>
        <li class="app_project">App</li>
        <li class="webSite">Website</li>
      </ul>
    </div>

    <div class="projects_storage">
      <ul aria-label="navegação de projetos">
        <li id="design"><a href="#" target="_blank"><img src="#" alt="wireframe criado barbearia"></a></li>
        <li id="design"><a href="#" target="_blank"><img src="#"
              alt="wireframe criado primeira versão desse portfólio"></a>
        </li>
        <li id="app_project"><a href="#" target="_blank"><img src="#" alt="site e app criado KiBeleza"></a></li>
        <li id="webSite"><a href="#" target="_blank"><img src="#" alt="Clone da Steam"></a></li>
        <li id="webSite"><a href="#" target="_blank"><img src="#" alt="site criado consumindo a API do Github"></a></li>
      </ul>
    </div>
    <a class="load_more" href="#">Mais Projetos</a>
  </section>
</template>

<script>

export default {
  name: 'Portfolio',

  setup() {
    return {

    }
  }
};
</script>

<style scoped>
/* PROJECTS */
.projects {
  padding: 30px;
  display: grid;
  justify-content: center;
  gap: 30x;
  background-color: #151515;
}

.projects ul {
  display: flex;
  justify-content: center;
  gap: 30px;
}

.projects_models ul li {
  cursor: pointer;
  font-family: 'Poppins', sans-serif;
  background-color: #222;
  border: 1px solid #333;
  margin-top: 20px;
  padding: 6px 20px;
  color: #707070;
  transition: .3s ease-in;
}

.projects_models ul li:hover {
  color: #fff;
  border: 1px solid #fff;
}

.projects_models ul li.active {
  background-color: #dc3545;
  color: #151515;
  font-weight: bold;
}

.projects_storage ul {
  display: grid;
  margin-top: 60px;
  gap: 20px;
  justify-content: center;
  grid-template-columns: repeat(4, 1fr);
}

.projects_storage ul li {
  display: none;
  max-width: 100%;
  height: 100%;
}

.projects_storage ul li.active {
  display: block;
  animation: animationImageButtom 2s ease-in-out forwards;
}

.projects_storage ul li img {
  max-width: 100%;
  height: 100%;
  border-radius: 4px;
  transition: .3s ease-in;
  border: 1px solid transparent;
}

.projects_storage ul li img:hover {
  border: 1px solid #fff;
}

.load_more {
  background-color: #222;
  text-decoration: none;
  justify-self: center;
  margin-top: 40px;
  padding: 20px 40px;
  border: 1px solid #333;
  color: #707070;
  transition: .3s ease-in;
}

.load_more:hover {
  color: #fff;
  border: 1px solid #fff;
}
</style>