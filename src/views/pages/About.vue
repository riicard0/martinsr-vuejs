<template>
  <!-- ABOUT -->
  <main id="about">
    <article aria-label="seção sobre mim" class="sobre">
      <div class="sobre_titulo">
        <h1>Sobre</h1>
        <p>Perfil Profissional - Sobre Mim</p>
        <div aria-label="seção apenas de ilustrações de botões">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
      <img src="../../assets/me/mee2.jpeg" alt="Minha imagem de perfil">
      <div class="sobre_conteudo">
        <div class="sobre_texto">
          <h1>Ricardo Martins</h1>
          <p>🇧🇷 Sou estudante e admirador da área de tecnologia, especificamente programação, há alguns anos. E há algum
            tempo venho em busca de uma oportunidade para embarcar de vez nessa jornada. Comecei estudando lógica de
            programação, com *Batch Script* e linguagem *C*, porém depois de um tempo resolvi seguir um "roadmap" focado
            em 'Front-End Developer' e venho nesse caminho até os dias atuais. 😁
            <br />
            <br />
            No final de 2022, estando com um conhecimento razoavelmente bom em *HTML*, *CSS* e *Javascript*, escolhi um
            framework para seguir como principal e resolvi focar totalmente em *Vue.js* e seu universo, claramente planejo
            continuar aprendendo outras stacks futuramente, mas estou buscando me dedicar e melhorar nessa tecnologia no
            momento. 👀
          </p>
        </div>
        <div class="sobre_info">
          <p><i class="fa-solid fa-calendar-days"></i>Birth: jan.1999</p>
          <p><i class="fa-sharp fa-solid fa-laptop-code"></i>Freelance: Available</p>
          <p><i class="fa-solid fa-location-dot"></i>Address: São Paulo, Brazil</p>
          <p><i class="fa-sharp fa-solid fa-globe"></i>Spoken Languages: Brazil, English</p>
          <p><i class="fa-solid fa-flag"></i>Nationality: Brazilian</p>
          <p><i class="fa-solid fa-envelope"></i>Email: ricarrd.omarttyns@gmail.com</p>
        </div>
      </div>
    </article>
  </main>
</template>

<script>

export default {
  name: 'About',

  setup() {

    return {}
  }
};
</script>

<style scoped></style>