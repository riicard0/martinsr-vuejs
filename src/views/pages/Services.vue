<template>
  <!-- SERVICES -->
  <section id="services" class="services">
    <div class="sobre_titulo">
      <h1>Serviços</h1>
      <p>Conhecimentos abrangentes sobre a área</p>
      <div aria-label="seção com botões sobre os conhecimentos Front-End">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>

    <div class="my_services">
      <ul aria-label="navegação secundária">
        <li>
          <i class="fa-sharp fa-solid fa-pen-to-square"></i>
          <h3>Web Design</h3>
          <p>Web design é o processo de planejar, criar e organizar elementos visuais e estruturais em um site para
            proporcionar uma experiência agradável e eficiente aos usuários. Envolve a seleção de cores, tipografia,
            layout e disposição de elementos para comunicar efetivamente a mensagem do site e facilitar a navegação.</p>
        </li>
        <li>
          <i class="fa-solid fa-globe"></i>
          <h3>Web Developer</h3>
          <p>Um web developer é um profissional que cria e desenvolve aplicativos e sites para a web. Eles trabalham com
            diferentes tecnologias de programação, como HTML, CSS e JavaScript, para construir a funcionalidade e a
            interatividade dos sites. Seu trabalho envolve escrever código, solucionar problemas e garantir que os sites
            sejam responsivos, seguros e otimizados para uma experiência de usuário eficiente.</p>
        </li>
        <li>
          <i class="fa-solid fa-camera"></i>
          <h3>Photography</h3>
          <p>Photography é a arte ou prática de capturar imagens usando uma câmera. Envolve a habilidade de selecionar e
            enquadrar sujeitos, controlar a exposição da luz e utilizar técnicas criativas para transmitir emoções, contar
            histórias ou capturar a beleza do mundo ao nosso redor. A fotografia pode ser usada para diversos propósitos,
            como documentar eventos, expressar criatividade ou comunicar mensagens visualmente.</p>
        </li>
        <li>
          <i class="fa-solid fa-layer-group"></i>
          <h3>SEO Analyst</h3>
          <p>Um SEO Analyst é um profissional que trabalha com otimização de mecanismos de busca (SEO, na sigla em
            inglês). Eles são responsáveis por analisar, otimizar e melhorar a visibilidade de um site nos resultados de
            pesquisa. Isso envolve a pesquisa de palavras-chave relevantes, a otimização de conteúdo e estrutura do site,
            a criação de estratégias de link building e o monitoramento de métricas de desempenho. O objetivo do SEO
            Analyst é aumentar o tráfego orgânico e melhorar a posição do site nos rankings dos mecanismos de busca, para
            que ele seja mais facilmente encontrado pelos usuários.</p>
        </li>
        <li>
          <i class="fa-solid fa-medal"></i>
          <h3>Creative Design</h3>
          <p>Creative design é o processo de concepção e desenvolvimento de soluções visuais e estéticas inovadoras.
            Envolve a criação de designs originais e a aplicação de elementos como cor, forma, tipografia e layout para
            transmitir uma mensagem ou expressar uma ideia de maneira visualmente impactante. O creative design abrange
            várias áreas, como design gráfico, design de produtos, design de interação e muito mais, e é fundamental para
            criar uma identidade visual única e cativante para marcas, produtos ou projetos criativos.</p>
        </li>
        <li>
          <i class="fa-sharp fa-solid fa-palette"></i>
          <h3>UX/UI</h3>
          <p>UX/UI (User Experience/User Interface) refere-se à combinação de design de experiência do usuário e design de
            interface do usuário. O UX concentra-se em criar uma experiência agradável e intuitiva para os usuários ao
            interagir com um produto ou serviço, garantindo que suas necessidades sejam atendidas. O UI, por sua vez,
            concentra-se no design visual e funcional da interface do usuário, incluindo elementos como layout, cores,
            tipografia e ícones. A combinação de UX/UI visa fornecer uma experiência de usuário eficiente, envolvente e
            esteticamente agradável.</p>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>

export default {
  name: 'Services',

  setup() {
    return {

    }
  }
};
</script>

<style scoped>
/* SERVICES */
.services {
  margin-top: -30px;
  padding: 60px;
  background-color: #151515;
}

.my_services {
  padding: 60px;
  color: white;
}

.my_services ul {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  align-items: center;
  justify-content: center;
}

.my_services ul li {
  cursor: pointer;
  border-radius: 6px;
  position: relative;
  padding: 10px;
  display: grid;
  gap: 30px;
  text-align: center;
  max-width: 300px;
  align-content: center;
  height: 300px;
  background-color: #222;
}

.my_services ul li i {
  font-size: 2.7rem;
  color: #dc3545
}

.my_services ul li h3 {
  color: #fff;
  font-size: 1.6rem;
  font-family: 'Poppins';
  font-weight: 500;
}

.my_services ul li p {
  color: #707070;
  font-size: 1.1rem;
}

.my_services li::before {
  content: '';
  transition: .5s ease-in-out;
  border-radius: 6px;
  width: 0px;
  height: 0px;
  position: absolute;
  top: -2px;
  right: -2px;
  border-top: 2px solid transparent;
  border-right: 2px solid transparent
}

.my_services li::after {
  content: '';
  transition: .5s ease-in-out;
  border-radius: 6px;
  width: 0px;
  height: 0px;
  position: absolute;
  bottom: -2px;
  left: -2px;
  border-bottom: 2px solid transparent;
  border-left: 2px solid transparent
}

.my_services li:hover::before {
  width: 100%;
  height: 100%;
  border-top: 2px solid red;
  border-right: 2px solid red;
}

.my_services li:hover::after {
  width: 100%;
  height: 100%;
  border-bottom: 2px solid red;
  border-left: 2px solid red;
}
</style>