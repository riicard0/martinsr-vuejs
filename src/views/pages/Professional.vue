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

<style scoped>
/* RESUME */
.my_resume {
  color: #fff;
}

.resume_generico {
  padding: 30px;
  display: grid;
  grid-template-columns: 1fr 1fr;
  justify-content: center;
  gap: 10px;
  align-items: start;
}

.resume_generico h2 {
  font-family: 'Poppins';
  font-size: 1.5rem;
  background-color: #ff5d56;
  justify-self: start;
  padding: 10px;
  border-radius: 3px;
}

.resume_generico h2 i {
  margin-right: 10px;
}

/* RESUME - EXPERIENCE */
.experience {
  margin-bottom: 30px;
  grid-column: 1;
  grid-row: 1;
}

.education {
  margin-bottom: 30px;
  grid-column: 2;
  grid-row: 1;
}

.experience_content ul {
  color: #ff5d56;
  gap: 10px;
  display: flex;
  cursor: pointer;
  margin-top: 20px;
  justify-content: center;
}

.resume_generico .experience_content div {
  background-color: #222;
  animation: ladoSecao .5s ease-in-out forwards;
  display: none;
  padding: 40px;
  position: relative;
}

.resume_generico .experience_content div.ativo {
  display: block;
}

.resume_generico .experience_content div::before {
  content: '';
  border-right: 30px solid transparent;
  border-bottom: 30px solid #222;
  position: absolute;
  top: -20px;
  left: 30px;
  display: inline-block;
}

.resume_generico .experience_content div span {
  color: #dc3545;
  font-family: 'Poppins';
  font-weight: bold;
}

.resume_generico .experience_content div h3 {
  font-family: 'Poppins';
  margin: 10px 0;
}

.resume_generico .experience_content div p {
  color: #707070;
  font-size: 1.1rem;
}

.experience_content ul li.ativo {
  color: #3e3d3d;
}

.experience_content ul li:hover {
  color: #ff0019;
}

/* RESUME - EDUCATION */
.resume_generico .education_content div {
  background-color: #222;
  padding: 40px;
  display: none;
  animation: ladoSecao .5s ease-in-out forwards;
  position: relative;
}

.education_content ul {
  color: #ff5d56;
  gap: 10px;
  display: flex;
  cursor: pointer;
  margin-top: 20px;
  justify-content: center;
}

.resume_generico .education_content div::before {
  content: '';
  border-right: 30px solid transparent;
  border-bottom: 30px solid #222;
  position: absolute;
  top: -20px;
  left: 30px;
  display: inline-block;
}

.resume_generico .education_content div span {
  color: #dc3545;
  font-family: 'Poppins';
  font-weight: bold;
}

.resume_generico .education_content div h3 {
  font-family: 'Poppins';
  margin: 10px 0;
}

.resume_generico .education_content div p {
  color: #707070;
  font-size: 1.1rem;
}

.education_content ul li.ativo {
  color: #3e3d3d;
}

.education_content ul li:hover {
  color: #ff0019;
}

.resume_generico .education_content div.ativo {
  display: block;
}

/* RESUME - COURSES */
.cursos {
  margin-top: 50px;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  align-items: start;
  padding: 30px;
  gap: 30px;
  justify-content: center;
}

.my_skill {
  display: grid;
}

.my_skill h2 {
  padding: 10px 30px;
  border-radius: 3px;
  background-color: #ff5d56;
  font-size: 1.5rem;
  font-family: 'Poppins';
  margin-bottom: 30px;
  justify-self: start;
}

.my_skill h2 i {
  padding-right: 10px;
}

.skill_content {
  font-size: 1.5rem;
  grid-column: 1/2;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
  margin-top: 10px;
}

.skill_content h3 {
  font-size: 1.5rem;
}

.skill_content ul {
  display: flex;
}
</style>