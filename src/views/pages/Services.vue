<template>
  <!-- SERVICES -->
  <section id="services" class="services">
    <div class="sobre_titulo">
      <h1>Services</h1>
      <p>Comprehensive knowledge in the field</p>
      <div aria-label="seção com botões sobre os conhecimentos Front-End">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>

    <div class="my_services site-website">
      <ul aria-label="navegação secundária">
        <li>
          <i class="fa-sharp fa-solid fa-pen-to-square"></i>
          <h3>Web Design</h3>
          <p>Web Design is the planning and creation of visual elements to provide a pleasant user experience.</p>
        </li>
        <li>
          <i class="fa-solid fa-globe"></i>
          <h3>Web Developer</h3>
          <p>Web Developer creates, develops, solves problems, ensures responsiveness, security, and a good user
            experience.</p>
        </li>
        <li>
          <i class="fa-solid fa-graduation-cap"></i>
          <h3>Student</h3>
          <p>Development Student seeks to enhance programming skills, learn new technologies, and develop projects to
            gain practical experience.</p>
        </li>
        <li>
          <i class="fa-solid fa-layer-group"></i>
          <h3>SEO Analyst</h3>
          <p>SEO Analyst optimizes the content by researching keywords and seeking resources to improve organic
            traffic and rankings.</p>
        </li>
        <li>
          <i class="fa-solid fa-user-shield"></i>
          <h3>Security</h3>
          <p>Security is the implementation of measures to protect websites and applications against threats and
            vulnerabilities, ensuring data integrity and confidentiality.</p>
        </li>
        <li>
          <i class="fa-sharp fa-solid fa-palette"></i>
          <h3>UX/UI</h3>
          <p>UX/UI combines user experience design and user interface design, creating an intuitive and pleasant
            experience with engaging and functional visual design.</p>
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
  padding: 40px;
  background-color: var(--color-8);
  height: 100vh;
}

.my_services {
  padding: 60px;
  color: var(--color-2);

}

.services::after {
  content: '';
  display: block;
  background-color: var(--color-2);
  width: 300px;
  height: 6px;
  border-radius: 5px;
  margin: 1% auto -5rem auto;
}

.my_services ul {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  align-items: center;
  justify-content: center;
}

.my_services ul li {
  border-radius: 6px;
  position: relative;
  padding: 10px;
  display: grid;
  gap: 30px;
  text-align: center;
  max-width: 300px;
  align-content: center;
  height: 300px;
  background-color: var(--color-9);
}

.my_services ul li i {
  font-size: 2.7rem;
  color: var(--color-5);
}

.my_services ul li h3 {
  color: var(--color-2);
  font-size: 1.6rem;
  font-family: var(--font-1);
  font-weight: 500;
}

.my_services ul li p {
  color: var(--color-3);
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
  border-top: 2px solid var(--color-5);
  border-right: 2px solid var(--color-5);
}

.my_services li:hover::after {
  width: 100%;
  height: 100%;
  border-bottom: 2px solid var(--color-5);
  border-left: 2px solid var(--color-5);
}
</style>