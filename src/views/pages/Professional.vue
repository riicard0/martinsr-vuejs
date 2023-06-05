<template>
  <!-- RESUME -->
  <div id="professional" class="my_resume">
    <div class="sobre_titulo">
      <h1>Profissional</h1>
      <p>Experiências Profissionais</p>
      <div aria-label="seção apenas de ilustrações de botões">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>

    <!-- RESUME - EXPERIENCE -->
    <div class="resume_generico">
      <h2 class="experience"><i class="fa-solid fa-handshake"></i>EXPERIÊNCIA</h2>
      <div class="experience_content">
        <div>
          <span>jan.2022-nov.2022</span>
          <h3>Auxiliar de Logística - Grupo GTEX</h3>
          <p>Responsável por fazer a separação dos produtos de maneira pré-estabelecida de acordo com as notas fiscais,
            por paletizar as cargas para saída de produtos e demais outras ocorrências que são demandadas; também
            responsável pela organização das ruas E, F, G, e H, e separação de paletes para o setor de produção.</p>
        </div>
        <div>
          <span>jan.2019-ago.2019</span>
          <h3>Professor de Música - Autônomo</h3>
          <p>Ministrava aulas como professor de violão para alguns alunos, sendo aulas individuais.</p>
        </div>
        <div>
          <span>set.2014-ago.2015</span>
          <h3>Auxiliar Administrativo - Melhoramentos CMPC</h3>
          <p>Responsável por fornecer total suporte ao chefe do setor, seja fazendo requisições, etiquetas, impressões,
            etc., quanto auxiliando, quando necessário, os eletricistas e instrumentistas do setor. (Terceirizado pela
            Guarda Mirim de Suzano)</p>
        </div>

        <ul>
          <li><i class="fa-sharp fa-solid fa-circle"></i></li>
          <li><i class="fa-sharp fa-solid fa-circle"></i></li>
          <li><i class="fa-sharp fa-solid fa-circle"></i></li>
        </ul>
      </div>

      <!-- RESUME - EDUCATION -->
      <h2 class="education"><i class="fa-solid fa-book"></i>EDUCAÇÃO</h2>
      <div class="education_content">
        <div>
          <span>2014-2015</span>
          <h3>Jovem Aprendiz - Guarda Mirim de Suzano</h3>
          <p>Atuei cerca de 9 meses como aprendiz do curso somente, que me trouxe muito conhecimento. Depois mais 11 meses
            como jovem aprendiz na Melhoramentos CMPC.</p>
        </div>

        <ul>
          <li><i class="fa-sharp fa-solid fa-circle"></i></li>
        </ul>

      </div>
    </div>

  </div>
</template>

<script>

export default {
  name: 'Professional',

  setup() {
    return {

    }
  }
};
</script>

<style scoped></style>