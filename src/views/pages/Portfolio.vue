<template>
  <!-- PROJECTS -->
  <section id="portfolio" class="projects">
    <div class="sobre_titulo">
      <h1>Portfolio</h1>
      <p>Professional Projects - Here are some of my projects.</p>
      <div aria-label="seção de botões">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>

    <div class="projects_models site-website">
      <ul aria-label="navagação entre modelos de projetos">
        <li class="all">All</li>
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
    <div class="load-button">
      <a class="load_more" href="https://github.com/riicard0?tab=repositories" target="_blank">Load More</a>
    </div>
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
  display: grid;
  justify-content: center;
  gap: 30px;
  padding: 40px;
  height: 100%;
  background-color: var(--color-2);
}

.projects ul {
  display: flex;
  justify-content: center;
  gap: 30px;
}

.projects_models ul li {
  cursor: pointer;
  font-family: var(--font-3);
  background-color: var(--color-9);
  border: 1px solid var(--color-6);
  padding: 6px 20px;
  color: var(--color-3);
  transition: .3s ease-in;
}

.projects_models ul li:hover {
  color: var(--color-2);
  border: 1px solid var(--color-2);
}

.projects_models ul li.active {
  background-color: var(--color-5);
  color: var(--color-8);
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
  border: 1px solid var(--color-2);
}

.load-button {
  display: flex;
  justify-content: center;
  align-items: center;
}

.load_more {
  background-color: var(--color-9);
  justify-self: center;
  align-items: center;
  color: var(--color-3);
  padding: 20px 40px;
  font-family: var(--font-3);
  border: 1px solid var(--color-6);
  text-decoration: none;
  transition: .3s ease-in;
}

.load_more:hover {
  color: var(--color-2);
  border: 1px solid var(--color-2);
}
</style>