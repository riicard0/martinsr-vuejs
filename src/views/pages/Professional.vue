<template>
  <!-- RESUME -->
  <div id="professional" class="my_resume site-website">
    <div class="sobre_titulo">
      <h1>Professional</h1>
      <p>Professional Experience || Professional Education</p>
      <div aria-label="seção apenas de ilustrações de botões">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>

    <!-- RESUME - EXPERIENCE -->
    <div class="resume_generico">
      <h2 class="experience"><i class="fa-solid fa-handshake"></i>EXPERIENCE</h2>
      <div class="experience_content">
        <div>
          <span>jan.2022-nov.2022</span>
          <h3>Logistics Assistant - GTEX Group</h3>
          <p>Responsible for sorting products according to pre-established criteria based on invoices, palletizing loads
            for product delivery, and handling other required tasks. Also responsible for organizing aisles E, F, G, and
            H, as well as pallet separation for the production department.</p>
        </div>
        <div>
          <span>jan.2019-ago.2019</span>
          <h3>Music Teacher - Self-employed</h3>
          <p>I used to teach guitar lessons to a few students, providing individual lessons.</p>
        </div>
        <div>
          <span>set.2014-ago.2015</span>
          <h3>Administrative Assistant - Melhoramentos CMPC</h3>
          <p>Responsible for providing full support to the department head, including making requests, labels, prints,
            etc., as well as assisting, when necessary, the electricians and instrument technicians in the department.
            (Outsourced by "Guarda Mirim de Suzano")</p>
        </div>

        <ul>
          <li><i class="fa-sharp fa-solid fa-circle"></i></li>
          <li><i class="fa-sharp fa-solid fa-circle"></i></li>
          <li><i class="fa-sharp fa-solid fa-circle"></i></li>
        </ul>
      </div>

      <!-- RESUME - EDUCATION -->
      <h2 class="education"><i class="fa-solid fa-book"></i>EDUCATION</h2>
      <div class="education_content">
        <div>
          <span>2014-2015</span>
          <h3>Young Apprentice - Guarda Mirim de Suzano</h3>
          <p>I worked for about 9 months as an apprentice in the course only, which brought me a lot of knowledge. Then,
            another 11 months as a youth apprentice at Melhoramentos CMPC.</p>
        </div>

        <ul>
          <li><i class="fa-sharp fa-solid fa-circle"></i></li>
        </ul>

      </div>
    </div>

  </div>
</template>

<script>
import { ref, onMounted } from 'vue';

export default {
  name: 'Professional',

  setup() {
    const divExperience = ref([]);
    const liExperience = ref([]);
    const divEducation = ref([]);
    const liEducation = ref([]);
    const activeDivExperience = ref(0);
    const activeDivEducation = ref(0);

    function slideShow(index) {
      divExperience.value.forEach((div) => {
        div.classList.remove('ativo');
      });
      liExperience.value.forEach((botao) => {
        botao.classList.remove('ativo');
      });

      divExperience.value[index].classList.add('ativo');
      liExperience.value[index].classList.add('ativo');

      activeDivExperience.value = index;
    }

    function slideShow2(index) {
      divEducation.value.forEach((div) => {
        div.classList.remove('ativo');
      });
      liEducation.value.forEach((botao) => {
        botao.classList.remove('ativo');
      });

      divEducation.value[index].classList.add('ativo');
      liEducation.value[index].classList.add('ativo');

      activeDivEducation.value = index;
    }

    onMounted(() => {
      divExperience.value = document.querySelectorAll('.experience_content div');
      liExperience.value = document.querySelectorAll('.experience_content ul li');
      divEducation.value = document.querySelectorAll('.education_content div');
      liEducation.value = document.querySelectorAll('.education_content ul li');

      divExperience.value[0].classList.add('ativo');
      liExperience.value[0].classList.add('ativo');
      divEducation.value[0].classList.add('ativo');
      liEducation.value[0].classList.add('ativo');
    });

    return {
      divExperience,
      liExperience,
      divEducation,
      liEducation,
      activeDivExperience,
      activeDivEducation,
      slideShow,
      slideShow2
    }
  }
};
</script>

<style scoped>
/* RESUME */
.my_resume {
  color: var(--color-4);
  padding: 40px;
}

.my_resume::after {
  content: '';
  display: block;
  background-color: var(--color-2);
  width: 300px;
  height: 6px;
  border-radius: 5px;
  margin: 1% auto -1rem auto;
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
  background-color: var(--color-3);
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
  color: var(--color-5);
  gap: 10px;
  display: flex;
  cursor: pointer;
  margin-top: 20px;
  justify-content: center;
}

.resume_generico .experience_content div {
  background-color: var(--color-9);
  animation: ladoSecao .5s ease-in-out forwards;
  display: none;
  padding: 40px;
  position: relative;
  border-radius: 5px 40px 40px 40px;
}

.resume_generico .experience_content div.ativo {
  display: block;
}

.resume_generico .experience_content div::before {
  content: '';
  border-right: 30px solid transparent;
  border-bottom: 30px solid var(--color-9);
  position: absolute;
  top: -20px;
  left: 30px;
  display: inline-block;
}

.resume_generico .experience_content div span {
  color: var(--color-5);
  font-family: var(--font-1);
  font-weight: bold;
}

.resume_generico .experience_content div h3 {
  font-family: var(--font-1);
  margin: 10px 0;
}

.resume_generico .experience_content div p {
  color: var(--color-3);
  font-size: 1.1rem;
}

.experience_content ul li.ativo {
  color: var(--color-9);
}

.experience_content ul li:hover {
  color: var(--color-3);
}

/* RESUME - EDUCATION */
.resume_generico .education_content div {
  background-color: var(--color-9);
  padding: 40px;
  display: none;
  animation: ladoSecao .5s ease-in-out forwards;
  position: relative;
  border-radius: 5px 40px 40px 40px;
}

.education_content ul {
  color: var(--color-5);
  gap: 10px;
  display: flex;
  cursor: pointer;
  margin-top: 20px;
  justify-content: center;
}

.resume_generico .education_content div::before {
  content: '';
  border-right: 30px solid transparent;
  border-bottom: 30px solid var(--color-9);
  position: absolute;
  top: -20px;
  left: 30px;
  display: inline-block;
}

.resume_generico .education_content div span {
  color: var(--color-5);
  font-family: var(--font-1);
  font-weight: bold;
}

.resume_generico .education_content div h3 {
  font-family: var(--font-1);
  margin: 10px 0;
}

.resume_generico .education_content div p {
  color: var(--color-3);
  font-size: 1.1rem;
}

.education_content ul li.ativo {
  color: var(--color-9);
}

.education_content ul li:hover {
  color: var(--color-3);
}

.resume_generico .education_content div.ativo {
  display: block;
}
</style>