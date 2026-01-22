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

      <!-- Title -->
      <div class="row justify-content-center align-items-end flex-wrap">
        <div class="col-12 col-sm-4 col-md-3 col-lg-3 g-4">
          <h1 class="fw-bolder">
            What I do:
          </h1>
        </div>

        <!-- Expertise pills -->
        <div class="col-12 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            Full-Stack
          </div>
        </div>

        <div class="col-12 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            Front-End
          </div>
        </div>

        <div class="col-12 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            Back-End
          </div>
        </div>
      </div>

      <!-- Expertise pills pt2 -->
      <div class="row justify-content-center">

        <div class="col-12 col-sm-4 col-md-3 col-lg-3">
        </div>

        <div class="col-12 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            Web Design
          </div>
        </div>

        <div class="col-12 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            DB Management
          </div>
        </div>

        <div class="col-12 col-sm-4 col-md-3 col-lg-3 d-flex justify-content-center">
          <div class="round_div px-5 py-1 mb-2 me-2">
            API Integration
          </div>
        </div>
      </div>

      <!-- Skills -->
      <div class="row g-4 align-items-start skills_c">

        <!-- Title -->
        <div class="col-12 col-lg-2">
          <h1 class="fw-bolder">Skills/Tools:</h1>
        </div>

        <!-- Skills icon + name -->
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

    <div class="divider">
      . ݁₊ ⊹ . ݁˖ . ݁
    </div>
  </section>
</template>




<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;


section {
  color: $white;
  min-height: 90vh;
}

h1 {
  color: $pink;
}

.skill_img {
  width: 50px;
  padding-bottom: 10px;
}

$neonPink: #FD7E98;

.round_div {

  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 8px 24px;
  margin: 10px;
  min-width: 120px;
  border: 1.5px solid $neonPink;
  border-radius: 50px;

  // Glass background 
  background: rgba(253, 126, 152, 0.05);
  backdrop-filter: blur(5px);
  -webkit-backdrop-filter: blur(5px);


  // Neon Shadow (Refined) 
  box-shadow:
    0 0 10px rgba(253, 126, 152, 0.3),
    inset 0 0 5px rgba(253, 126, 152, 0.2);


  @media (max-width: 576px) {
    max-width: 250px;
    margin: 30px;
  }
}

.skills_c {
  padding-top: 130px;
}

.divider {
  height: 270px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: $pink;
  font-family: monospace;
  font-size: 2rem;
  font-weight: 300;
  letter-spacing: 12px;
  opacity: 0.4;
  text-shadow: 0 0 15px rgba(253, 126, 152, 0.2);
}
</style>
