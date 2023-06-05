<template>
  <!-- FOOTER -->
  <footer>
    <div class="sobre_titulo">
      <h1>Ricardo Martins</h1>
      <p>Infelizmente ainda não tenho experiência no mercado profissional, porém esse é o principal objetivo, há momentos
        de desânimo, mas a persistência sempre esteve a frente!</p>
    </div>

    <nav aria-label="navegação para redes sociais">
      <ul class="footer_sociais">
        <li><i class="fa-brands fa-facebook-f"><a href="#"></a></i></li>
        <li><i class="fa-brands fa-twitter"><a href="#"></a></i></li>
        <li><i class="fa-brands fa-linkedin-in"><a href="#"></a></i></li>
        <li><i class="fa-brands fa-instagram"><a href="#"></a></i></li>
        <li><i class="fa-brands fa-github-alt"><a href="#"></a></i></li>
      </ul>
    </nav>

    <p class="footer_comercial">Todos os direitos reservados Ricardo Martins &copy; - 2023</p>
  </footer>
</template>

<script>

export default {
  name: 'Footer',

  setup() {
    return {

    }
  }
};
</script>

<style scoped>
/* FOOTER */
footer {
  background-color: #000;
  padding: 30px;
}

footer .sobre_titulo p {
  margin: 30px;
}

.footer_sociais {
  position: relative;
  display: flex;
  justify-content: center;
  gap: 30px;
  flex-wrap: wrap;
  align-items: center;
  color: #f7f7f7;
}

.footer_sociais li {
  background-color: #212020;
  border-radius: 50%;
  border: 1px solid #333;
}

.footer_sociais li i {
  padding: 30px;
  color: #f7f7f7;
}

.footer_sociais li:hover {
  transition: .3s ease-in-out;
  cursor: pointer;
  background-color: #3e3d3d;
}

.footer_sociais::before {
  position: absolute;
  content: '';
  width: 200px;
  height: 5px;
  bottom: -40px;
  background-color: #222;
}

footer .footer_comercial {
  text-align: center;
  color: #fff;
  margin: 90px auto;
  font-size: 1.5rem;
  font-family: 'Poppins', sans-serif;
}
</style>