<template>
  <!-- HOME | HERO -->
  <section id="home" aria-label="seção home" class="section-div site-website">
    <div>
      <h2>Howdy. I'm</h2>
      <h2 class="digitando">Front-End Developer ▪︎ Vue.js | Javascript</h2>
      <p>In the middle of 2021, I decided to focus on Front-End and I have been improving. My goal is to embrace the
        challenge and the knowledge that will come from this field.</p>
      <a href="#about">About Me</a>
    </div>
  </section>
</template>

<script>

export default {
  name: 'home',

  setup() {
    return {

    }
  }
};
</script>

<style scoped>
/* DOWNLOAD CV SEÇÃO */
.section-div {
  animation: inicializar .7s forwards;
  background-color: var(--color-6);
  display: grid;
  grid-template-columns: 1fr 1fr;
  justify-content: space-around;
  align-items: center;
  gap: 60px;
  padding: 60px;
  height: 94vh;
  background-image: url(../../assets/me/mee2.png);
  background-repeat: no-repeat;
  background-size: 70vh;
  background-position: right;
}

.section-div div {
  margin-top: 120px;
  align-self: start;
  display: grid;
  gap: 30px;
}

.section-div div h2:first-child {
  font-family: var(--font-1);
  font-weight: 600;
  color: var(--color-4);
}

.section-div div h2:nth-child(2) {
  font-family: var(--font-1);
  font-weight: 600;
  color: var(--color-5);
  text-shadow: 2px 2px 2px var(--color-1);
}

.section-div div p {
  font-family: var(--font-1);
  font-weight: 200;
  color: var(--color-4);
}

.section-div div a {
  justify-self: start;
  padding: 15px 40px;
  border-radius: 30px;
  transition: .3s ease-in;
  background-color: var(--color-2);
  color: var(--color-1);
  border: 1px solid transparent;
}

.section-div div a:hover {
  background-color: var(--color-1);
  color: var(--color-2);
  border: 1px solid transparent;
  border-radius: 5px;
}

.digitando::after {
  content: '|';
  margin-left: 5px;
  opacity: 1;
  animation: pisca .5s infinite;
}
</style>