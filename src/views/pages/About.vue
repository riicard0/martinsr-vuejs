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
      <img src="../../assets/me/mee3.jpeg" alt="Minha imagem de perfil">
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

<style scoped>
/* SEÇÃO PRINCIPAL SOBRE MIM */
main {
  background-color: #111;
  color: white;
}

main .sobre {
  /* margin-top: 60px; */
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 30px;
  justify-content: center;
  padding: 40px;
}

.sobre img {
  animation: ladoSecao .5s ease-in-out forwards;
  cursor: pointer;
  grid-row: 2;
  max-width: 100%;
  border-radius: 4px;
  filter: blur(0);
}

.sobre img:hover {
  transition: .5s ease-in;
  filter: blur(1px);
}

.sobre_conteudo {
  animation: sobeSecao .6s ease-in-out forwards;
  grid-column: 2/-1;
  display: grid;
  color: #707070;
  grid-template-columns: 1fr 1fr;
}

.sobre_texto {
  display: grid;
  grid-column: 1/-1;
  grid-template-columns: 1fr 1fr;
}

.sobre_texto h1 {
  font-size: 2.3rem;
  color: #fff;
  grid-column: 1/-1;
}

.sobre_texto h1::after {
  background-color: #ff5d56;
  height: 6px;
  width: 60px;
  margin: 20px 0;
  content: '';
  display: block;
  border-radius: 5px;
}

.sobre_texto p {
  font-size: 1.3rem;
  grid-row: 2;
  grid-column: 1/-1;
}

.sobre_info {
  margin: 30px 0 30px 0;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-column: 1/-1;
  gap: 15px;
  align-items: center;
}

.sobre_info i {
  color: #dc3545;
  display: inline-block;
  padding-right: 15px;
  font-size: 1.5rem;
}

.sobre_info p {
  font-size: .9rem;
}
</style>