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
    <div class="container-fluid">

      <!-- Skills -->
      <div class="row g-4 justify-content-center">
        <div class="col-8 col-sm-4 col-md-3 col-lg-6 d-flex justify-content-start">
          <h1>
            What I do:
          </h1>
        </div>
        <div class="col-2 col-sm-4 col-md-3 col-lg-3 d-flex flex-column align-items-start">
         <div>
          Full-Stack
         </div>
        </div>
        <div class="col-2 col-sm-4 col-md-3 col-lg-3 d-flex flex-column align-items-start">
         <div>
          Full-Stack
         </div>
        </div>
      </div>


      <div class="row g-4 justify-content-center">
        <div class="col-8 col-sm-4 col-md-3 col-lg-2">
          <h1>
            Skills:
          </h1>
        </div>
        <div
          v-for="skill in skills"
          :key="skill.name"
          class="col-4 col-sm-4 col-md-3 col-lg-2 d-flex flex-column align-items-center"
        >
          <img :src="skill.image" :alt="skill.name" class="skill_img mb-2" />
          <p class="text-uppercase text-center mb-0">{{ skill.name }}</p>
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
  background-color: $black;
  color: $white;
  min-height: 100vh;

  @include underline-on-hover;
}

h1, h3{
  font-family: 'VT323', sans-serif;  
  color: $pink;
}

.container-fluid{
  background: #FD7E98;
  background: linear-gradient(146deg, rgba(253, 126, 152, 1) 0%, rgba(0, 0, 0, 1) 100%);
  border-radius: 20px;
  margin: 0;
}


.skill_img {
  width: 100px;
  padding-bottom: 10px;
}
</style>
