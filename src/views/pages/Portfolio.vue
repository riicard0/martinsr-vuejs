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

<style scoped></style>