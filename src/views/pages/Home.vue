<template>
  <!-- HOME | HERO -->
  <section id="home" aria-label="seção home" class="section-div">
    <div>
      <h2>Howdy. I'm</h2>
      <h2 class="digitando">Front-End Developer ▪︎ Vue.js | Javascript</h2>
      <p>In the middle of 2021, I decided to focus on Front-End and I have been improving. My goal is to embrace the
        challenge and the knowledge that will come from this field.</p>
      <a href="#about">About Me</a>
    </div>

    <!-- <img src="../../assets/me/mee3.jpeg" alt="Minha imagem de perfil"> -->
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
  background-color: #292929;
  display: grid;
  grid-template-columns: 1fr 1fr;
  justify-content: space-around;
  align-items: center;
  gap: 60px;
  padding: 60px;
  height: 93vh;
  background-image: url(../../assets/me/mee3.jpeg);
  background-repeat: no-repeat;
  background-size: 55%;
  background-position: 90%;
}

.section-div div {
  margin-top: 120px;
  align-self: start;
  display: grid;
  gap: 30px;
}

.section-div div h2:first-child {
  font-family: 'Poppins';
  font-weight: 600;
  color: #f7f7f7;
}

.section-div div h2:nth-child(2) {
  font-family: 'Poppins';
  font-weight: 600;
  color: #B4DF9F;
  text-shadow: 2px 2px 2px #000;
}

.section-div div p {
  font-family: 'Poppins';
  font-weight: 200;
  color: #f7f7f7;
}

.section-div div a {
  justify-self: start;
  padding: 15px 40px;
  border-radius: 5px;
  border: 2px solid white;
  transition: .3s ease-in;
  background-color: #000;
  color: #fff;
  border: 2px solid transparent;
}

.section-div div a:hover {
  background-color: #fff;
  color: #000;
  border: 2px solid transparent;
}

/*.section-div img {
  max-width: 100%;
}*/

.digitando::after {
  content: '|';
  margin-left: 5px;
  opacity: 1;
  animation: pisca .5s infinite;
}
</style>