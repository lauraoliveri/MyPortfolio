<script>

import skillsData from '../data/skills.json';

export default {
  data() {
    return {
      skills: skillsData.skills,
      currentlyLearning: skillsData.currentlyLearning
    }
  }
}
</script>
<template>
  <section id="skills" class="py-5 px-3">
    <div class="container">

      <div class="row justify-content-center align-items-end">
        <div class="col-8 col-sm-4 col-md-3 col-lg-3">
          <h1 class="fw-bolder">
            What I do:
          </h1>
        </div>

        <div class="col-4 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            Full-Stack
          </div>
        </div>

        <div class="col-4 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            Front-End
          </div>
        </div>

        <div class="col-4 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            Back-End
          </div>
        </div>
      </div>

      <div class="row justify-content-center">

        <div class="col-8 col-sm-4 col-md-3 col-lg-3">
        </div>

        <div class="col-4 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            Web Design
          </div>
        </div>

        <div class="col-4 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            Responsive Design
          </div>
        </div>

        <div class="col-4 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            API Integration
          </div>
        </div>
      </div>

      <div class="row g-4 align-items-start skills_c">

        <!-- TITOLO -->
        <div class="col-12 col-lg-2">
          <h1 class="fw-bolder">Skills:</h1>
        </div>

        <!-- ICONE -->
        <div class="col-12 col-lg-10">
          <div class="row g-4">
            <div v-for="skill in skills" :key="skill.name"
              class="col-4 col-sm-4 col-md-3 col-lg-2 d-flex flex-column align-items-center">
              <img :src="skill.image" :alt="skill.name" class="skill_img mb-2" />
              <p class="text-uppercase text-center mb-0">{{ skill.name }}</p>
            </div>
          </div>
        </div>

      </div>



      <!-- Learning -->
      <!-- 
      <h3 class="text-center text-uppercase mt-5 mb-4">Currently Learning:</h3>

      <div class="row g-4 justify-content-center">
        <div
          v-for="skill in currentlyLearning"
          :key="skill.name"
          class="col-6 col-sm-4 col-md-3 col-lg-2 d-flex flex-column align-items-center"
        >
          <img :src="skill.image" :alt="skill.name" class="skill_img mb-2" />
          <p class="text-uppercase text-center mb-0">{{ skill.name }}</p>
        </div>
      </div> 
    -->
    </div>
  </section>
</template>




<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;


section {
  color: $white;
}

h1 {
  color: $black;
}

.skill_img {
  width: 50px;
  padding-bottom: 10px;
}

.round_div {
  width: 250px;
  background-color: $pink;
  border-radius: 20px;
  text-align: center;

  /* Neon shadow */
  box-shadow:
    0 0 8px rgba($pink, 0.6),
    0 0 16px rgba($pink, 0.4),
    0 0 24px rgba($white, 0.15);
}

.skills_c {
  padding-top: 130px;
}
</style>
