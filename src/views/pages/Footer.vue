<template>
  <!-- FOOTER -->
  <footer>
    <div class="site-website">
      <div class="sobre_titulo">
        <h1>Ricardo Martins</h1>
        <p>Unfortunately, I still don't have any experience in the professional market, but that is the main goal. There
          are moments of discouragement, but persistence has always been at the forefront!</p>
      </div>

      <nav aria-label="navegação para redes sociais">
        <ul class="footer_sociais">
          <li><a href="https://www.linkedin.com/in/riicard0/" target="_blank"><i class="fa-brands fa-linkedin-in"></i></a>
          </li>
          <li><a href="https://www.instagram.com/ricarrdo_marttyns/" target="_blank"><i
                class="fa-brands fa-instagram"></i></a></li>
          <li><a href="https://github.com/riicard0" target="_blank"><i class="fa-brands fa-github-alt"></i></a></li>
        </ul>
      </nav>

      <p class="footer_comercial">All rights reserved Ricardo Martins &copy; - 2023</p>
    </div>
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
  background-color: var(--color-1);
  padding: 70px;
}

footer .sobre_titulo h1 {
  font-size: 3rem;
}

footer .sobre_titulo p {
  margin: 30px auto 30px auto;
  color: var(--color-2);
  font-family: var(--font-1);
  font-size: 1rem;
  max-width: 900px;
}

.footer_sociais {
  position: relative;
  display: flex;
  justify-content: center;
  gap: 30px;
  flex-wrap: wrap;
  align-items: center;
  color: var(--color-4);
}

.footer_sociais li {
  background-color: var(--color-8);
  border-radius: 50%;
  border: 1px solid var(--color-9);
}

.footer_sociais li i {
  padding: 30px;
  color: var(--color-4);
}

.footer_sociais li:hover {
  transition: .3s ease-in-out;
  cursor: pointer;
  background-color: var(--color-9);
}

.footer_sociais::before {
  position: absolute;
  content: '';
  width: 200px;
  height: 5px;
  bottom: -40px;
  background-color: var(--color-9);
}

footer .footer_comercial {
  text-align: center;
  color: var(--color-5);
  margin: 90px auto;
  font-size: 1.5rem;
  font-family: var(--font-5);
}
</style>