<template>
  <!-- ABOUT -->
  <main id="about">
    <article aria-label="seção sobre mim" class="sobre site-website">
      <div class="sobre_titulo">
        <h1>About</h1>
        <p>Professional Profile - About Me</p>
        <div aria-label="seção apenas de ilustrações de botões">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
      <img src="../../assets/me/mee.jpeg" alt="Minha imagem de perfil">
      <div class="sobre_conteudo">
        <div class="sobre_texto">
          <h1>I'm Ricardo Martins</h1>
          <p>I am a student and an admirer of the technology field, specifically programming, for a few years now. And for
            some time, I have been searching for an opportunity to fully embark on this journey. I started by studying
            programming logic, with Batch Script and the C language, but after a while, I decided to follow a roadmap
            focused on becoming a Front-End Developer, and I have been on this path to this day.
            <br />
            <br />
            At the end of 2022, having a reasonably good knowledge of HTML, CSS, and Javascript, I chose a framework to
            pursue as my main focus and decided to fully concentrate on Vue.js and its ecosystem. I clearly plan to
            continue learning other stacks in the future, but I am currently seeking to dedicate myself and improve in
            this technology. 👀
          </p>
        </div>
        <div class="sobre_info">
          <p><i class="fa-solid fa-calendar-days"></i>Birth: <span>jan.1999</span></p>
          <p><i class="fa-sharp fa-solid fa-laptop-code"></i>Freelance: <span>Available</span></p>
          <p><i class="fa-solid fa-location-dot"></i>Address: <span>São Paulo, Brazil</span></p>
          <p><i class="fa-sharp fa-solid fa-globe"></i>Spoken Languages: <span>Brazil (Fluent), English (A2-B1)</span></p>
          <p><i class="fa-solid fa-flag"></i>Nationality: <span>Brazilian</span></p>
          <p><i class="fa-solid fa-envelope"></i>Email: <span>ricarrd.omarttyns@gmail.com</span></p>
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
  background-color: var(--color-7);
  color: var(--color-2);
  height: 100vh;
}

main .sobre {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 30px;
  justify-content: center;
  padding: 40px;
}

main .sobre::after {
  content: '';
  display: block;
  background-color: var(--color-2);
  width: 300px;
  height: 6px;
  border-radius: 5px;
  grid-column: 1/-1;
  grid-row: 6;
  margin: 0 auto;
}

.sobre img {
  animation: ladoSecao .5s ease-in-out forwards;
  cursor: pointer;
  grid-row: 2;
  max-width: 100%;
  border-radius: 5px;
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
  color: var(--color-3);
  grid-template-columns: 1fr 1fr;
}

.sobre_texto {
  display: grid;
  grid-column: 1/-1;
  grid-template-columns: 1fr 1fr;
}

.sobre_texto h1 {
  font-family: var(--font-5);
  font-size: 2.3rem;
  color: var(--color-2);
  grid-column: 1/-1;
}

.sobre_texto h1::after {
  background-color: var(--color-5);
  height: 6px;
  width: 100px;
  margin: 20px 0;
  content: '';
  display: block;
  border-radius: 5px;
}

.sobre_texto p {
  font-family: var(--font-1);
  color: var(--color-3);
  font-size: 1.1rem;
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
  color: var(--color-5);
  display: inline-block;
  padding-right: 15px;
  font-size: 1.5rem;
}

.sobre_info p {
  font-family: var(--font-3);
  font-size: 1.2rem;
  color: var(--color-3);
}

.sobre_info span {
  color: var(--color-4);
}
</style>